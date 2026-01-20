# Agent Profile: Qizhen Xuan (轩齐真)

> Undergraduate Researcher | Embodied AI & Robotics  
> Focus: **Perception–Decision–Control Loop in Physical Systems**

---

## 1️⃣ Research Identity

I am an undergraduate student with a strong background in **robotic control systems** and **multimodal learning**.  
My primary interest lies in **Embodied Intelligence**, especially:

- How high-level semantic understanding (vision/language)  
  can be grounded into **low-level robot control**
- How to reduce the **Sim-to-Real gap** via modeling and feedback

> I treat robots not as programs, but as **agents embedded in physics**.

---

## 2️⃣ Core Research Questions

Instead of listing skills, I focus on questions:

- **Perception:**  
  How can robots interpret *open-world* semantic signals beyond closed labels?

- **Decision:**  
  How should representations from perception influence planning or control?

- **Control:**  
  How can classical control (PID/LQR/KF) coexist with learning-based methods?

---

## 3️⃣ Active Research Modules

### 🧠 Module A — Multimodal Perception (AffectGPT)

**Problem:**  
Traditional emotion recognition relies on fixed categories and lacks generalization.

**Approach:**  
- Reproduced **AffectGPT**
- Used **CLIP-style semantic alignment** to enable *open-vocabulary* emotion modeling
- Focused on representation learning rather than downstream classification

**Keywords:**  
`Multimodal Learning` · `Transformer` · `Open-Vocabulary` · `PyTorch`

---

### 🤖 Module B — Physical Interaction & Control (RoboMaster)

**Problem:**  
High-speed, adversarial environments amplify modeling errors and disturbances.

**Approach:**  
- Modeled a **6-DOF manipulator** using DH parameters
- Designed **cascade PID + feedforward control**
- Applied **Kalman filtering** for state estimation under sensor noise
- Deployed on real hardware (STM32H7)

**Outcome:**  
🏆 RoboMaster National Second Prize

**Keywords:**  
`Robotics` · `Control Theory` · `State Estimation` · `Embedded Systems`

---

## 4️⃣ System View: Embodied Intelligence Loop

```text
[ Perception ]
   ↑        ↓
[ World ] ← [ Decision ]
   ↑        ↓
[ Actuation / Control ]
