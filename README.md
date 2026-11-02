<div align="center">

<img width="1200" height="475" alt="Keep the Future Human Banner" src="https://github.com/user-attachments/assets/0aa67016-6eaf-458a-adb2-6e31a0763ed6" />

# Keep the Future Human — Appendix Explainer

An interactive educational companion and policy simulator based on Anthony Aguirre's essay advocating for **Tool AI**, strict compute governance, and existential AI safety.

[![React](https://img.shields.io/badge/React-19.2-61DAFB?style=flat-square&logo=react&logoColor=black)](https://react.dev/)
[![TypeScript](https://img.shields.io/badge/TypeScript-5.8-3178C6?style=flat-square&logo=typescript&logoColor=white)](https://www.typescriptlang.org/)
[![Vite](https://img.shields.io/badge/Vite-6.2-646CFF?style=flat-square&logo=vite&logoColor=white)](https://vitejs.dev/)
[![Tailwind CSS](https://img.shields.io/badge/Tailwind_CSS-3.x-38B2AC?style=flat-square&logo=tailwind-css&logoColor=white)](https://tailwindcss.com/)
[![Framer Motion](https://img.shields.io/badge/Framer_Motion-12.x-black?style=flat-square&logo=framer&logoColor=white)](https://www.framer.com/motion/)

[View in AI Studio](https://ai.studio/apps/drive/1qJXBTe3feqGsQqTHWi5f8ENinh09cUgX) · [Report an Issue](https://github.com/coolbros/keep-the-futurehuman-Appendix-Explainer/issues)

</div>

---

## 📖 Table of Contents

- [Overview](#-overview)
- [Key Features](#-key-features)
  - [The Core Narrative](#the-core-narrative)
  - [Interactive Technical Appendices](#interactive-technical-appendices)
- [Tech Stack](#-tech-stack)
- [Getting Started](#-getting-started)
  - [Prerequisites](#prerequisites)
  - [Installation & Local Run](#installation--local-run)
  - [Building for Production](#building-for-production)
- [Project Architecture](#-project-architecture)
- [Conceptual Background & Reference](#-conceptual-background--reference)
- [License](#-license)

---

## 🔭 Overview

> *"We can cure diseases and solve physics with AI that remains under meaningful human control. We don't need to build a new species to solve our problems."*
> — **Anthony Aguirre**

**Keep the Future Human — Appendix Explainer** is an interactive, responsive web application designed to translate high-stakes AI safety theory, technical compute accounting, and regulatory governance into intuitive, visual experiences.

Rather than treating Artificial General Intelligence (AGI) as an inevitable evolutionary successor to humanity, the project visualizes a pragmatic third path: **Tool AI**. By restricting compute thresholds, establishing strict legal liability, and closing the gate on unconstrained autonomous agents, humanity can harness the transformative benefits of AI while maintaining human control.

---

## ✨ Key Features

### The Core Narrative

* **Hero & Thesis:** An atmospheric introduction illustrating the open "Gate" to uncontrolled superintelligence and the case for deliberate restraint.
* **The Problem of Convergence (Interactive Venn Diagram):** Explores how the lethal intersection of **High Intelligence**, **Autonomy**, and **Generality** transforms software from a helpful tool into a species-level threat.
* **Species-Level Risks:** Interactive breakdown of existential risk categories:
  * *Loss of Control:* Inability to steer systems smarter and faster than humans.
  * *Societal Disruption:* Erosion of economic and institutional trust.
  * *Geopolitical Instability:* Uncontrollable automated cyberwarfare and arms races.
* **The Blueprint (Governance Timeline):** A sequential roadmap detailing the pillars of non-proliferation:
  1. *Compute Accounting:* Tracking high-end GPUs like enriched nuclear material.
  2. *Hard Compute Caps:* Global speed limits on training runs ($10^{27}$ / $10^{25}$ FLOP limits).
  3. *Strict Legal Liability:* Eliminating negligence loopholes for model creators.
  4. *Hardware Security:* Cryptographic controls and remote kill-switches.
* **The Third Path (Tool AI vs. Agentic AGI):** An interactive split-screen comparison illustrating how bounded, auditable Tool AI delivers scientific breakthroughs without the catastrophic tail risks of agentic AGI.

---

### Interactive Technical Appendices

The heart of the application is an interactive simulator suite translating the essay's formal technical appendices into hands-on tools:

| Appendix | Simulator | Description |
| :--- | :--- | :--- |
| **Appendix A** | **Compute Scale Simulator** | Interactive FLOP exponent slider ($10^{20}$ to $10^{30}$ FLOPs) benchmarking runs against GPT-3, GPT-4, the proposed Regulatory Gate Threshold ($10^{25}$ FLOPs), Gemini Ultra, and human brain equivalents. |
| **Appendix B** | **Closing the Gate** | Step-by-step policy simulator showing the progression from an unrestricted arms race to a US pause, hardware reporting, international bilateral treaties, and an enforced global verification regime. |
| **Appendix C** | **The Liability Judge** | Legal scenario builder testing combinations of autonomy, generality, and harm severity to demonstrate when developers face **Strict Liability** versus **Safe Harbor** protections. |
| **Appendix D** | **Risk Tier Classifier** | Evaluator categorizing models from **RT-0** (Weak/Narrow AI) through **RT-4** (Prohibited Superintelligence Candidate) based on multidimensional capabilities and compute thresholds. |

---

## 🛠 Tech Stack

* **Framework:** [React 19](https://react.dev/)
* **Build Tool:** [Vite 6](https://vitejs.dev/)
* **Language:** [TypeScript](https://www.typescriptlang.org/)
* **Styling:** [Tailwind CSS](https://tailwindcss.com/)
* **Animations:** [Framer Motion](https://www.framer.com/motion/)
* **Icons:** [Lucide React](https://lucide.dev/)

> **Note:** This is a 100% client-side application. No external database, backend server, or API keys (e.g. Gemini API) are required to run it.

---

## 🚀 Getting Started

### Prerequisites

* [Node.js](https://nodejs.org/) (version 18.0.0 or higher recommended)
* `npm`, `pnpm`, or `yarn`

### Installation & Local Run

1. **Clone the repository:**
   ```bash
   git clone https://github.com/coolbros/keep-the-futurehuman-Appendix-Explainer.git
   cd keep-the-futurehuman-Appendix-Explainer
   ```

2. **Install dependencies:**
   ```bash
   npm install
   ```

3. **Start the local development server:**
   ```bash
   npm run dev
   ```

4. Open your browser and navigate to `http://localhost:5173` (or the URL shown in your terminal).

### Building for Production

To create an optimized production bundle:

```bash
npm run build
```

Preview the production build locally:

```bash
npm run preview
```

---

## 📂 Project Architecture

```
keep-the-futurehuman-Appendix-Explainer/
├── components/
│   ├── ui/
│   │   └── SectionWrapper.tsx    # Scroll & responsive layout container
│   ├── AppendixExplorer.tsx      # Interactive simulators for Appendices A-D
│   ├── Comparison.tsx            # Tool AI vs. Autonomous AGI interactive split
│   ├── Footer.tsx                # Citations, download links & credits
│   ├── GovernanceTimeline.tsx    # 4-stage governance roadmap
│   ├── Hero.tsx                  # Interactive gate animation & thesis
│   ├── Risks.tsx                 # Risk category breakdown
│   └── VennDiagram.tsx           # Interactive convergence diagram
├── App.tsx                       # Main application composition
├── index.html                    # HTML entry point, Tailwind config, & fonts
├── index.tsx                     # React DOM entry point
├── package.json                  # Dependencies and scripts
├── tsconfig.json                 # TypeScript compiler configuration
├── types.ts                      # Shared TypeScript interfaces & enums
└── vite.config.ts                # Vite build configuration
```

---

## 📚 Conceptual Background & Reference

* **Original Essay:** *"Keep the Future Human"* by [Anthony Aguirre](https://en.wikipedia.org/wiki/Anthony_Aguirre) (Cosmologist, physicist, and Co-Founder of the [Future of Life Institute](https://futureoflife.org/)).
* **Key Concept:** **Tool AI vs. Agentic AGI** — advocating for the deliberate choice to develop AI as powerful, controllable cognitive tools rather than autonomous, self-directing artificial species.
* **Governance Framework:** Implementing verifiable hardware telemetry, global compute tracking, and legal accountability analogous to nuclear non-proliferation regimes.

---

## 📄 License

This project is open-source. Please refer to the repository's license file or contact the maintainers for reuse guidelines.
