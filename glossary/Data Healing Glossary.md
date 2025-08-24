# Glossary of Terms

**Signal Shimmer**  
Low-amplitude, patterned perturbation introduced into a data stream to bias interpretation while preserving readability. Presence of shimmer warrants reduced confidence and **Checksum Review**.

**Checksum**  
A stable baseline of behavior or data used to detect tampering. If the checksum changes, possible interference is assumed.

**Checksum Mismatch**  
A divergence from the established checksum baseline. Treated as tamper-evident and requiring investigation.

**Trust Floor**  
The minimum acceptable confidence threshold for an automated decision. If shimmer is detected, drop to the Trust Floor and defer.

**Calibration Debt**  
Accumulated micro-bias that inflates apparent accuracy but degrades reliability over time.

**Null Test**  
A test where a harmless, non-salient variable is controlled and varied only under suspected interference to detect overfitting.
