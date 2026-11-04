## Hi, I'm Gourav 👋

I'm a Computer Science undergrad at **NIT Silchar** and a founding member of **[Nor AI Technologies](https://norai.tech)**, where I'm the AI lead and systems architect. I build AI systems that do real work: retrieval pipelines, stateful agents, and the full-stack products around them.

I also love competitive programming. I've solved 1400+ problems, I'm a **Codeforces Specialist**, and I won **Enigma 39.0**, NIT Silchar's flagship CP contest.

---

### 🏢 Nor AI Technologies

As one of the founding engineers at [norai.tech](https://norai.tech), I design the AI systems and make sure their answers follow rules a program can check. I built the company website and every free tool it ships:

| Tool | What it does |
|---|---|
| **[Grounded RAG](https://rag.norai.tech)** | Ask your documents anything. Every answer has clickable citations, and it says "not found" instead of guessing |
| **[TokenCraft](https://tokens.norai.tech)** | Token counter and cost calculator covering 94 LLMs at live rates |
| **[Judgewright](https://judge.norai.tech)** | Calibrates an LLM-as-judge against human labels using Cohen's κ, Krippendorff's α, and bootstrap CIs |
| **[SchemaCraft](https://schema.norai.tech)** | Converts JSON into OpenAI, Anthropic, Gemini, and MCP tool schemas, plus Pydantic, Zod, and TypeScript types |
| **[RegexCraft](https://regex.norai.tech)** | Regex tester with plain-English explanations, railroad diagrams, and a ReDoS watchdog |
| **[Anchorflow](https://anchor.norai.tech)** | Pins GitHub Actions to commit SHAs, audits token permissions, and flags injection sinks |
| **[Smart Rozgar](https://rozgar.norai.tech)** | Bilingual (Hindi/English) government job alerts, sorted by deadline, with eligibility checks |

All of them are free, need no sign-up, and most run entirely in your browser.

---

### 🚀 Featured projects

**[NorAI](https://github.com/GouravLuinor/NorAI)**: turn a lecture into something you can revise
Give it a lecture video, recording, PDF or slide deck. You get chapter notes with the lecturer's own slides and board work, quizzes, spaced-repetition flashcards, a mind map, and **Nora**, a tutor that answers only from that lecture and cites the second it was said.
- **98–100% of tutor citations verify** on a 66-question eval set, and out-of-scope questions are declined
- I rebuilt the 18-stage pipeline into a lean one: **29 → 9 Gemini calls**, about $0.03 for a 17-minute lecture, with unsupported claims cut from up to 19% to under 3%
- Multimodal notes written from the transcript *and* keyframes; timestamps land a **median 0.4 s** from YouTube's captions
- LangGraph tutor with hybrid BM25 + dense retrieval on a local 4-bit ONNX embedding model, so indexing uses no API quota
- SSRF-guarded fetching, fail-closed JWT and webhook verification, and one codebase that runs hosted or fully on your own PC

`FastAPI` `LangGraph` `Gemini` `React 19` `TypeScript` `ONNX Runtime` `Supabase` `Docker`

**[FocusFlow](https://github.com/GouravLuinor/focusflow)**: an adaptive execution engine for "what should I work on right now?"
Turns a vague goal into a dependency-aware task graph with Gemini, then ranks only the work that's actually unblocked. Built from the ground up for ADHD, autistic and dyslexic users.
- AI decomposition runs as an async **Celery** job. The model's output is treated as untrusted: it's schema-validated, cycle-checked (DFS) and committed atomically
- Explainable **6-factor priority engine** where every factor returns a score *and* a human-readable reason
- Adaptive duration estimates learned from measured session times, plus a validated task state machine
- Focus Mode with AI micro-steps, local **Faster-Whisper** voice entry, and ambient sound synthesized with the Web Audio API
- **147 automated tests** (111 pytest + 36 Vitest) and Playwright E2E. CI runs against real PostgreSQL 16 and Redis 7

`FastAPI` `PostgreSQL` `Redis` `Celery` `React` `TypeScript` `Gemini`

**[Personal Wellness Recommender](https://github.com/GouravLuinor/PersonalWellnessRecommender)**: a personalised, explainable wellness plan
Turns a two-minute lifestyle profile into a plan covering nutrition, movement, sleep and mindfulness, grounded in health guidelines.
- Guideline rules (Mifflin-St Jeor, WHO activity and sleep) generate 10,000 correlated synthetic profiles for training
- scikit-learn pipelines: gradient boosting for 9 numeric targets (**R² up to 0.98**) and random forests for plan types (**92–94% accuracy** vs a 32–46% baseline)
- Explains itself with a 0–100 wellness score, a per-area breakdown and permutation importance, and flags health risks such as high blood pressure
- 47 tests, including Streamlit `AppTest` end-to-end runs, with CI on every push

`scikit-learn` `pandas` `Streamlit` `Altair`

---

### 🛠️ Tech I work with

**AI / ML:** LangGraph · LangChain · ChromaDB · Gemini API · OpenAI Agents SDK · scikit-learn · Pandas · NumPy
**Backend:** Python · FastAPI · SQLAlchemy · PostgreSQL · SQLite
**Frontend:** React · TypeScript · Tailwind CSS · Streamlit
**DevOps / Cloud:** Docker · AWS (EC2, S3, Lambda, IAM) · GitHub Actions · Vercel · Render · Linux
**Languages:** C++ · C · Python · SQL · JavaScript

---

### 🏆 Competitive programming

| Platform | Achievement |
|---|---|
| [Codeforces](https://codeforces.com/profile/NorLui) | Specialist · max rating 1406 · 600+ solved |
| [LeetCode](https://leetcode.com/u/O1Nnpkej8w/) | Rating 1739 · 600+ solved |
| [CodeChef](https://www.codechef.com/users/norlui) | 2★ · max rating 1564 |

🥇 Winner, **Enigma 39.0** (NIT Silchar's flagship CP contest)
🥇 Winner, **Intelliverse**, Tecnoesis
🧩 Executive Member, **Coding Club NIT Silchar**: I run DSA workshops and write problems for contests, including CodeCauldron 4.0 (national, ICPC-style)

---

### 📫 Reach me

[LinkedIn](https://www.linkedin.com/in/gourav-kumar-singh-95257a31b) · [gauravopanime@gmail.com](mailto:gauravopanime@gmail.com) · [norai.tech](https://norai.tech)
