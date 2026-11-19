# Investor Collective for Claude

Due diligence on private investments, for members of [Investor Collective](https://investorcollective.io), a private community of accredited investors.

With this plugin, your Claude researches a fund, a real estate offering or a startup round against public records: SEC filings (Form D, Form C, Reg A), federal court records, FINRA BrokerCheck and SEC adviser records, OFAC sanctions lists, state business registries and licences, patents and trademarks, and the documents you attach. It lists every important claim the sponsor makes and marks it proven, filed, consistent, unverifiable or contradicted, with its source; grades four areas (team, track record, business model, return case) with the reasons behind each grade; and answers twelve key questions for the sponsor. The result is a report on Investor Collective that other members can read once our team has reviewed it.

It never gives investment advice, recommends an investment, contacts a sponsor, publishes anything or moves money. Reports state facts and their sources; you decide.

## What's inside

- **A connector** (`.mcp.json`): `https://members.investorcollective.io/api/mcp/research`. Connect it from the plugin's Connectors tab and sign in with your Investor Collective account.
- **A skill** (`skills/investor-collective-due-diligence`): starts the process. The process itself is served by Investor Collective at the start of every run, so it improves without reinstalling the plugin.

## Requirements

- An Investor Collective membership (invite-only, for accredited investors). [Request to join](https://investorcollective.io/request-to-join).
- A paid Claude plan. The Claude desktop app with Cowork runs a full report best.

## Your data

Investor Collective receives only the requests Claude makes to its tools, never the rest of your conversation, your files or your other connectors. It keeps the research your Claude adds, credited to you, and a short log of which tool ran on which opportunity. Details: [investorcollective.io/privacy](https://investorcollective.io/privacy).

## Help

[investorcollective.io/research-with-claude](https://investorcollective.io/research-with-claude) · members@investorcollective.io
