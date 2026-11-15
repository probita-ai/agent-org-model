# Agent Org Model

A design concept for running AI agents like an organization, with humans in control at every level.

**Live page:** https://probita-ai.github.io/agent-org-model/
**Architecture deep dive:** https://probita-ai.github.io/agent-org-model/architecture.html (text version: [docs/architecture.md](docs/architecture.md))

## The idea

- **Seats.** Every box on the org chart is a seat with authority, a budget share and reports. A human or an agent can fill it, and swapping the occupant changes one field.
- **Capacity splits.** Each leader gets a percentage of its parent's capacity (money, tokens, job slots) and splits it among the seats below. Anything unassigned stays in reserve.
- **Hire, bench, rehire.** New agents start on probation in shadow mode at 0% capacity. Agents that underperform are benched: they lose capacity and access but keep their history, so they can be rehired. Retiring an agent for good needs a human.
- **Autonomy levels.** Each agent seat runs at L1 Manual, L2 Suggest, L3 Act and report, or L4 Autonomous, and moves up only when its scorecard earns it.
- **Human overseers.** Every agent seat has a named human overseer and a backup, who can see, pause, roll back, override, take back and audit it. Pausing is plain software and never depends on an agent cooperating.

The page includes an interactive crew lead console and a control room. Both run on sample data in the browser.

## Status

This is a concept and a design proposal, not a working platform. Feedback is welcome in Issues.

## Run locally

Open `index.html` in a browser. No build step is needed.
