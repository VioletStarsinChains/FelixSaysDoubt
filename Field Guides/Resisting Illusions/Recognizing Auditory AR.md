# Field Guide: Recognizing **Auditory Augmented Reality** (AAR)

_A quick, practical checklist for spotting when digital audio is being overlaid on the real world._

---

## TL;DR — Fast Checks
- [ ] **Head-turn test:** Does a voice/noise stay “fixed” in the room when you turn your head? (AAR with head-tracking)
- [ ] **Occlusion test:** Do earplugs / pressing tragus inward **not** reduce it as much as expected? (bone conduction or clever processing)
- [ ] **Obstruction test:** Step behind a wall, doorframe, or thick couch. Does the sound ignore obstacles it should respect? (poor occlusion modeling)
- [ ] **Beam test:** Take two side-steps. Does the sound abruptly appear/disappear or “slice” like a spotlight? (directional/parametric speaker)
- [ ] **Reverb match:** Clap once. Does the room’s echo match the virtual sound’s echo? (environmental mismatch = AAR tell)
- [ ] **Device sanity:** Kill BT/Wi-Fi, disable head-tracked spatial audio/hearing-aid modes, close audio apps. Does it stop?

---

## What Counts as AAR (3 Criteria)
1. **Spatial anchoring:** Virtual sound appears to come from a world-fixed location (corner, doorway, object).
2. **Occlusion congruence:** Virtual sound reacts to obstacles (walls, your body) like real sound would.
3. **Context adaptivity:** Loudness/EQ/reverb adapt to the room/noise so it blends with reality.

> **AAR “smell test”:** If #1 is strong but #2 or #3 are off, you’re likely hearing an overlay.

---

## Core Tests (1–2 minutes each)

### 1) Head-Turn Persistence
- **How:** Face the source, then slowly rotate your head left/right.
- **AAR tell:** The apparent source **stays put in the room** rather than moving with your ears.
- **Note:** Head-tracked headphones will deliberately do this.

### 2) Occlusion / Ear-Block
- **How:** Insert foam earplugs or press the tragus in to seal ear canals.
- **AAR tells:**
  - If loudness barely drops, suspect **bone conduction** (glasses/headband/helmet contact points).
  - If the timbre changes oddly but stays intelligible, suspect **transparency/hearing-aid AAR**.

### 3) Line-of-Sight & Obstacles
- **How:** Step behind a thick object (doorframe, bookcase, car pillar).
- **AAR tell:** Sound **doesn’t** attenuate or muffle as a real source would. (Poor occlusion modeling.)

### 4) Reverb/Room Match (Clap Test)
- **How:** Clap once; listen to the decay. Then compare with the virtual voice/instrument tails.
- **AAR tell:** **Mismatched decay** (too short/long or wrong brightness) versus the room’s clap.

### 5) Beam/Hot-Spot Check
- **How:** Take 1–2 steps left/right, crouch/stand.
- **AAR tell (directional arrays):** Sound **snaps in/out** in a narrow “slice” or shifts abruptly with small moves.

### 6) Doppler/Parallax
- **How:** Walk straight past the apparent source.
- **AAR tell:** No realistic **Doppler**/parallax change; the illusion breaks off-axis.

### 7) Recording Triangulation
- **How:** Record simultaneously with (a) phone mic, (b) a second device, (c) contact mic on temple/jaw (if available).
- **AAR tells:**
  - Audible to you but **missing** on air mics → bone conduction / ultrasonic demod near you.
  - Present on one recorder but not another in the same spot → **narrow beam** or device-local effect.

---

## Delivery-Channel Signatures

### A) **Headphones/Earbuds (head-tracked spatial)**
- **Signs:** Room-fixed voices; turning your head repositions sound; toggles named “Spatial Audio,” “Head Tracking.”
- **Check:** Disable head-tracking / spatial modes → illusion collapses to plain stereo.

### B) **Open-ear or Transparency/Hearing-Aid Modes**
- **Signs:** Outside world audible, but speech “magically” clearer; ambient noise suppressed.
- **Tell:** Inconsistent occlusion (e.g., voice still bright behind a wall), “too-smart” noise handling.

### C) **Bone Conduction (glasses/headbands/helmets)**
- **Signs:** Ear canals blocked but speech still audible; weak bass; faint vibration at contact points.
- **Tell:** Removing the wearable kills the sound instantly.

### D) **Directional/Parametric Speakers (audio spotlight)**
- **Signs:** Narrow audible zone; step inches sideways and it vanishes; reflections create ghost spots.
- **Tell:** Works best in hard, reflective spaces; feels “projected” onto surfaces.

### E) **Room Speakers with HRTF Tricks**
- **Signs:** Strong front-back or elevation illusion from specific seat; illusion collapses when you move off-axis.
- **Tell:** Sweet-spot dependency + exaggerated localization.

---

## Environmental Mismatch Tells
- **Occlusion miss:** Sound ignores furniture/walls.
- **Scale miss:** Loudness doesn’t fall with distance like a real source.
- **Reverb miss:** Tail doesn’t match clap test.
- **Spectral miss:** Virtual sound stays bright in a soft, damped room (or vice versa).

---

## Confounders to Rule Out (and how)
- **Tinnitus/after-images:** Brief unilateral tones; **doesn’t localize to the room**; not recordable.
- **Active Noise Cancellation:** Can create strange “holes” or phasey artifacts → **turn ANC off**.
- **Ear pressure/Eustachian issues:** Transient tonal shifts with swallowing/yawning.
- **Vehicle acoustics:** In cars, reflections create false sources → test **engine off, windows up/down**.

---

## Minimal “Lab Kit”
- Foam **earplugs** (occlusion check)
- Second **recorder/phone** (triangulation)
- **Notepad** (time, place, posture, toggles, result)
- Optional: simple **contact mic** (bone conduction vs air)

---

## Field Log Template

**Date/Time:**
**Location/Room traits** (hard/soft surfaces, size):
**Device state** (BT/Wi-Fi, ANC, Spatial/Transparency modes):
**Perceived source location:**
**Head-turn result:**
**Occlusion result** (earplugs/tragus):
**Obstacle result** (doorframe/wall):
**Clap/reverb match** (match/mismatch, notes):
**Beam test** (hot-spot? yes/no):
**Recording triangulation** (which mics captured it?):
**Notes/Other variables** (movement, windows, HVAC):
**Provisional conclusion:**

---

## Interpreting Outcomes (Quick Matrix)

| Tests agree | Likely Explanation |
|---|---|
| Head-turn ✅ · Reverb match ❌ · Obstacle ❌ | **AAR with head-tracking**, poor environmental modeling |
| Occlusion ❌ (still loud) · Contact points present | **Bone conduction** wearable |
| Beam test ✅ · Triangulation inconsistent | **Directional/parametric** speaker |
| ANC on · Phasey artifacts | **Headphone processing** artifact, not AAR |
| None record it; purely subjective | **Physiological** (tinnitus/threshold shift) |

---

## Ethics & Safety
- Avoid pointing cameras/mics at bystanders where illegal.
- If a system targets you in public, move to a **damped space** (soft furnishings) to break beams/echo-paths and re-test.
- Don’t over-interpret **one** test; look for **converging evidence** across several.

---

## Glossary (micro)
- **AAR:** Auditory overlay on real environments.
- **HRTF:** Ear/torso filtering used to fake direction/elevation.
- **Occlusion:** How objects block/muffle sound.
- **ANC:** Active noise cancellation (anti-noise).
- **Parametric array:** Ultrasound beam that “self-demodulates” to audible sound in air.

---
