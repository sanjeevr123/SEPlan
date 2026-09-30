# SEPlan

**An SEP research platform for NUS students that simplifies university research, module mapping and comparison.**

> SEPlan is an independent student project and is **not** an official NUS platform. The landing page in this repo is a concept page, and the reviews and figures on it are illustrative mock data.

## The problem

NUS students deciding on a Student Exchange Programme (SEP) have to piece together information that is spread across EduRec, partner-university websites, course-mapping records, Reddit, Telegram groups, spreadsheets and seniors. Even after a lot of research, it is hard to tell whether a university is academically suitable, realistically attainable, affordable and a good personal fit.

Interviews with NUS students found:

- **Choosing a university is a process of elimination.** Students narrow down by country/region and cost first, and only then look at prestige, facilities and competitiveness.
- **Course mapping is a recurring pain point.** The hard part is finding usable, detailed course information overseas.
- **Information is fragmented.** Official sources cover administration well. Practical details (housing, visas, payments, SIM cards, food) come from unofficial sources.
- **Senior and peer knowledge is valuable but hard to find**, and it disappears when a cohort returns.
- **A generic chatbot is not enough.** General-purpose AI already answers generic questions, so the value has to come from SEP-specific data it cannot easily access.

## The product

The product has two layers:

**Knowledge layer** (SEP-specific, structured and community-generated)
- Historical module mappings, including the NUS and partner module codes, links to course pages and exam timing where available
- University pages with photos, a location map, exchange terms, typical monthly costs, housing and student life, and official links
- Reviews and experiences from previous students
- Destination communities and alumni

**Research layer** (AI grounded in that knowledge)
- Ask open-ended questions, such as "I need to clear CS3230 and CS3244, want to spend under S$18,000 and care about travelling. Compare my shortlisted universities."
- Compare shortlisted universities side by side against your own priorities
- Synthesise many reviews, noting when a conclusion rests on a small sample
- Use the user's shortlist and target modules as context

### Main features

| Feature | Description |
|---|---|
| **Search** | Discovery-first home page with popular universities and filters, with no sign-in needed to browse |
| **University page** | Decluttered, visual page with photo carousel, About, module mapping, exchange terms, housing and student life, a map and costs |
| **Research** | A chat sidebar that answers questions or adds findings to the university page |
| **Compare and rank** | Side-by-side comparison in which you can swap universities in place |
| **Share and feedback** | Lightweight post-SEP contributions (where you stayed, rent, courses taken, whether they were mapped) |

### Design principles

- **Distinguish the sources.** Official information, student experiences and AI-generated interpretation are shown separately, with source links and "last updated" dates.
- **Prominent AI warnings.** AI-generated research carries a clear notice that manual verification is preferred, especially for visas, deadlines and official course approvals.
- **Reduce effort.** Minimal input, optional onboarding, and concise summaries before detail.
- **Complement Telegram, don't replace it.**

## Go-to-market

The launch marketing plan is built around a 30-second "What kind of SEP traveller are you?" quiz that recommends universities from academic, budget and lifestyle preferences. It is promoted through:

1. Short-form social video (problem, solution, action)
2. Targeted Telegram group distribution with per-group tracking links
3. Faculty posters and welfare packs with per-location QR codes

The primary KPI is the quiz-to-platform conversion rate.

## Key risks

- Not reaching enough contributors, because reviews are sparse per university and the platform depends on new cohorts adding to it
- Access to historical mapping data, including legal limits on scraping or redistributing EduRec or university data
- Outdated information, and the cost of wrong information for students
- AI errors damaging trust in the whole platform
- Students finding EduRec, Telegram and ChatGPT "good enough"

## Roadmap

- **Phase 1, pre-application:** university discovery, module mappings, student reviews, application information, senior experiences and destination communities for a limited set of popular destinations. The Research interface is added once the data can be retrieved reliably.
- **Phase 2, full SEP lifecycle:** housing, costs, visa and preparation guides, food and transport recommendations, finding students going to the same destination, and travel planning.

## This repository

| File | Description |
|---|---|
| `index.html` | Single-page landing site (hero, scroll-driven research story, product walkthrough, agent demo, FAQ, early-access call to action) |
| `README.md` | This file |

The site is plain HTML, CSS and JavaScript with no build step. Open `index.html` in a browser to view it. Fonts load from Google Fonts.

## Status

Concept and landing page. Product research (interviews, wireframes and prioritisation) is done. There is no backend, real data or user accounts in this repository yet.
