# OpsPulse — Infrastructure Monitoring & Incident Response Platform

OpsPulse is a polished front-end simulation of an infrastructure operations console. It brings service health, resource inventory, incident workflows, logs, alert thresholds, and operational reporting into one workspace.

## Features

- Operations overview with live-simulation KPI cards and performance charts
- Infrastructure inventory with search, resource health, CPU and memory utilization
- Incident center with severity, acknowledgement, assignment, and resolution workflows
- Log explorer with text search and level/service filters
- Alert-rule management with enable/disable switches and rule creation
- Reports view with reliability metrics and CSV export
- Activity feed, responsive layout, demo settings, and reset option
- Simulated metric updates and local-only demo data

## Run locally

No build step or package installation is required.

1. Download or clone this repository.
2. Open `index.html` in a modern browser.
3. For a local development server, use VS Code Live Server or run `python -m http.server 8000` in the project folder, then open `http://localhost:8000`.

## Tech stack

- HTML5
- CSS3 (responsive layout)
- Vanilla JavaScript
- SVG charts
- CSV export using browser APIs

## Important note

This project is a learning/demo environment. Metrics, incidents, service health, logs, and alert events are simulated. It does not connect to real infrastructure or send real notifications.

## Suggested next development milestones

1. Add a Flask API and PostgreSQL database for persistent data.
2. Implement authentication and role-based access (Admin, Operator, Viewer).
3. Connect real monitoring data via Prometheus metrics endpoints.
4. Add Docker Compose and CI checks.
5. Deploy the demo and document the architecture.

## Project structure

```text
opspulse/
├── index.html
├── styles.css
├── app.js
├── README.md
└── PROJECT_NOTES.md
```

## Portfolio highlights

This project demonstrates practical familiarity with infrastructure monitoring concepts, service health, incident lifecycle, log filtering, threshold-based alerts, resource inventory, operational reporting, UI state management, and export workflows.
