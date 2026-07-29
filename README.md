# ObserveOps — Settings module (prototype)

A single self-contained HTML prototype of the **Settings** module for Motadata
ObserveOps: the full category rail, the Discovery Profile list, and the
Create Discovery Profile flow.

**Live:** https://kisu1311.github.io/setting/

## Three options

Three takes on the same module — switch between them with the toggle in the top bar
of any page.

| | |
|---|---|
| **Option 1 — Live parity** (`dashboard-ai-chat-assistant.html`) | Faithful to the live product (build 10.0.0). |
| **Option 2 — Improved** (`settings-improved.html`) | Identical everywhere except **Agent Based Discovery**: a leaf in the tree that opens straight onto the form, with an inline method switcher, pre-flight target validation, failure reasons with retry, and apply-to-all provisioning. |
| **Option 3** (`settings-option3.html`) | Same as Option 2, but the install method is a **field in the form** rather than a tab strip — each choice states what it requires, and the agent tile rules out what can't apply (picking Linux disables Group Policy and says why). |
| **Option 4** (`settings-option4.html`) | All three methods stay on screen as an **accordion** — the chosen one expands in place with its fields, the other two remain readable one-liners carrying their trade-off (Fastest / No credentials needed / Best at scale). |
| **Option 5** (`settings-option5.html`) | **Question-led.** Asks *"How would you like to install the agent?"* and offers the three as things you can say yes to ("I have an admin account for these machines"), with the product's own name underneath, a *what happens next* line, and a *help me choose* nudge. |

## What's in here

- `dashboard-ai-chat-assistant.html` — Option 1. The filename is vestigial; it
  began as a copy of the Dashboard clone.
- `settings-improved.html` — Option 2.
- `settings-option3.html` — Option 3.
- `.reference/monitor-icons/` — vendor/type icons used by the Discovery Profile grid.
- `index.html` — redirect so the root URL opens the prototype.

## Notes

- No build step. Open the HTML file directly in a browser.
- All hostnames, IP addresses and machine names shown in the grid are
  **placeholder values** from the RFC 5737 documentation ranges — not real infrastructure.
