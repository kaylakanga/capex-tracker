# CapEx Tracker — Capital Project Delivery Dashboard

A front-end dashboard for tracking a capital project's money, schedule, and paperwork the way a project delivery team actually runs it: earned value, change management, and RFIs, all reconciled to the rand.

**Live demo:** open `index.html` in a browser — no build step, no dependencies.

## The sample project

This dashboard is an independent project-controls **case study**. The demo dataset models a project in a real setting: **The Maboneng Arts Centre — Arts & Community Hub Expansion, Johannesburg**, in the Maboneng Precinct, a working arts district. An R86.4M renovation and expansion of an arts and community centre, delivered in phases *while the centre stays open*. Phased occupancy, a heritage brick façade, a performance hall build-out, and a rooftop solar + battery system (so performances run uninterrupted through load-shedding) make it a genuinely interesting delivery problem, not just a spreadsheet.

The centre, its team, and every figure are **illustrative estimates created for demonstration** — the setting and the problem are real; the numbers are mine, built to show the workflows. Real client project data is confidential and would never appear here.

## Why this project

I chose an arts and community hub on purpose. Art tells a people's story — who they are, where they've been, what they're building next — and the buildings that hold that art deserve the same engineering care as any plant or tower. I'm proudly pro-Black and committed to Black people thriving in technical spaces; a case study like this is where the engineer in me and the community in me meet. And the main thing about me is that I love to learn — it's how I live my life — so of course my showcase project is one I'd learn something real from.

It's also a genuinely great delivery challenge: phased construction in a building that never closes, a heritage façade you can't fake, a performance hall where the acoustics have to be right on opening night, and a solar system that has to carry the show when the grid goes down. The kind of work this case study represents is exactly the kind I want to do for real.

## What it does

- **KPI header** — original budget, revised budget, actual cost, committed cost, forecast at completion (EAC), percent complete, and schedule status
- **Earned value** — CPI / SPI with cost and schedule variance, and an interactive **S-curve** (planned value vs earned value vs actual cost) with a status-date marker
- **Milestone timeline** — phase-by-phase delivery progress across design, heritage approvals, construction phases, and handover
- **Change order log** — every change with cost and schedule impact and status (approved / pending / rejected); approved changes roll up into the revised budget automatically
- **RFI log** — open, answered, and overdue requests for information with owners and due dates
- **Cost breakdown by division** — earthworks & civils, structure, heritage brick façade restoration, interiors & community kitchen, performance systems, and rooftop solar & storage
- **"How It Works"** — a plain-language explanation of earned value, change management, and RFI tracking for anyone new to project controls

Every number on the page is computed from one dataset, so the dashboard reconciles: division budgets total the R86.4M budget, actuals total the reported actual cost, and approved change orders (+R2,162,700) produce the revised budget of R88,562,700.

## Why I built it

During my project management internship at JLL, I worked inside capital project data and documentation — status reporting, project records, close-out deliverables — for projects running across the country. I built CapEx Tracker to bring that discipline into one clean view: the same questions a project team asks every week. *Are we ahead or behind? What changed, what did it cost, and who owes us an answer?*

## Tech

Vanilla HTML, CSS, and JavaScript in a single file. Charts are hand-drawn SVG. No frameworks, no build step.

## Roadmap

- Editable dataset (add/edit milestones, change orders, RFIs in the browser)
- Multiple projects with a portfolio roll-up view
- Exportable weekly status report (print/PDF view)
