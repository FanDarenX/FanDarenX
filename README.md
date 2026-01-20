# Agent Profile — <Your Name / 中文名>
Undergraduate Researcher · Embodied AI / Robotics  
Focus: Grounding perception into decision & control in physical systems

**Keywords:** Embodied Intelligence · Multimodal Perception · Robot Control · Sim-to-Real  
**Looking for:** research internship / summer camp / graduate mentorship

---

## TL;DR (30s for PI)
I study the **Perception–Decision–Control** loop for embodied agents.

- **Multimodal Perception:** open-vocabulary semantic alignment for affect/intent understanding (AffectGPT reproduction & extensions).
- **Physical Control:** modeling + estimation + robust control under disturbance in high-dynamics settings (RoboMaster real-hardware deployment).
- **Goal:** reduce sim-to-real and improve closed-loop reliability with principled abstractions.

**Artifacts:** code · configs · logs · (optional) videos  
**Contact:** <email> · GitHub: <link> · CV: <link> · Google Scholar (if any): <link>

---

## Research Questions
1. **Grounding:** How do semantic representations (vision/language) become actionable motor commands?
2. **Robustness:** How can learning-based modules coexist with classical control under noise, delay, and unmodeled dynamics?
3. **Generalization:** How to move beyond closed-label perception to open-world semantics while keeping real-time feasibility?

---

## System View (Embodied Loop)
Perception provides structured state/goal representations; decision converts them to plans/actions; control executes them under physical constraints.

[World] → Perception → Decision/Planning → Control → Actuation → [World]

I use this loop as the organizing principle of my projects and learning.

---

## Selected Work / Projects

### Project A — Multimodal Perception: AffectGPT (Reproduction + Extension)
**Motivation:** emotion/affect understanding often overfits fixed categories and fails in open settings.  
**Core idea:** align multimodal features with text semantics to support **open-vocabulary** affect modeling.

**What I did**
- Reproduced core pipeline: data preprocessing, model, training & evaluation.
- Implemented CLIP-style semantic alignment for open-vocabulary affect concepts.
- Conducted ablations on representation choices and prompting strategies.

**Evidence**
- Reproduction report: `docs/affectgpt_repro.md`
- Training configs: `configs/affectgpt/*`
- Logs & curves: `runs/affectgpt/*`
- (Optional) Benchmark table & main metrics: `results/affectgpt.csv`

**Keywords:** Transformer · Contrastive Learning · Open-Vocabulary · PyTorch

---

### Project B — Physical Interaction & Control: RoboMaster (Real Hardware)
**Motivation:** high-speed adversarial environments amplify modeling error, disturbance, and sensor noise.  
**Core idea:** combine **modeling + estimation + feedback** into a reliable closed-loop controller.

**What I did**
- Built kinematic/dynamic model (DH parameters; calibration workflow documented).
- Designed cascade PID + feedforward; tuned under real-time constraints.
- Applied Kalman filtering for state estimation under measurement noise.
- Deployed on STM32H7; validated stability under disturbance.

**Evidence**
- Control design notes: `docs/control_notes.md`
- Calibration & identification: `docs/system_id.md`
- Embedded code: `firmware/*`
- Demo video: <video link> (recommended)

**Outcome:** RoboMaster National Second Prize (team) — my role: control/estimation & deployment  
**Keywords:** Control Theory · State Estimation · Embedded · Real-Time

---

## Reproducibility (PI-friendly)
- **Environment:** `environment.yml` / `requirements.txt`
- **Quickstart:**
  - `bash scripts/train_affectgpt.sh`
  - `bash scripts/eval_affectgpt.sh`
- **Results:** `results/` contains tables that match the report.
- **Seeds:** fixed seeds; deterministic flags documented in `docs/repro.md`.

---

## Technical Foundations (only stable competencies)
- **Programming:** C++ (modern), Python
- **Robotics:** ROS2, kinematics, feedback control, state estimation
- **ML:** PyTorch, Transformer-based models, contrastive learning
- **Systems:** Linux, embedded development, real-time constraints

---

## Current Direction (next 3–6 months)
- Close the loop: connect multimodal perception outputs to planning/control interfaces.
- Add robustness studies: latency/noise stress test; sim-to-real evaluation protocol.
- Build a small-scale embodied benchmark: task definition + metrics + baseline.

---

## Publications / Writing (optional but strong)
- Blog / notes: `notes/` (short technical memos; reproducible experiments)
- Reading list: `reading/embodied_ai.md` (papers + my takeaways)

---

## Contact
Email: <email>  
GitHub: <link>  
CV: <link>  
Location: <city> · Available: <time window>
