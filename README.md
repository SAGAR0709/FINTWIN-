# FinTwin: Personal Financial Digital Twin 💹

**FinTwin** is a PC-first, high-fidelity simulation environment designed to bridge the gap between financial intuition and mathematical reality. While most apps track where your money *went*, FinTwin simulates where your money *could go* based on a "Digital Twin" of your financial life.

## 🚀 The Challenge
Most people lack a safe "sandbox" to test high-stakes financial decisions. Decisions like taking an education loan, shifting from savings to aggressive ETFs, or increasing monthly spending are often made in the dark. 

**FinTwin** provides a "Financial Flight Simulator" to test these decisions against 30-year projections, market volatility, and "Black Swan" events before they happen in real life.

---

## 🛠 Tech Stack (Optimized for PC)
* **Frontend:** React.js / Next.js (App Router)
* **Styling:** Tailwind CSS (Fintech Dark Mode)
* **Charts:** Recharts or Chart.js (High-density time-series data)
* **State Management:** React Context API / `useReducer`
* **Math Engine:** Custom Stochastic engine for compounding interest and inflation.

---

## ✨ Key Features

### 1. The "Digital Twin" Engine
Input your current "Baseline" (Net worth, income, debt). The app creates a mirrored "Twin" where you can toggle variables—like a $50k loan or a 10% increase in SIPs—to see a side-by-side 20-year outcome.

### 2. PC-First Mission Control
A high-density dashboard designed for 1080p+ displays.
* **Left Sidebar:** Fixed controls for real-time data input.
* **Center Stage:** Large interactive `recharts` area showing "Baseline" vs. "Twin" trajectories.
* **Right Panel:** "Decision Lab" to inject one-off events (buying a house, career pivot).

### 3. "Black Swan" Stress Testing
A dedicated simulation toggle that injects random, statistically grounded negative events:
* 6-month job loss.
* Market crash (-20% correction).
* Unexpected medical emergency.
* *See which path (Baseline or Twin) is more resilient to failure.*

### 4. Mathematical Rigor
Built-in logic for:
* **Compounding Interest:** $A = P(1 + \frac{r}{n})^{nt}$
* **Loan Amortization:** Real-time debt-reduction visualization.
* **Inflation Drag:** Adjusted "Purchasing Power" views over 30 years.

---

## 📂 Project Structure
```text
├── src/
│   ├── components/
│   │   ├── Dashboard/       # Main Layout (PC Optimized)
│   │   ├── Sidebar/         # Input controls & Sliders
│   │   └── Visualizer/      # Recharts/Chart.js implementation
│   ├── hooks/
│   │   └── useSimulation.ts # The "Digital Twin" logic & math
│   ├── utils/
│   │   └── mathEngine.ts    # Compounding & Amortization formulas
│   └── App.tsx              # Main entry point
