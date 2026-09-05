# Setting Up the "Ask an Alum" Layer (Maintainer Notes)

This repo uses **GitHub Discussions** as the community/Q&A layer instead of a custom app. It's free, versioned, public by default, and needs zero backend.

## One-time setup
1. In the repo's Settings → Features, enable **Discussions**.
2. Create these categories:
   - **Ask an Alum** (Q&A format) — one thread per guide; students ask, the guide's author (and anyone else) can answer
   - **General** (Discussion format) — open chat, announcements, campus-specific news
   - **Feedback** (Discussion format) — suggestions for the repo itself

## Per-guide workflow
1. When a guide is merged, the author (or a maintainer) opens one "Ask an Alum" thread titled after the guide, e.g. `TellSoft — SDE Intern`.
2. Paste the thread link back into that guide's `ask_me_thread` field via a follow-up PR.
3. Students find the link at the bottom of the guide and ask there — answers are public and searchable forever, so the same question never has to be answered twice.

## Why this instead of DMs or booking calls
- No scheduling, no ops overhead, no burnout risk for alumni
- Every answer compounds — it helps every future student who reads the guide, not just the one who asked
- If an AI layer gets added later (see README roadmap), these threads become the training data for an auto-answer bot — the more questions get asked and answered here, the smarter that gets, for free
