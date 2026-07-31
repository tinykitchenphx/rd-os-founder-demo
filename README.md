# RD-OS — Lead Tracker

**A demonstration artifact.** RD-OS (Rapid Deploy Operating System) is an AI-assisted operational
workspace for small businesses. This repository holds a recorded walkthrough of one capability
inside it — the **Lead Tracker** — for hiring managers, recruiters, technical interviewers and AI
product teams.

No source code is published here. This repository contains the demonstration only.

---

## Watch

**[▶ Lead Tracker demonstration](video/rd-os-founder-demo.mp4)** · MP4 · 1920 × 1080 · 90 seconds

A WebM copy is kept alongside it at [`video/rd-os-founder-demo.webm`](video/rd-os-founder-demo.webm).
Stills are in [`screenshots/`](screenshots/) if you would rather scan than watch.

---

## The problem

Small businesses rarely lose information. They lose *where they put it*.

Operational context ends up spread across spreadsheets, inboxes, notebooks and memory. Every
question — what did we quote them, when did we last speak, what did they say about the nut allergy
— costs a search across four places, and the answer decays the moment someone doesn't write it down.

## The approach

RD-OS is deliberately not another conversational assistant. Conversation is a thin interface over a
thick problem: it answers a question and forgets. RD-OS organises operational information into a
**persistent workspace** where business context stays visible, actionable and connected across the
whole lifecycle of the work.

The Lead Tracker demonstrates that model end to end. Customer information, pipeline, dashboards,
workflow history, reporting and operational insight live in one continuous surface. The system
carries the administrative burden; every decision stays with the human.

## What the walkthrough shows

| | |
|---|---|
| **Executive Dashboard** | Eight live KPIs — pipeline value, open leads, booked and lost value, close rate, average days open, upcoming follow-ups, urgent leads |
| **Pipeline** | Five-stage board over a full nine-stage lifecycle, with a closed rail for lost and archived work |
| **Workflow movement** | Leads carried the length of the pipeline and back out of the closed rail again — stage totals recount on every drop |
| **Search** | Instant, across contact, company, phone, email, venue and tags |
| **Filters** | Nine filters — status, owner, priority, event type, source, tag, minimum revenue, date range |
| **Sorting** | Six orderings, with card order visibly changing |
| **Zoom** | Viewport scaling across the whole surface |
| **Lead Detail** | One continuous workspace: identity, customer information, event, notes, quote, tasks, follow-ups, communication, supporting information |
| **Timeline** | Chronological operational history with stage transitions |
| **Activity** | Auto-recorded event feed, newest first |
| **Charts** | Six reporting views — pipeline value, revenue, conversion funnel, sources, stage aging, weighted forecast |
| **Insights** | Derived probability, risk detection, missing information, recommended next action |

Every figure in the recording is computed from the demonstration book of business — twenty leads
with internally consistent histories. Nothing on screen is a mockup or a static image.

## Notes on the demonstration data

The twenty leads are fictional. Names, contacts and events are invented; no real client information
appears anywhere in the recording. The data is internally consistent by design — a lead is never
idle longer than it has existed, every stage was arrived at by a transition that appears in that
lead's own history, and the book contains real losses so the close rate is an honest number rather
than a flattering one.

## Built with

Next.js · React · TypeScript · Tailwind CSS · Framer Motion · ECharts · dnd-kit

---

## Repository contents

```
README.md                     this file
docs/PROJECT_SYNOPSIS.md      the longer-form project description
video/                        the demonstration, MP4 with a WebM copy
screenshots/                  eleven stills from the walkthrough
```

## Contact

**Traci White** — sales@tinykitchenphx.com
