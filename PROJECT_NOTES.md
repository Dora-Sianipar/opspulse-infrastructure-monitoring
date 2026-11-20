# OpsPulse Project Notes

## Project purpose
Create a portfolio-ready operations dashboard that helps a junior IT professional demonstrate how they understand monitoring and incident response workflows.

## Problem statement
Small teams need a clear operational view of monitored resources, service health, incidents, and logs. OpsPulse simulates that view and provides simple workflows to investigate and act on events.

## User roles (future backend)
- Viewer: read dashboards and reports
- Operator: acknowledge incidents, resolve incidents, and manage resources
- Administrator: manage alert rules, settings, and users

## Core workflows
1. Review service health and KPI overview.
2. Search infrastructure inventory and inspect resource status.
3. Acknowledge an incident, assign ownership, then resolve it.
4. Search logs by message, severity, and service.
5. Enable/disable alert rules and create a rule.
6. Export logs or a reliability snapshot to CSV.

## Data model (proposed)
- Resource: id, name, type, region, status, cpu_percent, memory_percent, uptime
- Incident: id, title, severity, service, status, created_at, owner, detail
- LogEvent: timestamp, level, service, message
- AlertRule: id, name, description, threshold, scope, enabled
- Activity: id, event_type, message, timestamp

## Test checklist
- [ ] Navigation switches sections and active menu state
- [ ] Infrastructure search filters rows
- [ ] Incident filters show matching status
- [ ] Acknowledge assigns incident to demo operator
- [ ] Resolve incident updates status and activity feed
- [ ] Create incident form adds a new incident
- [ ] Create resource form adds inventory entry
- [ ] Log filters work by text, severity, and service
- [ ] CSV export downloads data
- [ ] Alert rule toggles and creation work
- [ ] Responsive layout works on narrow screens
- [ ] Reset returns to initial demo state

## Limitations
All operational data is simulated in browser memory. There is no backend, real telemetry, authentication, or real alert delivery in this version.
