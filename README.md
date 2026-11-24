## Hey, I'm Abhilash

I build AI agents, the evals that prove they work, and the backend that keeps them running. Every project I ship has a held-out benchmark, ablations and a per-query cost behind it.
Right now I'm turning my enterprise search work into **[OrgBrain](https://github.com/abhilashHQ/enterprise-search-rag)**, an open-source company brain you can self-host.

[**abhilash24.me**](https://abhilash24.me) · [Blog](https://abhilash24.me/blog) · [LinkedIn](https://www.linkedin.com/in/abhilashreddymanda) · [abhilashreddy2429@gmail.com](mailto:abhilashreddy2429@gmail.com)

---

### Building now: OrgBrain

Plug in your company's docs and Slack, bring any AI subscription or API key, and get a teammate that answers from company knowledge with citations, says so when the answer isn't there, and remembers what the team tells it. It runs as a web app, a Slack bot and an MCP server.

It grew out of a retrieval pipeline I built against [EnterpriseRAG-Bench](https://huggingface.co/datasets/onyx-dot-app/EnterpriseRAG-Bench): 512K documents across Slack, email, tickets and docs.

**67.9 vs 47.7 for BM25 on a held-out split I ran once (+20.1, 95% CI +15.7 to +24.5) · Recall@10 82.2 · $0.0028 per question**

<a href="https://github.com/abhilashHQ/enterprise-search-rag"><img src="https://raw.githubusercontent.com/abhilashHQ/enterprise-search-rag/main/web/docs/video/qst_0421.gif" alt="Enterprise Search answering a question with cited sources and a reranked evidence panel" width="720"></a>

[Repo](https://github.com/abhilashHQ/enterprise-search-rag) · [Results and ablations](https://github.com/abhilashHQ/enterprise-search-rag#results)

---

### What I've built

| Project | What it is |
|---|---|
| [**CookCode**](https://github.com/abhilashHQ/CookCode) | A coding agent harness I built from scratch around a replayable event log. Every request the model saw can be rebuilt byte for byte, and runs can be resumed, forked and replayed. 0.80 on a Terminal-Bench 2.0 slice vs 0.76 for Terminus 2, 1,120 tests, 54 written design decisions. |
| [**Macky**](https://github.com/abhilashHQ/Macky) | A voice assistant in the Mac notch. Hold a key, say what you want, and it acts across Slack, Gmail, Spotify and your calendar, handing long jobs to background agents. Swift + GPT Realtime + MCP. ([site](https://heymacky.vercel.app), [demo](https://youtu.be/SIRyFt7ISx0)) |
| [**minimi memory harness**](https://github.com/abhilashHQ/minimi-context) | Memory layer that keeps one current version of a fact across WhatsApp, email and calendar. 22/24 correct vs 14/24, reading a quarter of the tokens. |
| [**DeepRead**](https://github.com/abhilashHQ/DeepRead) | Drop in an ML paper, get a plan for implementing it. The Q&A agent checks its own citations and rewrites answers that don't hold up. ([live](https://deep-read-seven.vercel.app)) |
| [**M-RAG**](https://github.com/abhilashHQ/Multimodal-Rag) | RAG over hardware datasheets that reads the figures and tables too. 61.5% on those questions, where text-only got none. |
| [**geo-measure-api**](https://github.com/abhilashHQ/geo-measure-api) | Upload a Shapefile or KML and get accurate per-feature area and length. FastAPI, GDAL, pyproj. |
| [**Anon-chat**](https://github.com/abhilashHQ/Anon-chat) | Anonymous chat on stateless Node.js WebSockets, handles 1,000+ concurrent connections. |

### Open source

| PR | What it does |
|---|---|
| [pipecat-ai/pipecat#6024](https://github.com/pipecat-ai/pipecat/pull/6024) | Keeps the OpenAI Realtime receive loop alive and reports connections that died |
| [kornia/kornia#5361](https://github.com/kornia/kornia/pull/5361) | Fixes `isinstance` checks in augmentation containers so they compile on torch 2.5.1 |

**Usually writing:** Python · TypeScript · Swift, plus FastAPI, Postgres, Redis, Qdrant, Docker and AWS.

---

### Latest writing

<!-- BLOG-POST-LIST:START -->
- [Oversight Arena: Training an LLM to Catch the AI Failures That Look Like Successes](https://abhilash24.me/blog/blog-post)
- [You Stopped Thinking, Robert. You&#39;re a Prompster Now](https://abhilash24.me/blog/you-stopped-thinking-robert)
<!-- BLOG-POST-LIST:END -->

More at [abhilash24.me/blog](https://abhilash24.me/blog)

---

### Hackathon builds

| Project | What it is |
|---|---|
| [**Oversight Arena**](https://github.com/abhilashHQ/overSight_Arena) | RL environment where one model supervises five coding agents and learns to catch failures that look like successes. Trained Qwen2.5-3B with GRPO. ([writeup](https://abhilash24.me/blog/blog-post)) |
| [**GitMergeEnv**](https://github.com/abhilashHQ/GitMergeEnv) | RL environment that trains agents to resolve git merge conflicts with whole-file consistency. |
| [**AfterCare**](https://github.com/abhilashHQ/afterCare) | Photograph an Indian hospital discharge summary, get a picture-and-voice medicine schedule in your language. AWS Lambda, Textract, Bedrock. ([live](https://main.d2nozesb14q5me.amplifyapp.com)) |
| [**Intelli-Credit**](https://github.com/abhilashHQ/Intelli-Credit) | Corporate credit appraisal engine for Indian lending workflows. |

Winner, [TCS AI Hackathon](https://drive.google.com/file/d/10CNecnstq9_I7sGFySNo0rsbjeyZCStA/view) (Jul 2026) · Grand Finalist, [Meta x PyTorch x OpenEnv](https://drive.google.com/file/d/1WuTUidWNzSoFeN349NXxyhVj-Tt4AKbd/view) (May 2026, top 0.1% of 52,000+) · Finalist, [IIT Hyderabad Innovation Hackathon](https://drive.google.com/file/d/12bqjwjR-m-M1cy7cO535n9wDSOPxa5L8/view) (Mar 2026)

---

Open to full-time remote roles in applied AI and backend engineering. If you're building agents, search or eval infra, [email me](mailto:abhilashreddy2429@gmail.com).
