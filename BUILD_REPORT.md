# BUILD REPORT — MambaLab (2026-05-23)

## Project
**MambaLab** — Interactive State Space Models & Selective Scan Laboratory

## Links
- **Live:** https://mambalab-three.vercel.app
- **GitHub:** https://github.com/middesurya/daily-webapp-2026-05-23-mambalab

## Idea Source
- **Trend:** Mamba-3 published at ICLR 2026, establishing new Pareto frontier for SSM quality-efficiency tradeoff
- **Gap:** 40+ existing "Lab" projects covering topics from quantum error correction to information geometry — but NO interactive SSM/Mamba explorer exists anywhere
- **Bay Area relevance:** Albert Gu (CMU→Cartesia AI) and Tri Dao (Stanford→Together AI) are Bay Area researchers; SSMs are a major architectural paradigm shift

## Scoring
| Criterion | Weight | Score | Weighted |
|-----------|--------|-------|----------|
| Novelty | 3× | 9 | 27 |
| Feasibility | 3× | 8 | 24 |
| Wow Factor | 2× | 9 | 18 |
| Learning Value | 2× | 10 | 20 |
| Utility | 1× | 8 | 8 |
| **Total** | | | **97/110** |

## Modules Built
1. **HiPPO & S4 Kernel Engine** — Matrix heatmaps, eigenspectrum analysis, convolutional kernel visualization with 3 discretization methods
2. **Selective Scan Simulator** — Fixed vs selective SSM comparison on 3 tasks with parameter dynamics visualization
3. **Sequence Modeling Arena** — SSM vs Transformer vs RNN training comparison on 4 diagnostic tasks
4. **Long-Range Dependency Explorer** — O(N) vs O(N²) scaling charts, memory comparison, Pathfinder task
5. **Mamba Architecture Explorer** — Mamba/Mamba-2/Mamba-3 block diagrams with parameter estimator
6. **SSM Evolution Timeline** — HiPPO→LSSL→S4→S4D→H3→Mamba→Mamba-2→Mamba-3 with Pareto frontier chart

## Technical Decisions
- **Single HTML file, zero dependencies** — consistent with lab series
- **Canvas-based rendering** — fast, no DOM manipulation overhead
- **Pure JS matrix math** — matrix multiplication, exponential (Padé approximation), eigenvalue estimation (Gershgorin circles)
- **Simulated training curves** — based on published benchmark results from papers, not live training

## Lessons Learned
- Matrix exponential via Taylor series needs sufficient terms (12) and squaring for stability
- Gershgorin circle theorem provides useful eigenvalue bounds for visualization without full eigendecomposition
- SSM parameter counts differ significantly across Mamba generations (MIMO in Mamba-3 doubles complex state)

## Build Stats
- **Lines of code:** ~2100 (HTML+CSS+JS)
- **File size:** 84 KB
- **Build time:** Single session
- **Deployment:** Vercel (static)
