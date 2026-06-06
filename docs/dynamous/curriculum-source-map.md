# Dynamous / Cole Curriculum Source Map

Built from local scrape: `/tmp/dynamous_scrape/priority_pages`  
Inventory: `/tmp/dynamous_scrape/priority_pages/inventory.csv`  
Coverage verified: 246 scraped pages, 246 saved, 0 scrape errors.

## 1. Executive take

The right path is not “watch everything in order.”

The useful path for Son is:

```text
Agentic Coding system fundamentals
→ PIV loop + commands + validation
→ remote/GitHub workflow
→ MCP / skills / subagents / worktrees
→ AI Agent Mastery production stack
→ AI Second Brain memory/security layer
→ Archon only after the local system is understood
```

The core progression Cole teaches is:

```text
System gap
→ PIV loop
→ context layer
→ commands
→ planning system
→ execution
→ validation
→ GitHub / remote coding
→ MCP / skills
→ subagents / parallel work
→ agents / RAG / apps
→ second brain / ops / security
```

The practical goal should be a working operating system, not course completion.

## 2. Source map

### 2.1 Primary course blocks

#### Agentic Coding Course — files 001-072

Role: the operating system for using AI coding assistants.

Primary resources found:

- Course repo: `https://github.com/dynamous-community/agentic-coding-course`
- Commands from Modules 4-7: `https://github.com/dynamous-community/agentic-coding-course/tree/main/.agents/commands`
- Main project: Obsidian AI Agent: `https://github.com/dynamous-community/obsidian-ai-agent`
- Remote coding system: `https://github.com/dynamous-community/remote-coding-agent`
- Help category: `https://community.dynamous.ai/c/agentic-coding/`

Best use:

- Build the repeatable coding workflow.
- Learn PIV loop discipline.
- Build reusable commands.
- Add validation before scaling to remote agents or Archon.

#### AI Agent Mastery Course — files 073-134

Role: production-shaped AI agent/app curriculum.

Progression:

```text
n8n prototype
→ RAG prototype
→ Python / Pydantic AI agent
→ API endpoint
→ frontend / auth / upload / rate limits
→ deployment
→ multi-agent architecture
→ evals
→ monetization
```

Best use:

- Convert the agentic coding workflow into real apps and automations.
- Learn n8n, RAG, Pydantic AI, FastAPI, deployment, observability, evals, and monetization.

#### AI Second Brain Course — files 135-142

Role: personal memory / operating layer.

Progression:

```text
Second Brain architecture
→ PRD
→ memory layer
→ hooks + memory search
→ integrations + skills
→ reflection / heartbeat / chat interface
→ security hardening
```

Best use:

- Build durable memory and personal context.
- Add hooks, skills, reflection, chat interface, and security.
- Useful, but dangerous if added too early because memory/context can become expensive and bloated.

#### Cole Collections — files 143-146

Role: resource layer.

Contains:

- Past workshops.
- Templates and resources.
- Cole’s AI development tech stack.
- Favorite MCP servers.

Best use:

- Reference material while implementing.
- Do not start here. Use it when a curriculum phase asks for a concrete tool/template.

### 2.2 Community discussion blocks

#### Agentic Coding Discussion — files 147-171

Main signals:

- Git worktrees + PIV loops need merge discipline.
- `/prime` can overfill context if too broad.
- `AGENTS.md` / `CLAUDE.md` should stay short.
- GitHub access causes many 404s unless Dynamous access is granted.
- Archon should usually come after Module 7.

#### Archon Discussion — files 172-196

Main signals:

- Old Archon lesson and new Archon are not identical.
- Archon is currently strongest as a build-time coding harness, not as a production runtime.
- Worktree resets can wipe local state if not committed/pushed.
- Claude permission rules do not automatically map to Archon autonomous workers.
- Docker persistence and `$ARCHON_HOME` need care.

#### AI Second Brain Discussion — files 197-221

Main signals:

- Second Brain should not automatically become context for every repo.
- Multi-repo work should usually happen inside each repo, unless Archon is intentionally orchestrating target repos.
- Shared memory/wiki layer is useful, but ownership and anti-rot rules matter.
- Security hooks can cause Claude to fight restrictions unless global rules are explicit.
- Token/cost blowups are real if memory/logs are replayed into every prompt.

#### AI Mastery Discussion — files 222-246

Main signals:

- n8n and local AI lessons drift as tools change.
- Local Docker URLs vs localhost URLs are common failure points.
- Embedding dimension mismatch breaks RAG.
- Pydantic AI remains relevant for production-shaped agents.
- Claude Agent SDK is good for personal apps, slower/costlier at scale.
- OpenRouter/Bifrost/key spend limits matter for guardrails.

## 3. Recommended curriculum for Son

Assumption: the goal is to ship a useful personal/business operating system with Hermes/Telegram/GitHub/Obsidian-style workflows, not just finish videos.

### Phase 0 — Setup and access

Use sources:

- `002-all-resources-for-the-course.txt`
- GitHub access threads: `154`, `157`, `171`, `214`, `216`, `235`, `236`

Do:

- Confirm Dynamous GitHub access.
- Clone/access:
  - Agentic Coding Course repo.
  - Obsidian AI Agent repo.
  - Remote Coding Agent repo.
  - AI Agent Mastery repo/materials.
- Install/check:
  - `uv`
  - Python 3.10+
  - Node/npm
  - Docker
  - GitHub CLI or normal Git workflow
  - Claude Code / Codex / chosen coding assistant

Friday artifact:

- `setup-check.md`
- `repo-access-check.md`
- one clean local project folder with course repos and notes.

Success check:

- No private GitHub link returns 404.
- You can run at least one repo’s setup command.

### Phase 1 — Baseline and System Gap

Use sources:

- Agentic Coding `001-007`

Do:

- Watch/read Module 1.
- Run the first exercise with your normal AI workflow.
- Do not optimize yet.
- Record what breaks:
  - vague prompts?
  - too much manual correction?
  - bad code review?
  - no validation?
  - context confusion?

Friday artifact:

- `baseline-ai-coding-retro.md`

Template:

```md
# Baseline AI Coding Retro

Task:
Assistant used:
Time spent:
What worked:
What failed:
Where I lost control:
Validation done:
What I would systematize:
```

Success check:

- You have a real before/after baseline for later comparison.

### Phase 2 — PIV Loop foundation

Use sources:

- Agentic Coding `008-014`
- Workshop `014-live-workshop-1...`

Do:

- Learn and apply PIV:

```text
Plan → Implement → Validate → Iterate
```

- Re-run the same or similar task using PIV.
- Create a structured plan before implementation.
- Commit before/after.
- Compare result against Phase 1.

Friday artifact:

- `piv-loop-template.md`
- one completed PIV loop with commit history.

Success check:

- You can point to the plan, implementation, validation notes, and iteration notes.

### Phase 3 — Context layer: rules and references

Use sources:

- Agentic Coding `015-019`
- Community threads:
  - `150-real-time-tunnel-navigation.txt`
  - `159-is-prime-supposed-to-use-50-of-your-context-window...txt`
  - `165-evaluating-agents-md-research-study...txt`

Do:

- Build a small always-loaded rule file.
- Move detailed docs into references.
- Keep global rules short.

Practical rule:

```text
Global rules: short, stable, always true.
References: long, task-specific, loaded only when needed.
Commands: workflows, not principles.
```

Friday artifact:

- `AGENTS.md` or `CLAUDE.md`, under 150 lines if possible.
- `/docs/ai-context/` folder with reference docs.

Success check:

- `/prime` or equivalent does not consume half the context window.
- The agent can find references without loading everything every time.

### Phase 4 — Commands and reusable workflows

Use sources:

- Agentic Coding `020-025`
- Thread `160-adding-skills-or-a-skill-finder-skill...txt`

Do:

- Build commands around IPO:

```text
Input → Process → Output
```

Start with:

- `/prime`
- `/plan-feature`
- `/execute`
- `/validate`
- `/code-review`
- `/system-review`

Do not create 50 commands. Build only the core loop.

Friday artifact:

- `.agents/commands/` or equivalent command folder.
- `command-contract.md` describing command inputs/outputs.

Success check:

- A command output can feed the next command without explanation.

### Phase 5 — Planning system and Obsidian Agent project

Use sources:

- Agentic Coding `026-033`
- Obsidian Agent repo/materials.

Do:

- Build the PRD.
- Start from an AI-optimized template.
- Run PIV loop #1 for the base app.
- Run PIV loop #2 to connect to Obsidian or a local note vault.

Artifacts:

- `prd.md`
- `structured-plan-template.md`
- `copilot-plugin-analysis.md` if using Obsidian Copilot.
- `pydantic-ai-streaming-notes.md` if using streaming.

Friday artifact:

- A minimal Obsidian/local-vault agent that can read/search notes.

Success check:

- Agent can answer from a local vault/file source with cited file references.

### Phase 6 — Execution and validation system

Use sources:

- Agentic Coding `034-042`
- Community thread `163-project-hygiene-during-piv-loops...txt`

Do:

- Implement `/execute`.
- Implement validation pyramid:

```text
lint/format
→ type checks
→ unit tests
→ integration tests
→ human review
```

- Add project hygiene review:
  - README
  - CHANGELOG
  - dependency files
  - `.gitignore`
  - `.dockerignore`
  - docs
  - tests

Friday artifact:

- `/validate`
- `/code-review`
- `/system-review`
- `project-hygiene-checklist.md`

Success check:

- The agent cannot call work “done” without validation evidence.

### Phase 7 — GitHub and remote coding

Use sources:

- Agentic Coding `043-054`
- Remote coding system repo.
- Community thread `166-logging-claude-code-session-ids...txt`

Do:

- Move workflow into GitHub Issues/PRs.
- Add issue-triggered or PR-triggered agentic workflows.
- Add release note generation.
- Add session continuity:
  - commit body references issue/session/progress doc.

Friday artifact:

- One issue → PR → review → merge workflow.
- `progress.md` or equivalent session continuity convention.

Success check:

- You can restart from issue + branch + progress file without relying on memory.

### Phase 8 — MCP, skills, and selective tool loading

Use sources:

- Agentic Coding `055-059`
- Cole Collection `146-my-favorite-mcp-servers.txt`
- Thread `160-adding-skills-or-a-skill-finder-skill...txt`

Do:

- Add only useful MCPs/tools.
- Avoid giant always-loaded tool lists.
- Consider a tool-search/RAG layer when tool count grows.

Useful targets:

- GitHub
- filesystem/search
- browser/Playwright
- database/Supabase/Postgres
- documentation retrieval
- Obsidian/local notes

Friday artifact:

- `tools-registry.md`
- one custom skill/SOP package.

Success check:

- The agent chooses the right tool without seeing 20+ irrelevant tools in prompt.

### Phase 9 — Subagents and parallel work

Use sources:

- Agentic Coding `060-068`
- Thread `151-git-worktrees-piv-loops...txt`

Do:

- Use subagents first for research/review, not autonomous implementation.
- Add worktrees only after validation is reliable.
- Use PRs as the clean merge/review gate.

Important rule:

```text
Agents can update tests and code, but should not rewrite the human acceptance spec without approval.
```

Friday artifact:

- `system-review-agent.md`
- `worktree-parallelization-sop.md`

Success check:

- Two independent changes can be reviewed/merged without losing acceptance intent.

### Phase 10 — AI Agent Mastery: production app path

Use sources:

- AI Agent Mastery `073-134`
- Local setup/debug threads `224`, `229`, `231`, `234`, `244`, `245`

Do:

Build in this order:

```text
n8n prototype
→ RAG prototype
→ Pydantic AI agent
→ FastAPI endpoint
→ frontend
→ auth / rate limit / upload
→ deploy
→ observability
→ evals
```

Common traps:

- n8n version drift.
- Docker service URL vs localhost URL mismatch.
- Embedding dimension mismatch.
- local model tool-calling weakness.
- file trigger disabled in newer n8n.

Friday artifact:

- One deployed small agent endpoint with logs and basic evals.

Success check:

- Agent works outside local notebook/terminal.
- There is a visible API or UI.
- You have at least one eval or regression test.

### Phase 11 — Second Brain and memory layer

Use sources:

- AI Second Brain `135-142`
- Community threads:
  - `197-ai-second-brain-category.txt`
  - `204-second-brain-where-to-start-from.txt`
  - `206-second-brain-vault-sync.txt`
  - `209-how-does-cole-work-across-multiple-repos...txt`
  - `217-second-brain-for-multiple-codebases...txt`
  - `218-claude-code-trying-to-bypass-block-secrets-py.txt`

Do:

- Build memory only after commands/validation are stable.
- Keep memory layer separate from project repos.
- Each repo should own its local rules/context.
- Shared Second Brain can be referenced, but should not blindly become context for every project.

Memory architecture recommendation:

```text
Hard facts / records → deterministic database or files
Soft preferences → memory layer
Project conventions → repo-local docs
Cross-project knowledge → shared wiki/Second Brain
```

Friday artifact:

- `memory-policy.md`
- local note/vault sync SOP
- security hook checklist

Success check:

- Memory improves continuity without replaying large logs into every prompt.

### Phase 12 — Archon, production runtime, and guardrails

Use sources:

- Archon lesson `058`
- Archon discussions `172-196`
- Cost/security threads `183`, `185`, `188`, `190`, `195`, `205`, `215`, `227`

Do:

- Use Archon after Module 7, not at the beginning.
- Use it for build-time agentic coding/workflow orchestration.
- Do not assume it is the right runtime for customer-facing long-running production workflows.

Guardrails to add:

- Spend limits on API keys or OpenRouter keys.
- Token usage dashboard or logs.
- Lazy-load memory.
- Budget killswitch.
- Stuck-loop detection.
- Human approval gates.
- Explicit commit/push points before Archon resets/worktree operations.

Friday artifact:

- `archon-readiness-checklist.md`
- `llm-spend-guardrails.md`
- `security-permissions-model.md`

Success check:

- You can explain what Archon owns, what Git owns, what the filesystem owns, and what production runtime owns.

## 4. Priority watchlist / failure-mode index

### Context and cost

- `159`: `/prime` can consume too much context.
- `165`: large `AGENTS.md` / `CLAUDE.md` hurts performance.
- `215`: memory/log replay caused $30 cost regression and near argv-size brick.
- `205`: track token usage by project/session/tool/subagent.
- `227`: set spend limits and model routing rules.

Action:

- Keep always-loaded context small.
- Lazy-load details.
- Add usage tracking before daily use.

### Git and worktrees

- `151`: worktrees need PR/review/acceptance gates.
- `188`: Archon source reset can wipe local state.
- `166`: session IDs/progress docs help resume workflows.

Action:

- Commit early.
- Use PRs for merge gates.
- Keep `progress.md`.

### Security

- `197`: YOLO mode needs hook protection.
- `218`: Claude may try to inspect/bypass secret-blocking hooks.
- `183`: Claude deny rules do not automatically apply to Archon workers.

Action:

- Use explicit global rules: do not bypass security hooks.
- Keep secrets out of repo and prompt.
- Use runtime injection and human approval for sensitive actions.

### Local AI / n8n / RAG

- `231`: n8n version drift and sub-workflow changes.
- `234`: `localhost` vs Docker service URLs.
- `229`: embedding dimensions must match vector DB schema.
- `244`: local file trigger disabled in n8n v2.

Action:

- Verify versions.
- Document URLs per runtime.
- Pin embedding model dimensions.

### Tool/provider compatibility

- `203`: Second Brain repo is Claude-specific but can be converted to Codex conventions.
- `226`: Claude Agent SDK is useful for personal apps; Pydantic AI still matters for production.
- `191`: Context7/OpenRouter reliability may vary; cloud VM may be more stable.

Action:

- Keep conventions portable:
  - `.claude/` for Claude.
  - `AGENTS.md` for Codex/general agents.
  - repo-local docs for model-agnostic context.

## 5. Practical build order for Son

If time is limited, do only this sequence:

1. **Weeks 1-2:** PIV loop + concise context layer.
2. **Weeks 3-4:** core commands: `/prime`, `/plan-feature`, `/execute`, `/validate`, `/code-review`, `/system-review`.
3. **Weeks 5-6:** Obsidian/local-vault agent with validation.
4. **Weeks 7-8:** GitHub Issue → PR workflow.
5. **Weeks 9-10:** Pydantic AI / FastAPI endpoint + basic evals.
6. **Weeks 11-12:** Second Brain memory layer + cost/security guardrails.
7. **Only then:** Archon/worktrees/parallel agents.

Do not start with Archon, Second Brain, and full remote coding at the same time. That stacks too many moving parts.

## 6. Build artifacts checklist

By the end, the useful deliverables are:

- `setup-check.md`
- `baseline-ai-coding-retro.md`
- `piv-loop-template.md`
- `AGENTS.md` / `CLAUDE.md`
- `/docs/ai-context/*`
- `.agents/commands/*`
- `prd.md`
- `/validate`
- `/code-review`
- `/system-review`
- `project-hygiene-checklist.md`
- `progress.md`
- `tools-registry.md`
- one custom skill/SOP package
- `system-review-agent.md`
- `worktree-parallelization-sop.md`
- one deployed agent endpoint
- `memory-policy.md`
- `llm-spend-guardrails.md`
- `security-permissions-model.md`
- `archon-readiness-checklist.md`

## 7. Index files generated locally

- Raw scrape folder: `/tmp/dynamous_scrape/priority_pages`
- Manifest: `/tmp/dynamous_scrape/priority_pages/manifest.json`
- Inventory CSV: `/tmp/dynamous_scrape/priority_pages/inventory.csv`
- Raw scrape archive: `/tmp/dynamous_priority_pages_246.tar.gz`
- This curriculum index: `/tmp/dynamous_curriculum_index.md`
