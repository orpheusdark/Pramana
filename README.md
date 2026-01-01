# Pramana

**Edge-Based Agentic AI for Offline Deepfake Detection**

---

## Problem

Deepfake audio and video can mislead:

* Field operatives
* Investigations
* Tactical decision-making

In real deployments:

* Internet access is unreliable
* Cloud-based detection introduces latency
* Manual verification is slow and error-prone

**Current systems detect deepfakes but fail to provide real-time, offline, on-device decision support.**

---

## Idea

**Pramana** (Sanskrit: *valid knowledge / proof*) is an **edge-based agentic AI system** that verifies the authenticity of audio and video directly on field devices.

Instead of acting as a passive classifier, Pramana operates as an **autonomous agent** that:

* Detects deepfake signals
* Aggregates confidence across audio and video
* Decides and assists next actions in real time
* Works fully offline

---

## Solution Overview

Pramana runs entirely on edge devices such as:

* Smartphones
* Body-cams
* Handheld tactical devices

**High-level flow:**

```
Media Input → Feature Analysis → Edge Detection Models → Agent Decision Engine → Alert / Assist
```

No cloud dependency. No external services.

---

## What Makes It Agentic

The system includes a **decision-making agent layer** that:

* Combines multiple detection signals
* Applies confidence-based reasoning
* Autonomously determines the response

Example:

* High confidence fake → Immediate alert
* Low confidence → Secondary verification suggested
* Borderline → Flag for manual review

This converts detection into **operational intelligence**.

---

## Prototype Scope

The prototype demonstrates:

* Offline deepfake detection
* Edge inference on real devices
* Agent-based confidence reasoning
* Real-time alerts

**Out of scope (by design):**

* Cloud learning pipelines
* Large-scale deployment infrastructure

---

## Feasibility

* Runs on consumer hardware
* Uses lightweight, optimized models
* Sub-second inference per clip
* Built with open-source tools

**Estimated build time:** ~28 hours
**Estimated cost:** ₹0 – ₹2,000

---

## Impact

* Improves trust in field-captured media
* Reduces misinformation at the source
* Enables faster, safer operational decisions
* Strengthens digital evidence integrity

---

## Team

**Team Pramana**
*Pramana: Evidence-based verification of digital truth*

---

