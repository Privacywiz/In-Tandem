# Tandem

**[Open the demo →](https://privacywiz.github.io/In-Tandem/)** · [Decision tree →](https://privacywiz.github.io/In-Tandem/decision-tree.html) · [How it works](Tandem_Overview.md)

Tandem is a prototype of a shared AI governance record for product, engineering and privacy teams. Instead of a review at the end, everyone works from one record from the day a system is registered until it's retired. Every flag, block, override and approval stays on it.

The demo runs in your browser with a fictional adtech company, Neffy Analytics. Nothing you type is saved or sent anywhere.

## Try it in ten minutes

1. Open the demo and pick **Implementer**. Register a system: choose Builder, Procurer or Enabler and watch the questions change.
2. Switch to **Governance lead** (role switcher, top right). Open the findings queue for the Neffy RTB model. Each finding compares the intake to Neffy's own policy text. Give every finding a status (block it, accept a fix plan, assign it or escalate it) and close the review.
3. Switch to **Implementer** and open the Neffy RTB model to see what came back.
4. Switch to **Accountable owner** and dispute the hard block on the resume-screening model.
5. Finish with **Executive** for the org-wide view.

## Who does what

| Role | What they do |
|---|---|
| Implementer | Brings the system in: a **builder** (built it), **procurer** (bought it) or **enabler** (turned it on inside a tool you already use). Registers it and answers the intake. |
| Reviewer | Privacy & ethics, policy, or security. Checks assigned systems against your policies, raises flags and blocks. |
| Accountable owner | Holds final deployment authority for a business unit. Can dispute a block; only the governance committee can override one. |
| Executive / governance committee | Sees totals across all systems and the override history. Decides disputes. |
| Governance lead | Keeps your approved policies loaded, shows where two policies overlap, and routes findings to owners. |

## What the labels mean

| Label | Meaning |
|---|---|
| Conflicts with policy | The intake says the system does something your policy doesn't allow. |
| Missing info | The intake left out something your policy needs before deployment. |
| Matches policy | Nothing to fix for this item. |
| Advisory flag | Logged and visible to reviewers; the system can still advance. |
| Hard block | The system can't advance until the block is fixed or the committee overrides it. |
| Escalated | Sent outside the review through your organization's own escalation procedure. |
| Policy set | The version of your approved policies the system was compared against. |

## What Tandem doesn't do

- It doesn't tell you what the law requires. It compares systems to **your organization's own policies**, as your organization approved them.
- It doesn't replace your lawyers or decide when to involve them. Counsel isn't a role in Tandem.
- It doesn't store legal advice. If your procedures involve counsel, the record can show only that counsel was consulted and when. There's no field for what counsel said, and the note fields ask people not to paste it.
- The demo's policies, people and findings are invented. Don't copy its policy text into your own.

## Escalation

Tandem doesn't decide when a question goes to counsel or anyone else outside the review. Your organization's own procedures do. In Tandem, a finding can be marked **Escalated**, and it stays open until the outcome comes back.

## Files

| File | What it is |
|---|---|
| `index.html` | The interactive demo |
| `decision-tree.html` | Roles, the routing decision tree and intake questions by type |
| `Tandem_Overview.md` | How the system works, in prose |
| `tandem_schematic.svg` | One-page diagram |
| `assets/intandem.css` | Styles from the InTandem design system |

Everything is static HTML. Download the repo and open `index.html`, or fork it and turn on GitHub Pages.

## Background

The design comes from privacy by design: safeguards work better built into the process than reviewed in at the end. Applied to AI governance, that means intake routing, a shared record and a decision log that run alongside a product for its whole life.

The ethical R&D principles developed by the R&D team at [AERDF](https://www.aerdf.org) were a direct inspiration. They treat respect for persons, reciprocal benefit, transparency and data minimization as binding design requirements, and this prototype tries to put that into practice.

Built by Asia Parks with Claude by Anthropic. Asia is a privacy attorney, but publishing this prototype doesn't make her your lawyer.

## Disclaimer

Informational only. Not legal advice. Using Tandem or this repository doesn't create an attorney-client relationship with anyone. Confirm anything legal with your own counsel.

Released under CC0 1.0 (see `LICENSE`).
