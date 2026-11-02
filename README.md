# Keep the Future Human - Appendix Explainer

An interactive web companion for Anthony Aguirre's essay *Keep the Future Human*. The app visualizes the paper's core arguments around Tool AI, compute governance, and existential risk, and provides interactive simulations for each of the paper's technical appendices (Appendices A through D).

Live app: [AI Studio preview](https://ai.studio/apps/drive/1qJXBTe3feqGsQqTHWi5f8ENinh09cUgX)

## Sections

- **Hero & Thesis:** Introduction to the argument for prioritizing bounded Tool AI over autonomous AGI.
- **Problem of Convergence:** Interactive Venn diagram showing the intersection of high intelligence, autonomy, and generality.
- **Risks:** Overview of loss of control, societal disruption, and geopolitical instability.
- **Governance Blueprint:** Timeline outlining compute accounting, training compute caps, strict developer liability, and hardware-level security.
- **Comparison:** Interactive side-by-side view comparing Tool AI against unconstrained agentic AGI.
- **Technical Appendices:**
  - **Appendix A (Compute Scale):** Slider modeling training compute from 10^20 to 10^30 FLOP against historical models and proposed regulatory thresholds.
  - **Appendix B (The Gate):** Step-by-step simulation of the transition from an unmonitored AI race to an international treaty regime.
  - **Appendix C (Liability Judge):** Scenario tool mapping system autonomy, generality, and harm severity to strict liability vs. safe harbor outcomes.
  - **Appendix D (Risk Classifier):** Categorization tool assigning models to tiers RT-0 through RT-4 based on capability profiles and compute limits.

## Tech Stack

- React 19
- TypeScript
- Vite 6
- Tailwind CSS
- Framer Motion
- Lucide React

The project runs entirely in the browser as a static single-page app. It does not require a backend, database, or API keys.

## Development

### Prerequisites

- Node.js 18 or later
- npm (or yarn / pnpm)

### Setup

1. Clone the repository:
   ```bash
   git clone https://github.com/coolbros/keep-the-futurehuman-Appendix-Explainer.git
   cd keep-the-futurehuman-Appendix-Explainer
   ```

2. Install dependencies:
   ```bash
   npm install
   ```

3. Start the dev server:
   ```bash
   npm run dev
   ```

4. Build for production:
   ```bash
   npm run build
   ```

5. Preview the production build:
   ```bash
   npm run preview
   ```

## Project Structure

```
keep-the-futurehuman-Appendix-Explainer/
├── components/
│   ├── ui/
│   │   └── SectionWrapper.tsx    # Section layout container
│   ├── AppendixExplorer.tsx      # Simulators for Appendices A-D
│   ├── Comparison.tsx            # Tool AI vs. AGI side-by-side
│   ├── Footer.tsx                # Links and attribution
│   ├── GovernanceTimeline.tsx    # Policy roadmap
│   ├── Hero.tsx                  # Landing section
│   ├── Risks.tsx                 # Risk category cards
│   └── VennDiagram.tsx           # Three-circle convergence diagram
├── App.tsx                       # Main page layout
├── index.html                    # Tailwind setup and font imports
├── index.tsx                     # React root
├── package.json
├── tsconfig.json
├── types.ts
└── vite.config.ts
```

## References

- Anthony Aguirre, *Keep the Future Human* (Future of Life Institute).
