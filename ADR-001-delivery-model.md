# ADR-001: Delivery Model for CampusService

- Status: Accepted
- Date: 2026-09-23
- Project: CampusService
- Author: Auezhanov Nurseiit

## Context

CampusService is an information system for receiving and processing technical issue reports at the university.

The project has a fixed academic schedule and mandatory deliverables during the semester. At the same time, detailed user requirements are not fully known yet and will be refined through interviews, feedback, story mapping and backlog management.

The first version of CampusService will focus on an MVP that supports the main workflow: creating a technical issue report, assigning a responsible specialist, changing request status, storing comments and status history, notifications and basic reporting.

Therefore, the project needs both predictable planning and the ability to adapt requirements during development.

## Decision drivers

The delivery model was evaluated using the following criteria:

1. Requirements uncertainty
2. Cost of change and error
3. Need for user feedback
4. Fixed academic deadlines
5. Team size and collaboration
6. Need for incremental delivery

## Considered options

### Option 1 — Predictive

The whole scope, schedule and requirements are defined before implementation.

Advantages:
- clear plan and milestones;
- simple progress tracking;
- suitable for fixed requirements.

Disadvantages:
- difficult to react to changing user requirements;
- feedback may arrive too late;
- unsuitable while the CampusService requirements are still being clarified.

### Option 2 — Adaptive

The project is delivered iteratively with a continuously updated backlog and frequent user feedback.

Advantages:
- easy to respond to changing requirements;
- frequent feedback;
- early delivery of working functionality.

Disadvantages:
- long-term scope is less predictable;
- academic milestones and mandatory artifacts still have fixed deadlines.

### Option 3 — Hybrid

The project uses fixed high-level milestones and semester deadlines, while detailed functionality is developed iteratively.

Advantages:
- keeps academic deadlines and required artifacts predictable;
- allows backlog and requirements to change after user feedback;
- supports incremental delivery of the CampusService MVP;
- combines planning with flexibility.

Disadvantages:
- requires discipline to keep the fixed plan and adaptive backlog synchronized;
- project documentation must be updated when decisions change.

## Decision

The Hybrid delivery model is selected for CampusService.

The project will use a fixed semester-level plan for major milestones and required laboratory artifacts. Inside these milestones, the team will manage functionality through an adaptive backlog and GitHub Projects.

Work items will move through the following workflow:

Backlog → Todo → In Progress → Review / Testing → Done

User feedback and new information may change priorities and detailed requirements, while the main project goals and semester deadlines remain controlled.

## Consequences

### Positive consequences

- The project can respond to new information from users.
- The MVP can be delivered incrementally.
- GitHub Projects can be used to manage the adaptive backlog.
- Major academic deadlines remain visible and predictable.
- Changes can be documented through ADRs and issues.

### Negative consequences

- The team must regularly update the backlog.
- Requirements and documentation may need revision after interviews.
- The project manager must control both milestone deadlines and day-to-day task flow.

## Rejected options

### Predictive

Rejected as the primary model because the detailed CampusService requirements have not yet been fully validated with real users.

### Adaptive

Rejected as the only model because the semester has fixed deadlines and mandatory deliverables that require higher-level planning.

## Review

This decision should be reviewed if the customer fixes all requirements in advance or if major project constraints change.
