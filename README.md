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
