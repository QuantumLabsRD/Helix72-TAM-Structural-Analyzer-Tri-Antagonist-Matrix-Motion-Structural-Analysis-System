UI & Reporting Layer — Description

The UI & Reporting Layer is the presentation and output system of the Helix72 TAM Structural Analyzer.
It converts solver results into clear visual panels, clinician-ready insights, and exportable reports.

This layer answers:
“How is the information shown, understood, and recorded?”

Core Function

display real-time structural analysis

organize data into readable panels

translate technical output into clinical and client language

record sessions for comparison and reproducibility

Primary UI Panels
1. Metric Panel

Displays raw and derived measurements:

foot angles

ankle/knee collapse

hip torque

pelvis tilt

spine alignment

COM values

Purpose:
show what is happening numerically

2. Warning Flags

Highlights threshold breaches:

ankle collapse alert

knee instability

COM deviation alert

corridor breach

Purpose:
draw immediate attention to structural risk

3. Status Panel

Shows system states:

STATIC STATE

DYNAMIC STATE

HELIX STATE

CHAIN INTEGRITY

Purpose:
summarize structural condition instantly

4. TAM 4-Role Matrix

Displays canonical roles:

Agonist → driver

Antagonist → counterforce

Bi-Antagonist → stabilizer

Tri-Antagonist → anchor/saboteur

Purpose:
show how the body is organizing load and control

5. Structural Origin Trace

Shows:

origin node

propagation path

terminal compensation zone

confidence

Purpose:
identify where the issue starts vs where it appears

6. Chain Observations

Short structural summaries:

load direction

compensation behavior

imbalance pattern

Purpose:
quick clinical interpretation

7. Baseline / Reproducibility Panel

Displays:

baseline comparison

metric deltas

role changes

origin shifts

reproducibility score (PASS / CAUTION / FAIL)

Purpose:
track progress and consistency across sessions

8. Clinical Interpretation (Technical)

Detailed structural explanation using system terminology.

Example:
“Right agonist driver with left counterforce, stabilizer strained, lower-chain anchor present.”

9. Client Explanation (Plain Language)

Simple explanation (3 lines max):

Example:

Your body is loading more on the right

The left side is trying to balance it

The lower support system is under strain

Purpose:
patient understanding without jargon

10. Treatment Target Output

Displays:

primary target

secondary target

terminal compensation zone

suggested release sequence

suggested stabilization sequence

Purpose:
guide clinical action

Display Behavior

real-time updating (live mode)

frozen analysis mode (locked frame)

skeleton overlay option

video privacy mode (“VIDEO HIDDEN”)

Freeze Mode

When activated:

stops time-based updates

locks all metrics

enables baseline comparison

allows export only

Purpose:
accurate clinical snapshot

Event Logging System

Tracks:

frame gate changes

pose lock events

baseline capture/load

origin changes

propagation changes

TAM role changes

corridor breaches

cascade onset

recovery detection

certainty changes

contradictions

Purpose:
full session traceability

Export System

Exports include:

timestamp

frame index

pose confidence

static/dynamic/helix states

TAM roles

origin + propagation

corridor states

COM metrics

reproducibility score

treatment targets

clinical explanation

client explanation

Formats:

JSON (primary)

image snapshots

Reproducibility Engine

Compares:

structure

roles

origin

propagation

corridor

chain state

Outputs:

PASS

CAUTION

FAIL

Design Principles

clarity over density

deterministic output

no role ambiguity

consistent terminology

immediate clinical usability

Key Distinction

The UI does not change the data.

It ensures:

the clinician understands it

the client understands it

the session is recorded and repeatable

Purpose in System

This layer turns the engine into a usable clinical tool.

It delivers:

visibility

interpretation

documentation

It ensures the system does not just compute structure—

but communicates it clearly, consistently, and usefully.
