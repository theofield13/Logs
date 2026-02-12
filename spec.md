# Stress Scenario Generator — spec.md

## 1. Purpose
Build an application that generates **regulator-appropriate stress scenarios** for financial risk management (ICAAP, ILAAP, ESG/climate, IFRS 9), integrates required **client and macro data**, applies scenarios to produce **transparent and auditable impacts** on key risk indicators, and generates an **AI-assisted report** aligned with regulatory expectations. The solution must be implementable in **Palantir Foundry**.

---

## 2. Core principles (must-haves)
- **Supervisory-proofing:** scenario definitions, narratives, and impact logic must be defensible and reviewable.
- **Transparency:** every output must be traceable back to inputs, assumptions, and impact methods.
- **Reproducibility:** same versions of inputs + scenario + heuristics must reproduce the same results.
- **Human-in-the-loop governance:** approvals are required before scenarios/heuristics/reports are used or exported.
- **Versioning & lineage:** scenarios, macro snapshots, client datasets, heuristics, and reports must be versioned with audit logs.

---

## 3. MVP scope
### In scope (MVP)
- Support at least **IFRS 9** and one of **ICAAP** or **ILAAP**.
- Scenario engine: template-driven + AI-generated scenario candidates + approval workflow.
- Client data integration: scenario-type-specific **data contracts**, mapping, and validation.
- Macro integration: ingest historical + (where possible) near real-time macro data from free sources, with snapshotting.
- Impact engine: apply scenarios to client data using a governed **Impact Heuristics Library** (RULE-based in MVP).
- AI report: generate a report grounded in approved scenario content + computed results, export as markdown.

### Out of scope (MVP)
- Full econometric forecasting/calibration framework.
- Full model risk management suite beyond basic approval/audit/versioning.
- Full jurisdiction-specific submission formats for all regulators.

---

## 4. Primary workflows

### 4.1 Scenario creation and approval
1. User selects:
   - scenario type (ICAAP / ILAAP / ESG / IFRS9)
   - regulator context (jurisdiction, regulators)
   - horizon and frequency (e.g., 36 months, monthly)
   - severity (baseline/adverse/severe)
2. System loads:
   - scenario template for the chosen type/context
   - required macro variables and constraints
   - required client data contract
3. AI generates N candidate scenarios (default 3):
   - assumptions list (explicit, enumerated)
   - macro variable paths/shocks
   - narrative draft aligned to the template
4. User selects/edits candidate.
5. Approver reviews and signs off → scenario becomes **APPROVED**.

### 4.2 Client data onboarding
1. System presents a **data contract** required for the chosen scenario type.
2. Client provides datasets.
3. User maps client fields to canonical fields.
4. System validates:
   - schema completeness and types
   - quality rules (ranges, null checks, keys uniqueness)
5. System outputs a **conformed dataset** + data quality report, versioned.

### 4.3 Macro data ingestion
1. System ingests macro time series from configured free sources.
2. System normalizes units and frequency.
3. System creates a **macro snapshot** (immutable) with provenance and licensing notes.
4. Scenario/run references a specific macro snapshot ID.

### 4.4 Run impact calculation
1. User selects:
   - approved scenario version
   - client dataset versions
   - approved heuristic set versions
2. System executes impact engine:
   - applies scenario macro shocks/paths
   - computes impacts on KPIs using heuristics
3. System outputs:
   - impact dataset (KPIs)
   - aggregation dataset (portfolio/entity summaries)
   - explainability dataset (inputs, intermediates, heuristic IDs/versions)

### 4.5 Report generation
1. User selects report template based on scenario type + regulator context.
2. AI drafts report text using only:
   - approved scenario content
   - computed outputs
   - approved template boilerplate
3. Approver signs off → report becomes exportable.

---

## 5. Functional requirements

### 5.1 Scenario Engine
- Must support scenario types: ICAAP, ILAAP, ESG/climate, IFRS 9 (MVP requires IFRS 9 + one of ICAAP/ILAAP).
- Must be template-driven (required macro vars, narrative structure, constraints).
- Must generate multiple candidate scenarios (AI-assisted).
- Must enforce approval gates before scenario is executable.
- Must store assumptions explicitly and label AI-generated content until approved.

### 5.2 Client Data Integration
- Must provide a data contract per scenario type describing:
  - required datasets
  - required columns, types, constraints
  - keys and quality rules
- Must support mapping from client schema to canonical schema.
- Must output conformed datasets and validation reports.
- Must version datasets and mapping configurations.

### 5.3 Macro Data Integration
- Must ingest historical and (where possible) near real-time macro data from free sources (initially).
- Must normalize units and align frequency.
- Must snapshot macro data and reference snapshots by ID.
- Must store provenance (source, retrieval time) and licensing notes.

### 5.4 Impact Engine + Impact Heuristics Library
- Must apply scenarios to client data to compute impacts on key risk indicators.
- Must use a governed, versioned library of heuristics:
  - MVP supports RULE heuristics (explicit formulas + parameters).
- Must produce explainability artifacts that allow validation:
  - heuristic ID/version used
  - inputs used
  - intermediate values (where applicable)
  - final outputs
- Must enforce approvals for heuristics before use.

### 5.5 AI Report
- Must generate an AI-assisted report aligned to the selected regulatory context.
- Must be grounded only in approved scenario content and computed results (no invented numbers).
- Must include:
  - scenario overview + assumptions
  - methodology (data sources, contracts, heuristic versions)
  - results (KPIs, summary tables)
  - limitations and validation notes
  - audit appendix (IDs/versions/timestamps)

---

## 6. Governance and audit
- Mandatory approval stages:
  - Scenario approval
  - Heuristic approval
  - Report approval
- Audit log must record:
  - scenario generation events and edits
  - approvals (who/when/what)
  - macro snapshot creation
  - runs executed (inputs versions)
  - report generation and export
- Reproducibility requires pinning:
  - scenario ID + version
  - macro snapshot ID
  - client dataset versions
  - heuristic IDs + versions

---

## 7. Palantir Foundry implementation constraints
- Design must be compatible with Foundry patterns:
  - datasets for inputs/outputs
  - pipelines for transformations
  - ontology objects for Scenario, Heuristic, Run, MacroSnapshot, Report
  - workflow states for approvals
- Outputs must be materialized as datasets + report artifacts (markdown/PDF later).

---

## 8. MVP acceptance criteria
- User can: select scenario type → generate candidates → approve scenario → ingest/map/validate client data → ingest macro snapshot → run impact computation with approved heuristics → generate and approve report → export.
- Every KPI in outputs is traceable to:
  - scenario definition and assumptions
  - macro snapshot and transformations
  - client dataset version
  - heuristic ID/version and parameters
- Rerunning with the same versions produces identical results.

