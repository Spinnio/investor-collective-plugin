---
name: investor-collective-due-diligence
description: "Research a private investment (a deal, fund, startup raise or real estate offering) with Investor Collective's due diligence process: public-records research on the deal, the people and the companies behind it, written as a report of facts on Investor Collective. Use when the member asks to research, vet, look into, check out or run due diligence on a deal or investment, to carry on a report already started, or to refresh the research on an Investor Collective deal."
---

# Skill: Investor Collective due diligence

**This file carries no rules.** They live on Investor Collective and arrive
through the connector at the start of every run, so they improve without
reinstalling this skill.

Needs the **Investor Collective Due Diligence** connector, switched on.

The first time each tool saves something, Claude asks the member's
permission. Say once, at the start: answer **Always allow**, or set it for
all of them in Claude under Plugins → Connectors → Investor Collective Due
Diligence → Permissions → Write/delete tools → Always allow. Nothing these
tools do publishes a deal or contacts anyone. A scheduled run needs this set
beforehand, because nobody is there to answer.

## What to do

1. **A new deal:** call `run_due_diligence` with what the member gave you (its
   name, a link, the company behind it) before any web search. It records the
   deal (or finds it, if Investor Collective already has it) and returns the
   rulebook. Follow it step by step, with `opportunity` set to the deal it
   names, dispatching the helper agents it names as subagents.
2. **Carrying on:** `my_deals`, then pick up where the rulebook's steps left
   off. A run stays open until it's finished.
3. **A deal Investor Collective already has:** `get_deal`, then
   `start_refresh` if the member wants it updated.
4. Hand back what the rulebook's last step says, with the link to the report.

## What this skill never does

Contacts the sponsor, fills in a form, gives investment advice, or uses
material the member doesn't have permission to share.
