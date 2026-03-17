Vector Limitation Notice — Helix72 TAM Structural Analyzer

Overview

The current build of the Helix72 TAM Structural Analyzer includes a known limitation within the foot and ankle vector calculation layer.
This affects how lower-chain alignment and load distribution are derived from 2D pose data.

Affected Metrics

The following outputs may appear inflated, overly sensitive, or inconsistent:

ankle collapse deviation

foot angle orientation

foot angle asymmetry

knee projection derived from ankle axis

stance symmetry calculations

certain center-of-mass (COM) projections influenced by foot position

Cause

The current system uses:

heel-to-toe vector

ankle reference point

global axis alignment

These are being interpreted in 2D space without full depth or ground-reaction context, which can introduce:

exaggerated angular readings

misaligned foot reference frames

amplified downstream effects (knee, COM, stance)

Impact on Analysis
Lower Chain

may over-report collapse severity

may misclassify medial vs lateral deviation

may exaggerate asymmetry

Upstream Effects

Because the system propagates structure upward:

knee tracking may appear distorted

hip loading may be slightly biased

COM projections may shift inaccurately

Reliable vs Advisory Data
Reliable (High Confidence)

pelvis tilt and rotation

spine alignment and curvature

shoulder alignment

torso shift

overall load direction

Advisory (Use Caution)

foot angle

ankle collapse

stance symmetry

knee projection linked to ankle axis

Clinical Guidance

When reviewing output:

treat foot/ankle metrics as early signals, not conclusions

confirm findings manually (visual + palpation)

prioritize upper-chain confirmation before acting on lower-chain alerts

avoid over-correcting based solely on ankle/foot readings

System Behavior

The limitation does not prevent detection of:

asymmetry

instability patterns

compensation chains

It only affects the precision of lower-chain magnitude and classification.

Planned Correction

Next upgrade will include:

corrected foot vector reference frame

improved ankle alignment model

corridor-based lower-chain normalization

reduced propagation distortion

better COM anchoring to base of support

Operational Status

Current system remains:

functional

clinically usable

structurally informative

With the understanding that:
lower-chain outputs are preliminary indicators

Key Principle

This is not a system failure.

It is a vector calibration limitation that:

slightly distorts magnitude

does not eliminate pattern detection

Final Note

Until the upgrade is deployed:

Use the system to locate patterns —
not to finalize ankle/foot conclusions.
