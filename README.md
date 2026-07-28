# Job Finder & Application Tracker

Daily Cursor Automation finds IT-services roles (≤4 years experience), applies where possible, and updates this tracker.

**Runtime:** each run is hard time-boxed to **5–8 minutes** (apply first, then commit tracker updates and stop).

## Profile

- **Candidate:** Jayanth Kanala
- **Resume:** https://jayanthkanala.github.io
- **Cert:** Microsoft Power BI
- **Target roles:** Data Analyst, BI Analyst, Full Stack Developer, Power BI Developer, and related IT services roles
- **Experience filter:** roles asking for under 4 years (entry / junior / 0–3 YOE)
- **Contact:** jkanala0@gmail.com

## Dashboard

Live board: **https://jayanthkanala.github.io/job-tracker/**

Reads `tracker/applications.json` (status filters + search + **Fetched** date). Updates whenever new data is **pushed** to `master` (GitHub Pages rebuilds from the repo — it will not change if the automation does not commit).

Each job includes `fetched_at` (when it was first found). The header shows **Data updated** from the last tracker write.

## Tracker

See [`tracker/applications.json`](tracker/applications.json) for application status.

| Status | Meaning |
|--------|---------|
| `found` | Listed, not yet applied |
| `applied` | Application submitted |
| `blocked` | Could not apply (login wall, CAPTCHA, etc.) |
| `skipped` | Duplicate or poor fit after review |
| `response` | Employer replied |
| `rejected` | Closed / rejected |
| `interview` | Interview stage |
