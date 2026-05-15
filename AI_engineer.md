# AI Engineer 6-Month Roadmap To-Do List

**Created from:** @DeRonin_ X thread (6-month practical AI engineering roadmap)  
**Start date:** Monday, May 18, 2026  
**Goal:** Become a job-ready AI Engineer who can build real LLM-powered applications, RAG systems, agents, and production workflows.  
**How to use this file:**
- Copy-paste into a file called `ai-engineer-roadmap-todo.md`
- Open in any Markdown editor (VS Code, Obsidian, Notion, Typora, etc.)
- Check off tasks with `[x]` as you complete them
- One long sequential to-do list, split into weekly chunks (4 weeks ≈ 1 month)
- Every week includes study tasks, resources, and practice projects exactly as outlined in the thread
- Track your own progress — the milestone at the end of each month is the big checkbox

---

## Week 1 (May 18 – 24, 2026) – Month 1: Python Fundamentals (Part 1)

- [ ] Complete **Python for Everybody** (Coursera) – Units 1-3 OR **freeCodeCamp Python Course** (YouTube) sections on basics
- [ ] Master: variables, data types, loops, conditionals, functions
- [ ] Master: lists, dictionaries, sets, tuples
- [ ] Practice daily coding in a Jupyter notebook or .py file (no passive watching)
- [ ] Set up virtual environments (`venv`) and `pip` package management
- [ ] Build practice project: Simple CLI personal expense tracker (reads/writes JSON file)
- [ ] Push the project to a new GitHub repo (even if tiny)

## Week 2 (May 25 – 31, 2026) – Month 1: Python + Git + Terminal

- [ ] Finish **Python for Everybody** / freeCodeCamp (remaining units) OR **CS50P** problem sets
- [ ] Master: File I/O, JSON handling, classes & basic OOP, error handling (`try/except`)
- [ ] Complete **GitHub Skills** interactive courses
- [ ] Complete **Learn Git Branching** (interactive)
- [ ] Master: `git init`, `add`, `commit`, `push`, `pull`, branching, merging, `.gitignore`, READMEs
- [ ] Complete terminal basics: **50 most popular Linux commands** video OR **Missing Semester of CS** (MIT)
- [ ] Master navigation (`cd`, `ls`, `pwd`, `mkdir`, `rm`), `cat`, `grep`, running Python scripts, environment variables
- [ ] Every new script from now on must live in its own GitHub repo

## Week 3 (Jun 1 – 7, 2026) – Month 1: APIs, HTTP, Async + SQL/Pandas

- [ ] Study HTTP basics (MDN Web Docs) + REST API Tutorial
- [ ] Master Python `requests` library + JSON handling
- [ ] Learn Python `async/await` (RealPython article)
- [ ] Build practice project: Python script that calls a free public API (Open-Meteo weather) and outputs clean JSON
- [ ] Complete **SQLBolt** (all 20 interactive lessons)
- [ ] Complete **10 Minutes to Pandas** (official) + Kaggle Pandas course
- [ ] Master: SQL `SELECT`, `WHERE`, `GROUP BY`, `JOIN`, `ORDER BY`; Pandas loading CSVs, filtering, aggregations

## Week 4 (Jun 8 – 14, 2026) – Month 1: FastAPI + Milestone

- [ ] Complete **FastAPI Official Tutorial** (start to finish)
- [ ] Watch **Python API Development** freeCodeCamp 19-hour course (focus on routes, Pydantic, uvicorn, /docs)
- [ ] Build and run a simple FastAPI app locally with GET/POST endpoints
- [ ] **Month 1 Milestone** – Check when you can:
  - [ ] Write Python programs that read/write files, call APIs, handle errors
  - [ ] Version code with Git and push to GitHub
  - [ ] Navigate terminal comfortably
  - [ ] Make HTTP requests in Python
  - [ ] Query SQLite with basic SQL
  - [ ] Build & run a FastAPI app

**Month 1 Complete** – You now have a solid coding foundation.

---

## Week 5 (Jun 15 – 21, 2026) – Month 2: Prompting Fundamentals

- [ ] Complete **Anthropic Interactive Prompt Engineering Tutorial** (all 9 chapters, run notebooks with Claude API)
- [ ] Read **Anthropic Prompt Engineering Docs** + **OpenAI Prompt Engineering Guide**
- [ ] Read **PromptingGuide.ai** (focus on core techniques)
- [ ] Focus: system vs user messages, specificity, chain-of-thought, few-shot prompting
- [ ] Practice: Write 5 different prompts for the same task (summarize, extract, classify) and compare outputs

## Week 6 (Jun 22 – 28, 2026) – Month 2: Structured Outputs + Tool Calling

- [ ] Complete **OpenAI Structured Outputs Guide** + **Instructor library** tutorial
- [ ] Build practice project: Invoice/receipt parser (raw text → structured Pydantic object)
- [ ] Complete **OpenAI Function Calling Guide** + **Anthropic Tool Use Docs**
- [ ] Complete OpenAI Cookbook notebook on function calling
- [ ] Build practice project: Simple assistant with 3 tools (get_weather, calculate, search_notes)

## Week 7 (Jun 29 – Jul 5, 2026) – Month 2: Streaming + Conversation State + Cost/Latency

- [ ] Study **OpenAI Streaming** + **Anthropic Streaming** docs
- [ ] Implement streaming in a FastAPI endpoint (`StreamingResponse`)
- [ ] Study **OpenAI Conversation State** guide + **Anthropic Messages API**
- [ ] Build practice project: Multi-turn terminal chatbot (maintain messages list, /reset command, token counting)
- [ ] Study OpenAI & Anthropic pricing pages + tokenizer tool + tiktoken library

## Week 8 (Jul 6 – 12, 2026) – Month 2: Failure Handling + Prompt Injection + Milestone

- [ ] Study error codes (OpenAI + Anthropic) + Tenacity retry library
- [ ] Implement retries, timeouts, fallbacks, validation
- [ ] Study **OWASP Top 10 LLM01: Prompt Injection** + prevention cheat sheet
- [ ] **Month 2 Milestone** – Check when you can:
  - [ ] Write reliable prompts
  - [ ] Get structured JSON with Pydantic + Instructor
  - [ ] Wire tool calling
  - [ ] Stream responses in FastAPI
  - [ ] Manage conversation history
  - [ ] Estimate token costs
  - [ ] Handle errors & prompt injection

**Month 2 Complete** – Core LLM app skills unlocked.

---

## Week 9 (Jul 13 – 19, 2026) – Month 3: Embeddings + Chunking

- [ ] Read Stack Overflow “Intuitive Introduction to Text Embeddings” + Google ML Crash Course + HuggingFace + OpenAI Embeddings Guide
- [ ] Practice: Embed 20 sentences and build nearest-neighbor search
- [ ] Study **Weaviate Chunking Strategies** + **Unstructured** + LangChain Text Splitters
- [ ] Experiment with RecursiveCharacterTextSplitter (500 tokens, 50 overlap)

## Week 10 (Jul 20 – 26, 2026) – Month 3: Vector Databases + Metadata Filtering + Reranking

- [ ] Complete **Chroma** docs (local) + **Pinecone** tutorials + **Qdrant** or **pgvector** if preferred
- [ ] Practice project: Index 50–100 pages of documentation into Chroma with metadata
- [ ] Study metadata filtering (Pinecone + LlamaIndex guides)
- [ ] Study **Cohere Reranking** + LangChain integration

## Week 11 (Jul 27 – Aug 2, 2026) – Month 3: Retrieval Quality + Hallucination Reduction + Citations

- [ ] Study LangChain Query Transformations + Pinecone “Improving Retrieval Quality”
- [ ] Study hallucination reduction guides (Zep + Voiceflow)
- [ ] Study Anthropic “Giving Claude Sources” + LangChain RAG with sources
- [ ] Continue building your RAG pipeline

## Week 12 (Aug 3 – 9, 2026) – Month 3: Full RAG Pipeline + Milestone

- [ ] Choose framework: **LlamaIndex** (recommended for RAG) or LangChain
- [ ] Build end-to-end “Chat with your docs” FastAPI app:
  - Ingest 10–20 PDFs/text files
  - Chunk + embed + store with metadata
  - Retrieve top-5 with reranking
  - Return grounded, cited answer
- [ ] **Month 3 Milestone** – Check when you can:
  - [ ] Explain embeddings & cosine similarity
  - [ ] Chunk documents intelligently
  - [ ] Store/query vector DB with filters
  - [ ] Add reranking
  - [ ] Debug retrieval failures
  - [ ] Build complete cited RAG system

**Month 3 Complete** – You can now ground LLMs in your own data.

---

## Week 13 (Aug 10 – 16, 2026) – Month 4: Agent Loops + Tool Selection

- [ ] Read **Anthropic “Building Effective Agents”** + OpenAI Practical Guide to Agents
- [ ] Study LangGraph (LangChain Academy course) or build agent from scratch (no framework)
- [ ] Practice: Build a 3-tool agent loop using only OpenAI/Anthropic API (perceive → plan → act → observe)
- [ ] Study OpenAI & Anthropic tool definition best practices (be extremely explicit)

## Week 14 (Aug 17 – 23, 2026) – Month 4: Advanced Agents, Workflows & Evals (continued from thread)

- [ ] Continue agent loop practice and add memory, human-in-the-loop, planning
- [ ] Study multi-step workflows and conditional chains
- [ ] Begin implementing evaluation metrics for your agents (accuracy, cost, latency, success rate)

*(Note: The original thread continues into advanced agent patterns, evals, production deployment, and final portfolio projects for Months 5–6. Continue the same pattern of weekly study + practice projects for the remaining months. Update this file with the rest of the thread as you progress or let me know if you want Weeks 15–26 pre-filled once you reach Month 4 end.)*

## Remaining Weeks (15–26) – Months 4–6

- Weeks 15–16: Finish Month 4 (Agents, evals, production patterns)
- Weeks 17–20: Month 5 (Production deployment, observability, scaling, advanced integrations)
- Weeks 21–24: Month 6 (Capstone projects, portfolio, job-ready systems)
- Weeks 25–26: Polish, deploy 3–5 full-stack AI apps, prepare for real-world use / job applications

**Final 6-Month Milestone** (by ~November 2026):
- You can independently build, deploy, and maintain production LLM applications, RAG systems, and autonomous agents.
- You have a public GitHub portfolio of 5+ real projects.
- You are ready to contribute as an AI Engineer.

---

**Pro Tips from the thread:**
- Code every single example — never just watch.
- Every project goes into GitHub immediately.
- Build real things people can use (not just notebooks).
- Track costs and latency from day 1.
- Focus on practical execution over theory.

You’ve got the complete roadmap. Now ship every week.  
Start today — May 18, 2026 is Week 1.

Good luck! In 6 months you’ll be building real AI products.