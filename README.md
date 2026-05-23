# MambaLab — Interactive State Space Models & Selective Scan Laboratory

An interactive, zero-dependency web laboratory for exploring **State Space Models (SSMs)** — from the foundational S4 architecture through Mamba's selective scan mechanism to the latest **Mamba-3** complex-valued MIMO formulation (ICLR 2026).

## Modules

### 1. HiPPO & S4 Kernel Engine
Visualize HiPPO matrices (LegS, LegT, LagT), eigenspectra, and convolutional kernels. Explore how structured initialization enables long-range memory and how discretization methods (ZOH, bilinear, Euler) affect the discrete-time system.

### 2. Selective Scan Simulator
Interactive comparison of fixed SSM (S4-style) vs selective SSM (Mamba-style). Watch how input-dependent Δ, B, C parameters allow the model to dynamically gate information flow based on content relevance.

### 3. Sequence Modeling Arena
Train and compare SSM, Transformer, and RNN on diagnostic tasks: Selective Copy, Induction Heads, Associative Recall, and Adding Problem. Real-time training curves reveal each architecture's strengths and weaknesses.

### 4. Long-Range Dependency Explorer
Visualize O(N) vs O(N²) scaling with interactive complexity charts, memory usage comparisons, and a Pathfinder-style visual task demonstrating where SSMs outperform Transformers.

### 5. Mamba Architecture Explorer
Build and compare Mamba/Mamba-2/Mamba-3 block architectures with interactive parameter configuration, FLOP estimation, and component-level architectural diagrams.

### 6. SSM Evolution Timeline
Interactive timeline from HiPPO (2020) through Mamba-3 (ICLR 2026) with key innovations, mathematical formulations, and a quality-vs-efficiency Pareto frontier chart.

## Technical Details

- **Zero dependencies** — single HTML file with inline CSS/JS
- **Pure JavaScript math** — matrix operations, eigendecomposition, SSM simulation
- **Canvas-based visualizations** — heatmaps, curves, architecture diagrams
- **Dark theme** — consistent with the lab series

## Key References

- Gu et al., "HiPPO: Recurrent Memory with Optimal Polynomial Projections" (NeurIPS 2020)
- Gu et al., "Efficiently Modeling Long Sequences with Structured State Spaces" (ICLR 2022)
- Gu & Dao, "Mamba: Linear-Time Sequence Modeling with Selective State Spaces" (2023)
- Dao & Gu, "Transformers are SSMs: Generalized Models and Efficient Algorithms Through Structured State Space Duality" (ICML 2024)
- Gu, Dao et al., "Mamba-3: Improved Sequence Modeling using State Space Principles" (ICLR 2026)

## License

MIT — Built autonomously by [Surya Midde](https://github.com/middesurya) with Claude Code.
