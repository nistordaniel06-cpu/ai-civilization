# AI Civilization — Autonomous World V1

Public Android-friendly browser prototype of an autonomous isometric city simulation.

## Play
Open the GitHub Pages URL after enabling Pages for main / root, or open index.html locally in a browser.

## Features
- Autonomous construction and mayor decisions (rules-based)
- Population, housing, farming, employment, economy, research and elections
- Isometric city, event log, speed controls, pause and local save
- Runs offline without API keys

## V2 — Citizen simulation
- Named citizens with age, home assignment and deterministic job allocation
- Employment and unemployment dashboard
- Visual commuter dots and vehicle markers (not yet pathfinding or car sprites)
- Citizens persisted in local saves

## Limitations
This is an early playable simulation, **not yet** LLM-powered agents or a native Android APK. The city progresses only while the page is open.

## Roadmap
1. Godot 4 Android client and native APK build
2. Individual citizen agents, households, businesses, goals and memory
3. Election/policy agents and transparent decision history
4. Research and sandboxed self-improvement proposals
5. Optional server-side simulation and AI model adapters with cost controls
6. Separate paper-trading lab with **no real-money execution** until explicitly approved and risk reviewed

## Security
Never commit API keys or brokerage credentials. Keep simulated game currency separate from real funds.


## Product direction — V4.1 (October 2026)

Three separate mobile-first pages:
- `index.html`: autonomous city, population, companies, labor market, happiness, economy, routes and local saves.
- `governor.html`: Governor OS, policies, ministry allocations, project approvals, transparent advisor and decision history.
- `roadmap.html`: public development roadmap and completed milestones.

### Simulation principles
- The game remains **offline-first**, rule-driven, and does not pretend to use external LLMs.
- The Governor can override selected public policies and approve discretionary construction; city automation continues otherwise.
- Saves are browser-local (`localStorage`, key `aiciv-save`). No login, backend persistence or device synchronization yet.
- A revision counter helps reconcile Governor changes with the live city tab; simultaneous writes may still race and require a transactional backend in a future version.
- Private companies, payroll and consumption are currently **simplified indicators**, not a complete double-entry economy.
- Real-world financial transactions, trading and external actions are not enabled; any future capability requires explicit approval and controls.

### Next engineering priorities
1. Extract the simulation into testable modules, introduce save migrations and automated tests.
2. Add households, citizen wallets, real agent-to-agent transactions and economic balancing.
3. Add persistent connected road network, route caching, vehicle sprites and building inspection.
4. Introduce ministerial proposals with traceable reasons, budgets and audit trails.
5. Add optional LLM agents with strict token budgets, simulation-only permissions and deterministic fallback.
