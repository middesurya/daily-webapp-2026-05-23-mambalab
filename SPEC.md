# MambaLab — Interactive State Space Models & Selective Scan Laboratory

## Overview
MambaLab is an interactive, zero-dependency web laboratory for exploring State Space Models (SSMs), from the foundational S4 architecture through Mamba's selective scan mechanism to the latest Mamba-3 complex-valued MIMO formulation. Built as a single HTML file with inline CSS/JS.

## Why This Matters
State Space Models represent one of the most significant architectural innovations challenging the Transformer paradigm. Mamba-3, published at ICLR 2026, establishes a new Pareto frontier on performance-efficiency axes. Yet there is NO interactive tool for exploring these concepts hands-on.

## Modules

### 1. HiPPO & S4 Kernel Engine
- Visualize HiPPO matrices (LegS, LegT, LagT) and their eigenspectra
- Continuous-to-discrete SSM conversion (ZOH, bilinear, Euler)
- Convolutional kernel visualization for different sequence lengths
- Show how structured initialization (HiPPO) vs random dramatically changes performance

### 2. Selective Scan Simulator
- Interactive Mamba selective scan mechanism
- Input-dependent Δ (step size), B (input matrix), C (output matrix) parameters
- Side-by-side comparison: fixed SSM vs selective SSM on the same sequence
- Visualize how the model "focuses" on relevant tokens

### 3. Sequence Modeling Arena
- Compare SSM vs Transformer vs RNN on toy benchmark tasks
- Tasks: Selective Copy, Induction Heads, Associative Recall
- Real-time training curves and accuracy metrics
- Show where SSMs excel (long-range) vs struggle (in-context learning)

### 4. Long-Range Dependency Explorer
- Pathfinder-style visual task (trace a path in a 2D grid)
- Adjustable sequence length (1K → 16K tokens)
- Demonstrate SSM's linear scaling vs Transformer's quadratic
- Memory and compute cost visualizations

### 5. Mamba Architecture Explorer
- Build and visualize Mamba/Mamba-2/Mamba-3 block architectures
- Interactive component diagram: conv1d → SSM → gating → output
- Mamba-3 innovations: complex-valued states, MIMO formulation
- Parameter count and FLOP estimator

### 6. SSM Evolution Timeline
- Interactive timeline: S4 → S5 → H3 → Hyena → Mamba → Mamba-2 → Mamba-3
- Key innovation at each step with mathematical formulation
- Performance comparison charts across benchmarks
- Architectural diff view between generations

## Technical Stack
- Single HTML file, zero dependencies
- Canvas-based visualizations
- Pure JavaScript math (matrix ops, eigendecomposition)
- CSS Grid layout, dark theme consistent with lab series

## Scoring
- Novelty: 9/10 (no existing SSM interactive lab)
- Feasibility: 8/10 (complex math but doable in JS)
- Wow Factor: 9/10 (Mamba is THE hot topic)
- Learning Value: 10/10 (deep mathematical foundations)
- Utility: 8/10 (useful for researchers and students)
- **Total: 93/110**
