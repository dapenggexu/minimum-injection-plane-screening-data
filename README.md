# Minimum Injection-Plane Screening Data

This repository contains publication-facing processed data corresponding to the numerical results reported in:

> *Minimum Injection-Plane Screening of Irregular Regional LEO Constellations: Exact Circular-Arc Covering, Resource Landscapes, and Performance--Deployment Trade-offs*

Source code is not included.

## Data files

| File | Manuscript correspondence | Supported result |
|---|---|---|
| `data/figure1_arc_model_summary.csv` | Figure 1(a) numerical anchor and Section 5.1 | Previous and corrected default-cell reachable-arc widths, relative width bias, and counts of changed exact covering classifications. |
| `data/figure2_conditioned_landscape.csv` | Figure 2, arc-conditioned population; conditioned resource-landscape table | Exact-covering summaries for 18 spacecraft-count and deployment-resource cells. |
| `data/figure2_uniform_landscape.csv` | Figure 2, uniform population; uniform resource-landscape table | Exact-covering summaries for 45 spacecraft-count and deployment-resource cells. |
| `data/figure3_conditioned_heuristic_summary.csv` | Figure 3 and the arc-conditioned columns of the heuristic-comparison table | Aggregated overestimation, underestimation, and excess-count results for four feasible-cover baselines. |
| `data/figure3_uniform_heuristic_summary.csv` | Figure 3 and the uniform columns of the heuristic-comparison table | Aggregated overestimation, underestimation, and excess-count results for the uniform reference population. |
| `data/figure4_performance_frontiers.csv` | Figure 4 and the default performance-frontier table | Complete evaluated performance frontiers, including infeasible low-`K` rows represented by empty performance fields. |
| `data/table_marginal_p95_improvement.csv` | Section 5.3 | Adjacent-`K` P95 improvements and the largest observed improvement on each evaluated frontier. |
| `data/table_winner_robustness.csv` | Section 5.4 | Arc-model robustness results for six inherited representative solutions. |

## Conventions

- `N`: number of spacecraft.
- `budget_mps`: round-trip velocity budget in m/s.
- `horizon_days`: deployment deadline in days.
- `K_min`: exact minimum injection-plane count within the circular-arc model defined in the manuscript.
- `evaluation_start_offset_sec`: start offset of the evaluation window in seconds; the two windows remain separate.
- P95 and maximum-gap fields are expressed in minutes.
- Empty frontier performance fields indicate that the evaluated set contains no feasible candidate at that allowed plane count; no interpolation is applied.

Candidate identifiers, random seeds, source-control hashes, machine paths, and implementation files have been removed from this publication-facing dataset.

## Citation

Please cite the manuscript above. Complete bibliographic details will be added after publication.
