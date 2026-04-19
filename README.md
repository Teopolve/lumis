<div align="center">

<img src="./logo.svg" alt="LUMIS" width="320"/>

### *Illuminate your search.*

**The world's first AI-native search engine.**
Powered by Claude. Built in public. Destined for the world.

[![Status](https://img.shields.io/badge/status-building%20in%20public-F5B82E?style=flat-square)]()
[![Phase](https://img.shields.io/badge/phase-0%20foundation-3B82F6?style=flat-square)]()
[![Built with](https://img.shields.io/badge/built%20with-Claude-F5B82E?style=flat-square)](https://anthropic.com)
[![License](https://img.shields.io/badge/license-MIT-10B981?style=flat-square)](./LICENSE)

**[🌐 Explore the live mockups](https://teopolve.github.io/lumis/mockups/01-homepage.html)** · [Concept Document](./docs/LUMIS_Concept_Document_v2.docx) · [Design System](https://teopolve.github.io/lumis/design-system/LUMIS_Design_System.html) · [Roadmap](./ROADMAP.md)

</div>

---

## What is LUMIS?

LUMIS (from Latin *lumen* — light) is a next-generation search engine built from first principles. It is not *"Google with a chatbot on top"* — it is a complete reimagination of how humans access knowledge, with Claude as its reasoning core.

### The problem

Today's search is broken. Google returns links, not answers. ChatGPT answers, but can't verify anything in real-time. Between the two, people waste hours every day navigating noise, ads, SEO-optimized nothing, and unverifiable claims.

### The vision

LUMIS sits at the intersection of three worlds:

- **Not a pure AI** (like ChatGPT) — because it searches the real-time web
- **Not Google** — because it understands, synthesizes, and cites sources
- **The intelligent librarian with access to the world**

One mission: *make human knowledge accessible, understandable, and trustworthy for every person on the planet — with no advertising, no algorithmic manipulation, no compromises.*

---

## See LUMIS in motion

Four interactive mockups, built with Claude Design, showing what LUMIS will feel like.
**Click each one to explore live in your browser:**

### 🏠 [01 — Homepage](https://teopolve.github.io/lumis/mockups/01-homepage.html)
*The invitation. Zen, editorial, calm.*

### 💡 [02 — Answer Page](https://teopolve.github.io/lumis/mockups/02-answer-page.html)
*The promise kept. Synthesized answer with cited sources and Trust Score.*

### 🧠 [03 — Deep Mode](https://teopolve.github.io/lumis/mockups/03-deep-mode.html)
*The power. Real-time research cockpit analyzing dozens of sources.*

### ⚖️ [04 — Perspective Engine](https://teopolve.github.io/lumis/mockups/04-perspective-engine.html)
*The ethics. Constitutional AI applied to search — every viewpoint, equal dignity.*

---

## The 17 features that make LUMIS different

### Fundamentals
1. **Synthesized answers with cited sources** — Claude reads the best sources and delivers a direct, complete answer with every claim linked to its origin
2. **Conversational, multi-turn search** — LUMIS is a dialogue, not a query. Follow up, clarify, go deeper
3. **Zero advertising, zero algorithmic bias** — no advertiser can buy positions. Only quality determines ranking
4. **Deep Mode** — for serious research, LUMIS analyzes dozens of sources, academic papers, official data

### Innovative (never-before-seen integrated)
5. **Temporal Lens** — search across specific time windows; see how a topic evolved
6. **Perspective Engine** — for contested topics, automatically presents multiple legitimate viewpoints
7. **Trust Score** — dynamic reliability score for every source, based on peer-review, track record, transparency
8. **Visual Knowledge Graph** — navigate concepts as a graph, not a list
9. **Anti-Hallucination Layer** — every claim verified against source material in real-time
10. **Cross-Language Deep Search** — simultaneous search across 50+ languages
11. **Research Memory** — LUMIS remembers your research sessions (with explicit consent)
12. **Prediction Insights** — data-driven projections with explicit uncertainty
13. **Comparison Mode** — structured, unbiased comparison of any two things
14. **True Privacy Mode** — zero data stored, queries encrypted, no profiling
15. **Academic & Patent Search integrated** — arXiv, PubMed, JSTOR, patents, open government data
16. **Synthesis Report** — turn any session into a structured, downloadable document

### Radical transparency
17. **Source Challenge** — users can "challenge" a source; LUMIS recomputes and shows the difference
18. **Research Trails** — every session leaves a navigable, shareable path
19. **Education Edition** — age-calibrated, free for schools and universities
20. **Mistake Log** — LUMIS publicly admits its errors in a transparent log
21. **Collaborative Research Rooms** — shared research spaces where LUMIS holds the team's context

---

## The LUMIS Constitution

Inspired by Anthropic's Constitutional AI, these 10 principles filter every response before it reaches the user:

1. **Truth before all else** — never a pleasing answer over a true one
2. **Multi-perspective always** — on contested topics, show all legitimate viewpoints
3. **Admit uncertainty** — when evidence is weak, say so explicitly
4. **Zero political or commercial bias** — no party, no company, no ideology favored
5. **Child protection** — minors are not ad targets or testing subjects
6. **Privacy as a fundamental right** — True Privacy Mode is not premium, it's a right
7. **Algorithmic transparency** — users can always know why LUMIS answered a certain way
8. **No emotional manipulation** — no dark patterns, no engagement-maximizing nudges
9. **Universal accessibility** — WCAG AAA as target, not afterthought
10. **Public accountability** — monthly Transparency Reports, every error admitted

Read the full Constitution and AI Safety Framework in the [Concept Document](./docs/LUMIS_Concept_Document_v2.docx).

---

## Tech stack

| Layer | Technology |
|-------|------------|
| Frontend | Next.js 15 (App Router) + TypeScript + Tailwind CSS v4 |
| Backend | Node.js + Next.js API Routes (evolving to microservices) |
| AI Core | **Anthropic Claude API** |
| Search layer | Brave Search API (for real-time web retrieval) |
| Web reading | Playwright |
| Database | PostgreSQL (Supabase) + Redis (Upstash) |
| Auth | Clerk |
| Hosting | Vercel + Cloudflare |
| Monitoring | Sentry + Vercel Analytics |

Built with [Claude Code](https://claude.com/claude-code) and [Claude Design](https://claude.ai/design).

---

## Project status

**Current phase**: Phase 0 — Foundation
**What exists today**: complete concept document, full design system, 4 interactive mockups (live!)
**What's next**: Next.js setup + MVP (Phase 1, starting this week)

See the full [ROADMAP](./ROADMAP.md) for the 10-month development plan across 6 phases.

> LUMIS is being built in public, one commit at a time. Watch it emerge.

---

## Documentation

- [**Concept Document v2**](./docs/LUMIS_Concept_Document_v2.docx) — 18 chapters: vision, features, architecture, AI Safety Framework, Constitution, personas, demo scenarios, risks, business model, go-to-market
- [**Design System (live)**](https://teopolve.github.io/lumis/design-system/LUMIS_Design_System.html) — colors, typography, components, mockup in motion
- [**CLAUDE.md**](./docs/CLAUDE.md) — context file for Claude Code sessions
- [**Roadmap**](./ROADMAP.md) — phase-by-phase development plan

---

## Follow the build

This project is being built entirely in public, powered by Claude. If you want to follow the journey:

- ⭐ **Star this repo** to watch it evolve
- 🐦 Follow updates on X: [@Teopolve](https://x.com/Teopolve)
- 💡 Open an issue with ideas, questions, feedback
- 📬 Feedback welcome — LUMIS is built for people, not for noise

---

## License

MIT — see [LICENSE](./LICENSE).

You're free to study, learn, and build on ideas here. If you use substantial parts of this work, please attribute it.

---

<div align="center">

**LUMIS**
*Illuminate your search.*

Built with light, for those who seek.
Independent project — Matteo, 2026.

</div>
