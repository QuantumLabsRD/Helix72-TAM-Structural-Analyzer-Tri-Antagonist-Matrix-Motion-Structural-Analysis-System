System Architecture — Description

The Helix72 TAM Structural Analyzer is built as a modular, four-layer architecture designed for deterministic, real-time biomechanical analysis. Each layer has a fixed responsibility, ensuring stability, traceability, and clean separation between measurement, interpretation, and presentation.

Layer 1 — Core System
Handles camera input, pose acquisition, frame gating, pose lock, and global state management. This layer ensures consistent data flow and prevents unstable frames from entering the engine.

Layer 2 — Geometry & Metrics Engine
Transforms raw pose landmarks into structured biomechanical metrics. This includes joint angles, ankle/knee collapse deviation, hip torque estimates, corridor alignment, center-of-mass (COM) models, and node-level burden calculations. It defines the measurable state of the body without interpretation.

Layer 3 — TAM / Helix72 Solver
Applies the Tri-Antagonist Matrix (4-role model) and Helix72 stability logic to interpret structure. It determines:

Agonist (driver)

Antagonist (counterforce)

Bi-Antagonist (stabilizer state)

Tri-Antagonist (anchor/saboteur)

It also evaluates:

static vs dynamic states

chain integrity (stable → cascade)

origin node and propagation pathways

contradiction detection and certainty scoring

This layer converts metrics into structural meaning.

Layer 4 — Interface & Reporting
Presents results in real time and exports usable outputs. It includes:

metric panels and warnings

TAM role display

origin trace and chain observations

clinical interpretation (technical)

client explanation (plain language)

session logging, baseline comparison, and report export

Design Principles

deterministic processing (no drift)

separation of measurement vs interpretation

fail-safe frame gating and pose locking

reproducible outputs via baseline comparison

clinically interpretable structure

This architecture allows the system to clearly distinguish:

where structure is failing

where compensation is occurring

where stability is being preserved

and to do so consistently across frames, sessions, and users.
