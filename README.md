# Metis — interface prototype

Static prototype screens for **Metis**: AI agents that run back-office operations for
Indian insurers and asset managers, and produce a regulator-ready record of every
action they take.

**Live:** https://shloknambiar.github.io/metis-mockup/

All data is fictional. *Sahyadri Insurance Services* and *Deccan General* are invented
companies; the agents, policy numbers and figures are sample data for demonstration.

## What's here

Fourteen screens in two sets.

**One day — Priya's Tuesday** (`journey/`) — one motor policy renewal moving across
five surfaces and one ledger:

| Screen | |
| --- | --- |
| `whatsapp.html` | A ₹8,240 write-off approved from a phone, recorded with the channel named |
| `teams.html` | An agent halts on a missing claim record and says so in Teams |
| `needs-you.html` | The human supplies what was missing |
| `ledger.html` | The full case trail — **interactive**, click a blue chip for the source |
| `ask.html` | Cited answers, and a question the system refuses to guess at |
| `memory.html` | Tonight's memory review, including an unresolved conflict |

**The console — admin to analyst** (`console/`) — the same app seen from five roles:

| Screen | |
| --- | --- |
| `today.html` | The floor right now — **interactive**, click an agent to follow their day |
| `roles.html` | Five roles, five different apps out of one |
| `analyst.html` | The junior view: three nav items, one queue |
| `workflow-studio.html` | A workflow as an editable document, with autonomy tiers |
| `routing.html` | Data class decides the model; unclassified data is refused |
| `connections.html` | Every system an agent can reach, and how far in |
| `monitor.html` | Runs, halt reasons, unit cost |
| `access.html` | Roles, and config changes written to the same ledger |

## Two rules that run through every screen

**Blue means traceable.** The accent is reserved for provenance — citation chips,
source links, verified markers. Never an ordinary button.

**A halt is not an error.** When a required value is missing, the agent stops rather
than defaulting it. Stopping is the system working correctly, so it is styled as a
calm request for help, never as a failure.

## Running locally

No build step. Open `index.html`, or serve the folder:

```bash
python -m http.server 8000
```

## Stack

Plain HTML and CSS. Two screens use a little vanilla JavaScript for the interactive
parts. Type is Hanken Grotesk, Newsreader and JetBrains Mono via Google Fonts;
colours follow the Metis design system.
