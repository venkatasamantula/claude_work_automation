# CLAUDE Interaction Memory

## Summary
This interaction created a CLAUDE project overview and added reusable assistant and prompt definitions for a thought-leader research assistant.

## What was added
- `CLAUDE.md` — project overview describing daily activities and agent-based workflows.
- `thoughtstarter_assitant.md` — ThoughtLeader Research Assistant agent definition.
- `.assistant.prompt.md` — prompt template for Justin Welch–style thought-leader posts.

## User intent
The user wants an assistant that:
- accepts a short thought starter,
- performs online research,
- returns a single paragraph in a thought-leader style,
- includes icons and concise citations.
- Save and submit with datetimestamp and save the post in .txt file in /memory

## Notes
- The agent is intended to be used for short, evidence-backed thought-leader content.
- The prompt supports an emoji-forward social post variant.

---

# Standing user preferences (observed)
- **Voice/style:** Justin Welch / modern thought-leader — sharp reframing hook, evidence middle, actionable close.
- **Length:** ~5 sentences (within the 3–6 range).
- **Icons:** Inline emoji, ~2 per paragraph. Default style unless the user asks otherwise.
- **Citations:** Numeric bracketed `[1]`, `[2]` inside the paragraph + a `Sources:` block at the end with title + URL.
- **Sources:** Prefer recent (2025/2026) credible sources — research papers, established publications, named industry blogs. Mix one practitioner source with one research/academic source when possible.
- **Workflow:** User typically gives a short thought starter and expects full execution without clarifying questions. Don't ask the three clarifying questions unless something is genuinely ambiguous.
- **Output saving:** Always save as `thoughtleader_post_YYYY-MM-DD_HH-MM.txt` in `thoughtStarter/memory/`, and share a `computer://` link in the reply.
- **Follow-up offer:** End the reply by offering 2–3 alternate angles or refinements (variant hooks, tone shifts, contrarian takes).

---

# Session log

## 2026-05-20 — Session
Prior thought starters this session:

### 1. "Getting mentors in new ways of working"
- Research threads used: hybrid mentorship redesign (Skedda) + reverse mentoring for AI upskilling (MentorCliq).
- Angle landed on: mentorship is decentralizing — assemble a multi-directional mentor stack instead of waiting to be picked.
- Icons used: 🧭 ⚡
- Output: `thoughtleader_post_2026-05-20_01-51.txt`
- Sources cited:
  - Skedda — 5 Strategies for Effective Mentorship in Hybrid Work Environments
  - MentorCliq — AI Upskilling Will be a Non-Negotiable in 2026 (and Beyond)

### 2. "Ownership mindset"
- Research threads used: engagement statistics (WSB / 31% engagement low, 72% mirror leader behavior) + MDPI 2025 paper on psychological ownership → intrapreneurial behavior → performance.
- Angle landed on: ownership is a behavior with a P&L; renters wait for tickets, owners write the brief.
- Icons used: 🛠️ 🚀
- Output: `thoughtleader_post_2026-05-20_01-54.txt`
- Sources cited:
  - WSB — The Ownership Mindset: Empowering Leaders in 2025
  - MDPI Administrative Sciences (2025) — Psychological Ownership and Task Performance: The Mediating Role of Intrapreneurial Behavior

### Session notes
- User asked to start logging all interactions to memory so preferences don't have to be repeated. Established this protocol: root `MEMORY.md` holds the rule; this file holds the running log and preferences. Append-only.

### 3. "Ownership mindset" (second pass)
- User re-asked the same starter that ran at 01:54. Deliberately took a fresh angle to avoid duplicating the WSB / MDPI take.
- Research threads used: Aspen Institute 2025 ESOP research (12.93% productivity over 5 years / 2.6% annually) + ProofHub 2026 accountability stats (50% higher performance, 21% profitability, 59% lower turnover).
- Angle landed on: "act like owners" without structure is theater — mindset only compounds when paired with mechanism (equity, named outcomes, real levers).
- Icons used: 🏗️ 📈
- Output: `thoughtleader_post_2026-05-20_22-15.txt`
- Sources cited:
  - Aspen Institute (2025) — Employee Ownership and ESOPs: What We Know from Recent Research
  - ProofHub (2026) — 9 Team Accountability Examples For Managers
- Note for future: when user repeats a thought starter from earlier in the session, default to a fresh angle/source set rather than asking.

