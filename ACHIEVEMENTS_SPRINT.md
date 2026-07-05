# GitHub Achievements Sprint — 14-Day Plan

**Account:** OlaroPeterCelestine  
**Rule:** All commits use **your name only** — run `./scripts/commit-as-me.sh "message"`  
**Honest limit:** Arctic Code Vault & Mars 2020 are **retired forever**.

---

## Your forks (AI worldwide)

You now fork high-visibility AI repos. Recruiters see activity; achievements need **merged PRs** and **real engagement**.

| Tier | Repos forked |
|------|----------------|
| LLM frameworks | langchain, llama_index, autogen, semantic-kernel |
| Models & inference | transformers, vllm, llama.cpp, ollama, peft, whisper |
| AI apps | dify, gradio, langflow, ComfyUI, AutoGPT, gpt-engineer |
| SDKs | openai-python, anthropic-sdk-python, generative-ai-python |
| Learning | LLMs-from-scratch, ChatGLM3 |

---

## Achievement checklist

| Badge | Target | How (legitimate) | ETA |
|-------|--------|------------------|-----|
| 🔫 **Quickdraw** | 1 | Open + close issue on your repo within 5 min | Day 1 |
| ⚡ **YOLO** | 1 | Merge small PR on **your** repo without review | Day 1 |
| 🦈 **Pull Shark** | 2 merges | 2 merged PRs to **other** repos | Week 1–2 |
| 🧙 **Open Sourcerer** | Multi-repo | PRs merged in 2+ different upstream repos | Week 2 |
| 🤝 **Pair Extraordinaire** | 1 co-author | Pair with someone; use `Co-authored-by: Name <email>` | Week 2 |
| 🧠 **Galaxy Brain** | 2 accepted | Answer questions in [GitHub Community](https://github.com/orgs/community/discussions) | Week 2–3 |
| 💜 **Public Sponsor** | 1 | Publicly sponsor any OSS dev ($1+/mo) | Anytime |
| ⭐ **Starstruck** | 16 stars | Promote **one** public showcase repo | Ongoing |
| ❤️ **Heart On Your Sleeve** | Beta | React ❤️ on GitHub changelog posts | Anytime |

---

## Day 1 — Instant badges (your repos)

### Quickdraw
```bash
gh issue create --repo OlaroPeterCelestine/OlaroPeterCelestine \
  --title "chore: profile polish" --body "Tracker item"
# Fix or note done, then within 5 minutes:
gh issue close --repo OlaroPeterCelestine/OlaroPeterCelestine <ISSUE_NUMBER>
```

### YOLO
```bash
git checkout -b docs/small-tweak
# make a tiny README tweak
./scripts/commit-as-me.sh "docs: clarify availability in profile"
git push -u origin docs/small-tweak
gh pr create --title "docs: clarify availability" --body "Minor profile copy tweak"
gh pr merge --merge --admin   # no review requested
```

---

## Week 1 — Pull Shark (2 merged PRs)

**Do not spam.** One quality PR beats ten rejected ones.

### Strategy
1. Pick **small** issues: docs, typos, missing type hints, test fixes
2. Comment on the issue first: "I'd like to work on this"
3. Wait for assignment (required for LangChain and many large repos)
4. Branch from **your fork**, commit with `commit-as-me.sh`
5. PR title: `fix: short description (Fixes #123)`

### Good targets (smaller repos, faster review)
- [fuseiq-io/fuseiq-agent-sdk](https://github.com/fuseiq-io/fuseiq-agent-sdk/issues/1) — LangChain adapter
- [topoteretes/cognee](https://github.com/topoteretes/cognee/issues/3405) — LangChain bridge
- Documentation fixes in **your forks** of gradio, openai-python, datasets

### PR workflow (no Cursor attribution)
```bash
gh repo clone OlaroPeterCelestine/openai-python
cd openai-python
git remote add upstream https://github.com/openai/openai-python.git
git checkout -b fix/docs-example
# edit files
../whatsai-bot/scripts/commit-as-me.sh "docs: improve quickstart example clarity"
git push -u origin fix/docs-example
gh pr create --repo openai/openai-python --head OlaroPeterCelestine:fix/docs-example \
  --title "docs: improve quickstart example clarity" --body "Fixes #XXX"
```

---

## Week 2 — Galaxy Brain & Pair Extraordinaire

### Galaxy Brain
1. Go to https://github.com/orgs/community/discussions
2. Filter **Q&A** → answer 2 questions with clear, helpful replies
3. Ask askers to mark your answer **Accepted**

### Pair Extraordinaire
When pairing:
```
git commit -m "feat: add adapter tests

Co-authored-by: Partner Name <partner@email.com>"
```
Use **real collaborators only** — not AI tools.

---

## Week 3 — Starstruck & Public Sponsor

### Starstruck (16 stars)
- Make **one** public showcase repo (sanitized demo of WhatsAI or LLM tutorial)
- Share on LinkedIn, X, dev Discord
- Ask colleagues to star if they find it useful

### Public Sponsor
```bash
# GitHub → Sponsors → pick any maintainer → $1/month → Public
```

---

## What NOT to do

- ❌ Fake stars, fake sponsors, or bot PRs
- ❌ Mass identical PRs across forks (maintainers will ban you)
- ❌ `Co-authored-by: Cursor` or AI attribution in commits
- ❌ Claim retired achievements (Arctic Vault, Mars 2020)

---

## Track progress

Create issue on your profile repo and check boxes weekly:

```markdown
- [ ] Quickdraw
- [ ] YOLO
- [ ] Pull Shark (2 merges)
- [ ] Open Sourcerer
- [ ] Pair Extraordinaire
- [ ] Galaxy Brain (2 accepted)
- [ ] Public Sponsor
- [ ] Starstruck (16 stars)
- [ ] Heart On Your Sleeve
```

---

*Clean code. Real contributions. Your name on every commit.*
