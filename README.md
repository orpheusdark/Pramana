# Pramana

### Edge-Based Agentic AI for Offline Deepfake Detection & Authenticity Verification

**Team:** Pramana
**Problem Statement:** Agentic AI for Deepfake Detection & Authenticity Verification
**Focus:** Offline, low-power, real-time deepfake detection for field and tactical environments

---

## 1. Problem Overview

Deepfake audio and video present a growing threat to:

* Field operations
* Evidence integrity
* Tactical and intelligence decision-making

In real-world environments:

* Internet access is unreliable or unavailable
* Cloud-based detection introduces latency and risk
* Manual verification is slow and error-prone

Existing solutions focus on detection accuracy in controlled environments but fail to provide **on-device, real-time, autonomous decision support**.

---

## 2. Our Idea: Pramana

**Pramana** (Sanskrit: *valid knowledge / proof*) is an **edge-based agentic AI system** that verifies the authenticity of audio and video content directly on field devices.

Instead of acting as a passive classifier, Pramana functions as an **autonomous agent** that:

* Detects deepfake signals
* Aggregates confidence across multiple modalities
* Decides and recommends actions in real time
* Operates fully offline

---

## 3. What We Are Building (Prototype Scope)

The prototype demonstrates:

* Offline deepfake detection on edge devices
* Audio and video authenticity analysis
* Agent-based confidence aggregation
* Real-time alerts and decision guidance

**Out of scope (intentionally):**

* Cloud-based learning pipelines
* Large-scale deployment infrastructure
* Continuous online retraining

The focus is **feasibility, clarity, and real-world constraints**.

---

## 4. System Architecture

```
Media Input (Camera / Mic / File)
        ↓
Feature Extraction (Audio + Video)
        ↓
Edge Deepfake Detection Models
        ↓
Agent Decision Engine
        ↓
Alert / Tag / Assist Operative
```

All components run **entirely on-device**, without cloud dependency.

---

## 5. Core Components

### 5.1 Media Input Layer

* Live camera feed or recorded video
* Live audio input or audio files
* Designed for smartphones, body-cams, and laptops

---

### 5.2 Feature Extraction

**Video Features**

* Facial landmark consistency
* Temporal artifact detection
* Lip-sync alignment

**Audio Features**

* Spectral anomalies
* Voice consistency across time

Only lightweight features are used to ensure fast edge inference.

---

### 5.3 Deepfake Detection Models

* Pretrained lightweight CNN-based models
* Optimized for edge inference
* Converted to ONNX / TensorFlow Lite formats

The system supports independent audio and video confidence scoring.

---

### 5.4 Agent Decision Engine (Key Innovation)

This layer makes the system **agentic**, not just predictive.

The agent:

* Aggregates audio and video confidence scores
* Applies rule-based reasoning
* Determines response actions autonomously

**Example decision logic:**

* High fake confidence → Immediate alert
* Low confidence → Suggest secondary verification
* Borderline confidence → Flag for manual review

This transforms detection into **operational intelligence**.

---

### 5.5 Response & Assistance Layer

* Visual authenticity warnings
* Confidence explanation for users
* Secure tagging of suspicious media
* Local audit logging for post-operation review

All responses are delivered in real time.

---

## 6. Edge & Offline Design

Pramana is designed for constrained environments:

* No internet dependency
* Low power consumption
* Fast inference (< 1 second per clip)

Optimizations include:

* Model quantization
* Lightweight inference pipelines
* Efficient feature selection

---

## 7. Technology Stack

* Python
* PyTorch / TensorFlow Lite
* OpenCV
* ONNX Runtime
* Android / Desktop edge deployment

All components are built using open-source tools.

---

## 8. Prototype Implementation Plan

| Task                       | Estimated Time |
| -------------------------- | -------------- |
| Data preparation & testing | 5 hours        |
| Model setup & inference    | 8 hours        |
| Edge optimization          | 6 hours        |
| Agent logic implementation | 4 hours        |
| UI & demo integration      | 5 hours        |

**Total:** ~28 hours

---

## 9. Cost & Resources

**Estimated prototype cost:** ₹0 – ₹2,000

Resources required:

* Laptop (GPU optional)
* Smartphone (Android preferred)
* Webcam or phone camera

No paid APIs or infrastructure required.

---

## 10. Use Cases

* Body-cam footage authenticity verification
* Field audio message validation
* Rapid media verification for intelligence teams
* Support for misinformation detection units

---

## 11. Limitations & Risk Mitigation

**Limitations**

* Performance degrades on extreme compression
* New deepfake styles require model updates
* Device hardware capabilities vary

**Mitigation Strategies**

* Multi-signal confidence aggregation
* Periodic model updates
* Human-in-the-loop fallback for low confidence cases

---

## 12. Impact

Pramana enables:

* Faster and safer decision-making
* Trustworthy digital evidence
* Reduced misinformation risk at the source
* Practical deployment in field environments

**Outcome:**
Authenticity verification at the point of action.

---

## 13. Repository Structure (Proposed)

```
pramana/
├── models/
│   ├── audio_detector/
│   └── video_detector/
├── agent/
│   └── decision_engine.py
├── inference/
│   ├── audio_infer.py
│   └── video_infer.py
├── ui/
│   └── alert_interface.py
├── utils/
│   └── preprocessing.py
└── README.md
```

---

## 14. Conclusion

Pramana demonstrates that:

* Deepfake detection can operate offline
* Agentic reasoning improves reliability
* Edge-based verification is practical and scalable

The system is designed for **real-world constraints**, not laboratory conditions.

---
