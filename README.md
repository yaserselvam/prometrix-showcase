# Prometrix

**AI job-search intelligence.** Companies use AI to filter candidates; Prometrix gives the
candidate the AI: find the right roles, tailor the CV, write the cover letter, prep the interview,
and apply, all in one place.

> **Human-in-the-loop by design.** Prometrix generates; it never auto-submits an application and
> never fabricates experience. It reframes what is real, and a person always approves before
> anything is sent.

_Founded and built as a full-stack AI product. Currently in active development._

---

## What it does

| Area | What it does |
|---|---|
| **Find** | Personalised job feed from your preferences (role, salary, location, visa sponsorship), broad UK coverage, and a daily match email. |
| **Apply** | One-click optimise-then-apply: evaluate the role, tailor the CV, draft the cover letter, then hand off to the real application. A browser extension does the same on any job board. |
| **Score** | A 10-dimension role evaluation, a live ATS-style CV editor, and a free CV mini-audit. |
| **Prepare** | A mock-interview simulator with scored questions and a debrief, a LinkedIn profile optimiser, and a STAR story bank. |
| **Track** | An application tracker (applied to interview to offer) and a document vault for every CV and cover letter. |
| **Autonomous ops** | An agent-run "company" handles content and CV-service delivery overnight, built on the Claude Agent SDK, behind hard quality gates. |

Freemium model: a free tier plus paid Pro and Max plans.

---

## How it is built

- **Backend:** Python and FastAPI, async SQLAlchemy, and background workers for evaluation, alerts, and nightly agent runs.
- **Frontend:** Next.js, TypeScript, and Tailwind CSS.
- **AI:** Anthropic Claude across a tiered model setup (heavier models for evaluation and optimisation, lighter models for live scoring), with token and cost tracked on every call.
- **Extension:** a Chrome extension to optimise and apply on any job listing.
- **Trust by construction:** server-enforced quality gates block optimisation when the evaluator flags a fabrication risk or an unresolved critical gap; nothing is ever auto-submitted or published.

---

## Status

Founded and in active development. This repository is a public overview; the application source
is kept private.

Overview maintained by [Yaser Selvam](https://github.com/yaserselvam).
