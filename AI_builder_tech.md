# AI Automation Builder Course: 6-Month Roadmap (Technical/Developer Path)
**1 Hour/Day • Monday–Friday Only • Total: ~130 hours (core) + ~60 hours dev add-ons**

**Article is available here:** https://x.com/DeRonin_/status/2043722737080819983 

**Start date assumption**: Next Monday (or Day 1 = your first available Monday).  
**Path**: **Technical/Developer** — You already code (or are ready to). You follow the **exact same core n8n roadmap** as the non-technical path (because n8n is still the fastest way to ship client work and get paid), **BUT** you ALSO complete the “Developer Path” add-ons at the end of each month. This unlocks bigger contracts, custom backends, LangGraph agents, and full-stack AI automations.  
**Rule**: 1 hour max per day. Split your hour between core + dev add-on if needed (e.g., 40 min core, 20 min dev). Build the habit.  
**How to use this file**:  
1. Copy the entire content into `ai-automation-roadmap-todo-technical.md`.  
2. Open in any markdown editor that supports checkboxes (Notion, Obsidian, Typora, VS Code, etc.).  
3. Check the box **✅** when you finish the task.  
4. Complete **both** the core milestone **and** the dev add-on milestone before moving to the next month.  

**Tools needed from Day 1**: Free n8n account, Postman, Notion, OpenAI/Anthropic API key, Python environment (for dev add-ons), GitHub account.

---

## Month 1: Build your first workflow in n8n + Just enough Python
**Goal (core)**: Master n8n + APIs + prompting. Build 1 personal automation.  
**Goal (dev add-on)**: Learn just enough Python to read docs, write small scripts, and glue things when n8n hits a wall.

### Week 1
- [ ] **Monday**: Read n8n Official Docs — Quickstart + Core Concepts (Triggers, Actions, Data flow). Take notes on how data moves between nodes. (docs.n8n.io)
- [ ] **Tuesday**: Complete n8n Academy first 2 beginner modules. Create your first empty workflow and add a Schedule Trigger + Set node.
- [ ] **Wednesday**: Watch Productive Dude YouTube (first 2 beginner videos). Build a simple “Daily price checker → Google Sheet” workflow.
- [ ] **Thursday**: Finish n8n Academy core concepts. Practice error handling and fallback paths in a test workflow.
- [ ] **Friday**: Add HTTP Request node to your test workflow. Test with a free public API (e.g. GitHub API).

### Week 2
- [ ] **Monday**: Study “What is a Webhook?” (Zapier blog) + MDN HTTP basics. Take notes on GET/POST/PUT/DELETE and status codes.
- [ ] **Tuesday**: Go through Postman “Getting Started” lessons. Make your first API call in Postman (GitHub user example).
- [ ] **Wednesday**: Recreate the exact same GitHub API call inside n8n HTTP Request node. Compare JSON output.
- [ ] **Thursday**: Read REST API Tutorial (restfulapi.net). Focus on JSON structure, rate limits, and authentication (API keys vs Bearer).
- [ ] **Friday**: Build a personal automation: Auto-save email attachments to Google Drive (or similar low-stakes task).

### Week 3
- [ ] **Monday**: Read “How to Read API Documentation” (Postman blog). Study Stripe API docs as example.
- [ ] **Tuesday**: Pick any tool you already use (Notion, Slack, Airtable, HubSpot). Find its API docs and locate Authentication + one endpoint.
- [ ] **Wednesday**: In Postman, make ONE successful API call to that tool. Document the request/response.
- [ ] **Thursday**: Replicate the same call inside n8n. Handle JSON parsing.
- [ ] **Friday**: Review all API concepts. Build a second personal automation that uses an API.

### Week 4
- [ ] **Monday**: Start Anthropic Interactive Prompt Engineering Tutorial (GitHub). Complete first 3 chapters.
- [ ] **Tuesday**: Finish Anthropic tutorial + OpenAI Prompt Engineering Guide. Focus on system vs user prompts and structured JSON output.
- [ ] **Wednesday**: Read LearnPrompting.org basics + the advanced article from @EXM7777. Practice few-shot prompting.
- [ ] **Thursday**: Watch 1–2 Andrej Karpathy videos + skim Simon Willison’s recent posts. List 5 things LLMs are good at and 5 they’re bad at.
- [ ] **Friday**: **Core Month 1 Milestone** — Build a 3–5 step personal workflow. Explain webhooks, JSON, status codes, and prompts in plain English. Review everything.

**Developer Path Add-on (spread across the month — do 1–2 per week in your 1 hour)**  
- [ ] Complete Python for Everybody (Coursera, audit) OR freeCodeCamp Python Course — focus on variables, loops, conditionals, functions, lists, dicts, JSON, requests library, try/except.  
- [ ] Read chapters 1–8 of Automate the Boring Stuff with Python (free book).  
- [ ] Write 3 small scripts: (1) fetch GitHub API with requests, (2) parse JSON and save to CSV, (3) simple error-handling wrapper.  
- [ ] **Dev Month 1 Milestone** — Run a Python script that calls the same API you used in n8n and prints structured output. You can now read Python code in API docs.

---

## Month 2: Embed AI into your workflows + Call LLMs from Python
**Goal (core)**: 3–5 AI-powered workflows running automatically.  
**Goal (dev add-on)**: Make the same LLM calls from Python that you make in n8n (for custom backends later).

### Week 5
- [ ] **Monday**: Read n8n AI Nodes + LangChain docs (full AI section).
- [ ] **Tuesday**: Complete n8n Academy AI Workflows course (first half).
- [ ] **Wednesday**: Import 3 AI templates from n8n.io/workflows/?categories=AI. Run and dissect them.
- [ ] **Thursday**: Build practice project #1: Google Form → LLM classification → Airtable.
- [ ] **Friday**: Build practice project #2: Gmail trigger → AI classify email → route to different actions.

### Week 6
- [ ] **Monday**: Read Anthropic “Building Effective Agents” (workflow patterns section only).
- [ ] **Tuesday**: Sketch 3 real business skeletons on paper (Trigger → AI → Action → Output).
- [ ] **Wednesday**: Build one full email triage workflow (Gmail → AI classify → route to Slack/CRM/archive).
- [ ] **Thursday**: Study n8n Error Handling & Retry docs. Add error workflow + Slack notification.
- [ ] **Friday**: Add retry-on-fail + fallback logic to all previous workflows.

### Week 7
- [ ] **Monday**: Study OpenAI + Anthropic pricing pages + Tokenizer tool.
- [ ] **Tuesday**: Calculate monthly cost for your email triage workflow (assume 1,000 emails/day).
- [ ] **Wednesday**: Recalculate for 2 more workflows you’ve built.
- [ ] **Thursday**: Early Monetization prep — Create Upwork profile (“AI Automation Builder — n8n Specialist”). Write bio and first proposal template.
- [ ] **Friday**: **Core Month 2 Milestone** — Have 3–5 working AI workflows. Estimate costs accurately. Identify your first $300–$500 gig.

### Week 8 (Early Monetization push)
- [ ] **Monday**: Apply to 3–5 Upwork/Fiverr jobs (or post 1 workflow on X/LinkedIn). Record 1 Loom demo.
- [ ] **Tuesday**: Apply to 3–5 Upwork/Fiverr jobs (or post 1 workflow on X/LinkedIn). Record 1 Loom demo.
- [ ] **Wednesday**: Apply to 3–5 Upwork/Fiverr jobs (or post 1 workflow on X/LinkedIn). Record 1 Loom demo.
- [ ] **Thursday**: Apply to 3–5 Upwork/Fiverr jobs (or post 1 workflow on X/LinkedIn). Record 1 Loom demo.
- [ ] **Friday**: Apply to 3–5 Upwork/Fiverr jobs (or post 1 workflow on X/LinkedIn). Record 1 Loom demo.

**Developer Path Add-on**  
- [ ] Complete OpenAI API Quickstart + Anthropic API Quickstart (official docs).  
- [ ] Work through OpenAI Cookbook examples (chat completions, structured output, function calling).  
- [ ] Build 2 Python scripts: (1) same email-classification chain as your n8n workflow, (2) cost calculator that estimates tokens before calling the model.  
- [ ] **Dev Month 2 Milestone** — You can now call OpenAI/Anthropic from Python with temperature=0, system prompts, and parse JSON responses reliably.

---

## Month 3: Build 1–2 repeatable service workflows
**Goal (core)**: 1–2 polished, sellable automations + first paying client (or pilot).  
**Goal (dev add-on)**: Add custom Python/RAG where n8n alone isn’t enough (especially for knowledge bots).

**Pick your 1–2 use cases** (Lead Gen or Cold Outreach recommended for highest demand).

### Week 9–10 (Days 41–50)
- [ ] **Monday**: Build the chosen workflow step-by-step (30 min nodes + 30 min testing + documenting).
- [ ] **Tuesday**: Build the chosen workflow step-by-step (30 min nodes + 30 min testing + documenting).
- [ ] **Wednesday**: Build the chosen workflow step-by-step (30 min nodes + 30 min testing + documenting).
- [ ] **Thursday**: Build the chosen workflow step-by-step (30 min nodes + 30 min testing + documenting).
- [ ] **Friday**: Build the chosen workflow step-by-step (30 min nodes + 30 min testing + documenting).

### Week 11
- [ ] **Monday**: Polish the workflow (error handling, cost calc, Loom video, Notion handoff doc). Create fixed-price offer ($300–$700).
- [ ] **Tuesday**: Polish the workflow (error handling, cost calc, Loom video, Notion handoff doc). Create fixed-price offer ($300–$700).
- [ ] **Wednesday**: Polish the workflow (error handling, cost calc, Loom video, Notion handoff doc). Create fixed-price offer ($300–$700).
- [ ] **Thursday**: Polish the workflow (error handling, cost calc, Loom video, Notion handoff doc). Create fixed-price offer ($300–$700).
- [ ] **Friday**: Polish the workflow (error handling, cost calc, Loom video, Notion handoff doc). Create fixed-price offer ($300–$700).

### Week 12
- [ ] **Monday**: Launch on Upwork/Fiverr/Contra + n8n Template Marketplace. Deliver first gig or free pilot.
- [ ] **Tuesday**: Launch on Upwork/Fiverr/Contra + n8n Template Marketplace. Deliver first gig or free pilot.
- [ ] **Wednesday**: Launch on Upwork/Fiverr/Contra + n8n Template Marketplace. Deliver first gig or free pilot.
- [ ] **Thursday**: Launch on Upwork/Fiverr/Contra + n8n Template Marketplace. Deliver first gig or free pilot.
- [ ] **Friday**: **Core Month 3 Milestone** — 1–2 repeatable workflows + at least 1 paying client (or pilot).

**Developer Path Add-on**  
- [ ] For your chosen use case, add a custom Python script (or LangChain/LlamaIndex RAG if doing Internal Knowledge Bot).  
- [ ] Deploy one small FastAPI endpoint (optional) that your n8n workflow can call as a custom node.  
- [ ] **Dev Month 3 Milestone** — You have at least one workflow that mixes n8n + custom Python code.

---

## Month 4: Add AI agents to your toolbox + Python agent frameworks
**Goal (core)**: Know exactly when to use agents vs simple chains.  
**Goal (dev add-on)**: Build production-grade agents with LangGraph/CrewAI.

### Week 13
- [ ] **Monday**: Read Anthropic “Building Effective Agents” (full) + OpenAI Practical Guide to Agents. Take notes on the loop and when agents are overkill.
- [ ] **Tuesday**: Read Anthropic “Building Effective Agents” (full) + OpenAI Practical Guide to Agents. Take notes on the loop and when agents are overkill.
- [ ] **Wednesday**: Read Anthropic “Building Effective Agents” (full) + OpenAI Practical Guide to Agents. Take notes on the loop and when agents are overkill.
- [ ] **Thursday**: Read Anthropic “Building Effective Agents” (full) + OpenAI Practical Guide to Agents. Take notes on the loop and when agents are overkill.
- [ ] **Friday**: Read Anthropic “Building Effective Agents” (full) + OpenAI Practical Guide to Agents. Take notes on the loop and when agents are overkill.

### Week 14
- [ ] **Monday**: Study n8n AI Agent Node docs + import 3 agent templates. Build your first support agent (Tier-1 ticket handler).
- [ ] **Tuesday**: Study n8n AI Agent Node docs + import 3 agent templates. Build your first support agent (Tier-1 ticket handler).
- [ ] **Wednesday**: Study n8n AI Agent Node docs + import 3 agent templates. Build your first support agent (Tier-1 ticket handler).
- [ ] **Thursday**: Study n8n AI Agent Node docs + import 3 agent templates. Build your first support agent (Tier-1 ticket handler).
- [ ] **Friday**: Study n8n AI Agent Node docs + import 3 agent templates. Build your first support agent (Tier-1 ticket handler).

### Week 15
- [ ] **Monday**: Add human-in-the-loop (Wait node + Slack approval) to all agents. Practice deciding chain vs agent for 5 business tasks.
- [ ] **Tuesday**: Add human-in-the-loop (Wait node + Slack approval) to all agents. Practice deciding chain vs agent for 5 business tasks.
- [ ] **Wednesday**: Add human-in-the-loop (Wait node + Slack approval) to all agents. Practice deciding chain vs agent for 5 business tasks.
- [ ] **Thursday**: Add human-in-the-loop (Wait node + Slack approval) to all agents. Practice deciding chain vs agent for 5 business tasks.
- [ ] **Friday**: Add human-in-the-loop (Wait node + Slack approval) to all agents. Practice deciding chain vs agent for 5 business tasks.

### Week 16
- [ ] **Monday**: Build reliability (max iterations, logging, retries). Test edge cases.
- [ ] **Tuesday**: Build reliability (max iterations, logging, retries). Test edge cases.
- [ ] **Wednesday**: Build reliability (max iterations, logging, retries). Test edge cases.
- [ ] **Thursday**: Build reliability (max iterations, logging, retries). Test edge cases.
- [ ] **Friday**: **Core Month 4 Milestone** — Working n8n agent + clear decision framework for when to use agents.

**Developer Path Add-on**  
- [ ] Complete LangGraph intro course (academy.langchain.com).  
- [ ] Build one small agent with CrewAI or AutoGen (multi-agent optional).  
- [ ] **Dev Month 4 Milestone** — You can now choose between n8n Agent node **or** a custom LangGraph agent depending on the client need.

---

## Month 5: Make your automations production-ready
**Goal (core)**: Deploy, monitor, and hand off to non-technical clients.  
**Goal (dev add-on)**: Add custom Python backends and advanced monitoring where needed.

### Week 17
- [ ] **Monday**: Deploy n8n on Railway (1-click). Set up custom domain + HTTPS. Test all previous workflows on production instance.
- [ ] **Tuesday**: Deploy n8n on Railway (1-click). Set up custom domain + HTTPS. Test all previous workflows on production instance.
- [ ] **Wednesday**: Deploy n8n on Railway (1-click). Set up custom domain + HTTPS. Test all previous workflows on production instance.
- [ ] **Thursday**: Deploy n8n on Railway (1-click). Set up custom domain + HTTPS. Test all previous workflows on production instance.
- [ ] **Friday**: Deploy n8n on Railway (1-click). Set up custom domain + HTTPS. Test all previous workflows on production instance.

### Week 18
- [ ] **Monday**: Add global monitoring (error workflows, logging, uptime checks). Create client handoff package (JSON export + Loom + Notion doc).
- [ ] **Tuesday**: Add global monitoring (error workflows, logging, uptime checks). Create client handoff package (JSON export + Loom + Notion doc).
- [ ] **Wednesday**: Add global monitoring (error workflows, logging, uptime checks). Create client handoff package (JSON export + Loom + Notion doc).
- [ ] **Thursday**: Add global monitoring (error workflows, logging, uptime checks). Create client handoff package (JSON export + Loom + Notion doc).
- [ ] **Friday**: Add global monitoring (error workflows, logging, uptime checks). Create client handoff package (JSON export + Loom + Notion doc).

### Week 19
- [ ] **Monday**: Practice handoff with a mock client (friend/family). Add 7-day support process.
- [ ] **Tuesday**: Practice handoff with a mock client (friend/family). Add 7-day support process.
- [ ] **Wednesday**: Practice handoff with a mock client (friend/family). Add 7-day support process.
- [ ] **Thursday**: Practice handoff with a mock client (friend/family). Add 7-day support process.
- [ ] **Friday**: Practice handoff with a mock client (friend/family). Add 7-day support process.

### Week 20
- [ ] **Monday**: Review all workflows for production readiness. Fix any remaining issues.
- [ ] **Tuesday**: Review all workflows for production readiness. Fix any remaining issues.
- [ ] **Wednesday**: Review all workflows for production readiness. Fix any remaining issues.
- [ ] **Thursday**: Review all workflows for production readiness. Fix any remaining issues.
- [ ] **Friday**: **Core Month 5 Milestone** — All workflows deployed, monitored, and ready to hand off.

**Developer Path Add-on**  
- [ ] Add custom Python/FastAPI microservice for any complex logic your n8n workflows call.  
- [ ] Set up structured logging + basic observability (e.g., Prometheus or simple Slack alerts from Python).  
- [ ] **Dev Month 5 Milestone** — You can hand off a hybrid n8n + custom Python solution that a non-technical client can still manage.

---

## Month 6: Scale & become hireable
**Goal (core)**: Portfolio, advanced use cases, consistent income.  
**Goal (dev add-on)**: Full custom backends and advanced agent orchestration.

### Week 21–24 (Daily focus — repeat this pattern)
- [ ] **Monday**: Build 1 new repeatable workflow (choose from remaining use cases) + update portfolio.
- [ ] **Tuesday**: Build 1 new repeatable workflow (choose from remaining use cases) + update portfolio.
- [ ] **Wednesday**: Build 1 new repeatable workflow (choose from remaining use cases) + update portfolio.
- [ ] **Thursday**: Build 1 new repeatable workflow (choose from remaining use cases) + update portfolio.
- [ ] **Friday**: Build 1 new repeatable workflow (choose from remaining use cases) + post 1 workflow demo on X/LinkedIn. Apply to 5 higher-rate gigs per week ($1k–$5k).

### Final 5 days (Week 24)
- [ ] **Monday**: Full portfolio review. Reach out to past clients for testimonials. Set up recurring monthly support packages.
- [ ] **Tuesday**: Full portfolio review. Reach out to past clients for testimonials. Set up recurring monthly support packages.
- [ ] **Wednesday**: Full portfolio review. Reach out to past clients for testimonials. Set up recurring monthly support packages.
- [ ] **Thursday**: Full portfolio review. Reach out to past clients for testimonials. Set up recurring monthly support packages.
- [ ] **Friday**: **Core Month 6 Milestone** — 5+ paid clients or equivalent income, full production-ready portfolio, ready to be hired as AI Automation Builder.

**Developer Path Add-on (Month 6)**  
- [ ] Build one fully custom backend (FastAPI + LangGraph) for a complex client use case.  
- [ ] Add advanced monitoring, rate-limit handling, and cost tracking in Python.  
- [ ] **Dev Month 6 Milestone** — You can now take on $5k–$20k+ contracts that require custom code + n8n hybrid solutions.

---

**Maintenance after Month 6**  
- [ ] Every Monday: 1 hour reviewing new n8n templates **or** LangGraph updates.  
- [ ] Every Friday: Post 1 workflow or client win.

You now have the **complete technical path** — same speed to first client as the non-technical route, but with Python, LangGraph, and custom backends that open bigger doors.  

Open this file every workday, check the boxes, and you’ll finish as a fully hireable AI Automation Builder who can ship both no-code **and** code-heavy solutions.  

You’ve got this. Start Monday and watch the checks fill up! 🚀