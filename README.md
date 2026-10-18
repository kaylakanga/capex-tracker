# CapEx Tracker — Capital Project Delivery Dashboard

A front-end dashboard for tracking a capital project's money, schedule, and paperwork the way a project delivery team actually runs it: earned value, change management, and RFIs, all reconciled to the dollar.

**Live demo:** open `index.html` in a browser — no build step, no dependencies.

## The sample project

The demo dataset follows a fictional project: **The Sankofa Centre — Black Arts & Community Hub Expansion, Toronto.** A $4.8M renovation and expansion of a Black-led arts and community centre, delivered in phases *while the centre stays open*. Phased occupancy, heritage elements, a performance hall build-out, and accessibility upgrades make it a genuinely interesting delivery problem, not just a spreadsheet.

All figures are **sample data for a fictional project**, created to demonstrate the workflows. Real client project data is confidential and would never appear here.

## Why this project

I chose a Black arts and community hub on purpose. Art tells a people's story — who they are, where they've been, what they're building next — and the buildings that hold that art deserve the same engineering care as any plant or tower. I'm proudly pro-Black and committed to Black people thriving in technical spaces; a project like this is where the engineer in me and the community in me meet.

It's also a genuinely great delivery challenge: phased construction in a building that never closes, heritage details you can't fake, and a performance hall where the acoustics have to be right on opening night. The Sankofa Centre is fictional — but the kind of work it represents is exactly the kind I want to do for real.

## What it does

- **KPI header** — original budget, revised budget, actual cost, committed cost, forecast at completion (EAC), percent complete, and schedule status
- **Earned value** — CPI / SPI with cost and schedule variance, and an interactive **S-curve** (planned value vs earned value vs actual cost) with a status-date marker
- **Milestone timeline** — phase-by-phase delivery progress across design, heritage approvals, construction phases, and handover
- **Change order log** — every change with cost and schedule impact and status (approved / pending / rejected); approved changes roll up into the revised budget automatically
- **RFI log** — open, answered, and overdue requests for information with owners and due dates
- **Cost breakdown by division** — general conditions, structure, envelope & heritage, interiors, performance systems, site & accessibility
- **"How It Works"** — a plain-language explanation of earned value, change management, and RFI tracking for anyone new to project controls

Every number on the page is computed from one dataset, so the dashboard reconciles: division budgets total the $4.8M budget, actuals total the reported actual cost, and approved change orders (+$120,150) produce the revised budget.

## Why I built it

During my project management internship at JLL, I worked inside capital project data and documentation — status reporting, project records, close-out deliverables — for projects running across the country. I built CapEx Tracker to bring that discipline into one clean view: the same questions a project team asks every week. *Are we ahead or behind? What changed, what did it cost, and who owes us an answer?*

## Tech

Vanilla HTML, CSS, and JavaScript in a single file. Charts are hand-drawn SVG. No frameworks, no build step.

## Roadmap

- Editable dataset (add/edit milestones, change orders, RFIs in the browser)
- Multiple projects with a portfolio roll-up view
- Exportable weekly status report (print/PDF view)
