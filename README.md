# Hi, I'm Alejandro Quirós 👋

**IT Engineer at Taco Bell Costa Rica & Panama** · I design and ship production data platforms and AI agents, end to end: from data pipelines and data lakes to LLM evaluation, CI/CD and the web app people actually use.

📍 Costa Rica · 🎓 Finishing a B.Sc. in Information Technology at Universidad Invenio

---

## Featured work

> My professional work lives in private repositories, so only a technical overview is shared here.

### 🤖 Conversational BI agent
Designed and built end to end by me. Natural-language analytics over sales, loyalty and invoices, served in Microsoft Teams and a web portal, returning figures, tables, charts and Excel files.

**Built in-house (no agent framework):**
- **Agent loop** written from scratch (no LangChain / LangGraph): an orchestrator model routes and writes, sub-agents run in-process, bounded iterations
- **Structured metric tool:** the model never writes SQL for core metrics; it emits a typed request (metric · dimensions · time · filters) that resolves through the semantic layer with hard, per-user scoping
- **Guarded ad-hoc querying** for sub-agents: read-only, with access filters enforced in code
- **Personal-data access** gated by an explicit purpose-confirmation flow
- **Anti-hallucination guards** on money figures, counts and answers given without a tool call
- **Server-enforced outputs:** exports re-run the query under the user's scope and the server, not the LLM, inserts file links
- **Two-tier memory** (semantic + episodic) with per-domain few-shot retrieval
- **LLM provider abstraction** with a standby model for rollback
- **Replay harness** that re-runs real user questions against raw data · ~760 tests

**Stack:** Python · FastAPI · SSE · Azure OpenAI (GPT-4.1 + mini sub-agents, embeddings) · **Cube** semantic layer + Cube Store pre-aggregations · Amazon Athena on S3 · PostgreSQL + pgvector · Redis · Docker · GitHub Actions

---

## 🌱 Open source

| Project | Contribution | Status |
|:--|:--|:--:|
| <a href="https://github.com/Gentleman-Programming/gentle-shell"><img src="https://img.shields.io/github/stars/Gentleman-Programming/gentle-shell?style=flat-square&logo=github&label=gentle-shell&color=7aa2f7" alt="gentle-shell"></a> | Diagnosed and reproduced a crash on session switch; fixed upstream | <a href="https://github.com/Gentleman-Programming/gentle-shell/issues/3072"><img src="https://img.shields.io/github/issues/detail/state/Gentleman-Programming/gentle-shell/3072?style=flat-square" alt="#3072"></a> <a href="https://github.com/Gentleman-Programming/gentle-shell/pull/3127"><img src="https://img.shields.io/github/pulls/detail/state/Gentleman-Programming/gentle-shell/3127?style=flat-square" alt="#3127"></a> |
| <a href="https://github.com/Gentleman-Programming/gentle-ai"><img src="https://img.shields.io/github/stars/Gentleman-Programming/gentle-ai?style=flat-square&logo=github&label=gentle-ai&color=7aa2f7" alt="gentle-ai"></a> | Proposed a `doctor` improvement with an implementation plan | <a href="https://github.com/Gentleman-Programming/gentle-ai/issues/6136"><img src="https://img.shields.io/github/issues/detail/state/Gentleman-Programming/gentle-ai/6136?style=flat-square" alt="#6136"></a> |
| <a href="https://github.com/Gentleman-Programming/gentle-ai"><img src="https://img.shields.io/github/stars/Gentleman-Programming/gentle-ai?style=flat-square&logo=github&label=gentle-ai&color=7aa2f7" alt="gentle-ai"></a> | Reported a state regression in `uninstall` | <a href="https://github.com/Gentleman-Programming/gentle-ai/issues/6137"><img src="https://img.shields.io/github/issues/detail/state/Gentleman-Programming/gentle-ai/6137?style=flat-square" alt="#6137"></a> |

---

## 🛠️ Stack

**Languages:** Python · TypeScript/JavaScript · SQL · C#<br>
**Data & cloud:** AWS (Fargate, Lambda, Step Functions, S3, Athena, Glue, QuickSight) · Azure (App Service, SQL, Container Apps, OpenAI, Key Vault)<br>
**AI:** Azure OpenAI · LLM agents · MCP · Cube semantic layer · pgvector · evaluation harnesses<br>
**Web:** Flask · FastAPI<br>
**AI dev tools:** Claude Code · Codex · OpenCode · Gentle Shell (Pi) · Engram (agent memory) · MCP servers<br>
**Terminal & CLI:** PowerShell · Bash · GitHub CLI · AWS CLI · Azure CLI · Herdr<br>
**Tooling:** Docker · GitHub Actions · n8n · Git

---

## 📊 GitHub stats

<p align="center">
  <a href="https://git.io/streak-stats">
    <img src="https://streak-stats.demolab.com?user=Alequip&theme=tokyonight&hide_border=true&date_format=j%20M%5B%20Y%5D" alt="GitHub streak stats" />
  </a>
</p>

---

## 📫 Get in touch

- 📷 Instagram: [@ale_quip](https://www.instagram.com/ale_quip)
