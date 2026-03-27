# it-helpdesk-auto-routing
Automated IT Help Desk ticket routing system built on ServiceNow with NLP classification, SLA enforcement, and workflow automation

# IT Help Desk Auto-Routing System

Automated ticket routing system built on **ServiceNow PDI** that
classifies incoming IT incidents using keyword/NLP detection and
routes them to the correct assignment group — eliminating manual
triage.

## Status
> 🚧 In Development — core Business Rules and routing logic complete.
> Full deployment and testing in progress.

## Features
- Auto-classification by category (Hardware, Network, Software, Security)
- Priority matrix (Urgency × Impact → P1–P4)
- SLA enforcement with auto-escalation
- Email notifications to agents and users
- Auto-closure workflow after 3-day resolution window

## Tech Stack
- ServiceNow (Washington DC PDI)
- GlideScript (Server-side JavaScript)
- Workflow Editor
- Business Rules + SLA Definitions

## Architecture
![Architecture](docs/architecture.png)

## Roadmap
- [x] Assignment group design
- [x] Routing logic (Business Rules)
- [x] Priority auto-calculation
- [x] SLA definitions
- [ ] Virtual Agent intake flow
- [ ] Predictive Intelligence (ML classification)
- [ ] Performance Analytics dashboard
- [ ] Full deployment & testing

## Installation

1. Download the update set XML from `/update_sets/`
2. In ServiceNow go to:
   `System Update Sets → Retrieved Update Sets → Import Update Set from XML`
3. Upload the XML file
4. Click `Preview Update Set` → then `Commit Update Set`
5. All configurations will be automatically installed

## What's Included in the Update Set
- Auto-routing Business Rule (category → assignment group)
- Auto-priority Business Rule (urgency × impact matrix)
- SLA definitions (P1–P4 with escalation)
- Email notifications (assignment + acknowledgement + SLA warnings)
- Auto-closure Flow (3-day resolved → closed)
- SLA breach auto-escalation Business Rule

## Author
Chandu Anand Sai Vivek — [LinkedIn]([https://linkedin.com/in/yourprofile](https://www.linkedin.com/in/anand-sai-vivek-chandu/))
