# JQIE — Job-Quality Impact Explorer

This repository accompanies the manuscript **"From Retail Scheduling to Supply-Chain Living Wages: An Agent-Based Simulation to Quantify the Business Value of Improving Job Quality for All"** (Zhang & Gaudiano, accepted for publication in *Merits*, MDPI, 2026 — see `Zhang-Gaudiano-2026-Merits-paper.pdf`). It contains the NetLogo simulation model, the simulation output data behind the paper's results, and the final figures and tables as they appear in the manuscript.

## What is JQIE?

The Job-Quality Impact Explorer (JQIE, pronounced "Jackie") is a proof-of-concept agent-based simulation of frontline retail workers. It models how four job-quality inputs — pay level, guaranteed minimum hours, advance scheduling notice, and the ability to swap shifts — shape individual worker satisfaction and behavior (absenteeism, task efficiency), and how those behaviors roll up into company-level financial outcomes such as profit and customer coverage.

The goal is not to produce definitive predictions, but to give organizational leaders, policymakers, and advocates a way to explore how job-quality interventions are likely to affect financial performance under different assumptions — translating a moral case for better jobs into numbers decision-makers can act on.

## Repository contents

```
JQIE-public/
├── JQIE-web.nlogox                          NetLogo model (built for NetLogo 7)
├── Zhang-Gaudiano-2026-Merits-paper.pdf      Manuscript (submitted version)
├── LICENSE                                   MIT license
├── Data-files/                               Raw simulation output behind the paper's results
│   ├── FFFF2TTTT-L.csv                       Main sweep: all 4 JQ factors off → all on,
│   │                                          2 companies × 10 seeded runs per condition
│   ├── FFFF2TTTT-L2.csv                      Independent repeat of the run above, used to
│   │                                          confirm the seeded model reproduces exactly
│   ├── Sat-add-sweep-lists.csv               Satisfaction-decrement sensitivity sweep
│   └── Sat-add-sweep-table.csv               (same sweep, wide/table format)
└── Figures/                                  Figures and tables as published in the paper
    ├── 01-JQIE UI-wide.png                   Model interface
    ├── 02-jqie_profitability_two_panel.svg   Main profitability results (Table 2 data)
    ├── 03-chart_profit.png                   Sensitivity: profit gap
    ├── 04-chart_coverage.png                 Sensitivity: customer coverage gap
    ├── 05-chart_laborcost.png                Sensitivity: labor cost gap
    ├── 06-jqie_decomposition.svg             Decomposition of the profit gap by JQ factor
    ├── 07-jqie_productivity_paradox.svg      The "productivity paradox" result
    ├── T1-jqie-parameters-table.svg          Table 1: model structural parameters
    ├── T2-jqie-profit-table.svg              Table 2: profit / effect-size (Cohen's d) results
    └── T3-jqie-isolating-factors-table.svg   Table 3: isolating individual JQ factors
```

## Running the model

The model requires **NetLogo 7** (it will not open correctly in earlier NetLogo versions). You can download NetLogo from the [NetLogo home page](https://www.netlogo.org/). Open `JQIE-web.nlogox` in NetLogo and use the interface and BehaviorSpace experiments to run and reproduce simulation sweeps. The `Data-files/` CSVs were generated from BehaviorSpace runs of this model using fixed random seeds, so re-running the same experiment configuration reproduces the same output.

## Manuscript status

The paper has been **accepted for publication** in *Merits* (MDPI). The included PDF is the accepted version; it has not yet been assigned a final DOI. This README and the citation below will be updated with the DOI once it is issued.

## Citation

If you use this model or data, please cite:

> Zhang, C. & Gaudiano, P. (2026). *From Retail Scheduling to Supply-Chain Living Wages: An Agent-Based Simulation to Quantify the Business Value of Improving Job Quality for All.* Merits, MDPI. [DOI to be added upon publication.]

## License

Released under the MIT License — see `LICENSE`.
