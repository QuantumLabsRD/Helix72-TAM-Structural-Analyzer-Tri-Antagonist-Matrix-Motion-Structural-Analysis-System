Reproducibility & Baseline System — Description

Purpose

The Baseline & Reproducibility System ensures that Helix72 TAM outputs are repeatable, comparable, and clinically trackable across time.

It answers:

did the structure actually change?

is the system reading consistently?

is the intervention producing measurable improvement?

Baseline Capture

A baseline is a frozen reference state of the subject.

Captured data includes:

full metric set

TAM roles

Helix state

chain integrity

origin node

propagation path

corridor states

COM values

certainty level

Rule:
Baseline must be captured under stable pose + high confidence.

Baseline Load

When a baseline is loaded, the system:

locks reference values

enables delta comparison

switches UI into comparison mode

Delta Comparison

The system compares current frame vs baseline across:

Metrics

joint angles

collapse deviations

COM shift

corridor breach

Structural State

static state change

dynamic state change

Helix state change

TAM Roles

driver shift

counterforce change

stabilizer state change

anchor relocation

Origin & Propagation

origin node change

propagation path change

compensation shift

Reproducibility Engine

Evaluates whether two states are structurally consistent.

It does not rely only on raw numbers.

It compares:

structural pattern

role consistency

origin stability

propagation agreement

corridor alignment

chain integrity

Reproducibility Outputs

PASS

structure matches baseline

minimal variation

CAUTION

moderate variation

partial mismatch

FAIL

significant structural difference

pattern breakdown

Reproducibility Score Factors

Weighted inputs:

metric similarity

role consistency

origin agreement

propagation agreement

corridor agreement

pose confidence

contradiction presence

Clinical Use
Before / After Treatment

capture baseline (pre)

perform treatment

capture post

compare improvement

Progress Tracking

compare across sessions

identify consistent patterns

validate treatment effectiveness

System Validation

confirm readings are stable

detect noise vs real change

Baseline Integrity Rules

must use same camera position

same stance setup

similar lighting

similar clothing visibility

high pose confidence

Violation of these reduces reproducibility reliability.

What Reproducibility Means

PASS ≠ perfect posture

FAIL ≠ bad outcome

It means:

PASS → consistent structure

FAIL → structure changed

Interpret change clinically.

Baseline Metadata

Each baseline stores:

timestamp

pose confidence

frame index

environment context

system state

UI Behavior

When baseline mode is active:

delta values displayed

changes highlighted

role shifts shown

origin shifts shown

Freeze Interaction

Baseline works best with:

freeze mode ON

stable frame

no motion interference

Key Principle

Reproducibility is not about identical numbers.

It is about:
consistent structural patterns over time

Purpose in System

This system ensures:

trust in readings

measurable progress

objective comparison

Final Insight

Baseline + reproducibility turns the analyzer from:
a scanner

into:
a tracking and validation system
