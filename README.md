# Sim2O_supplementary

Table 1. Wall-clock statistics averaged over online training (mean ± std over seeds)

| Environment | Method | act_time | step_time | steps_per_sec |
|---|---|---:|---:|---:|
| Ant-2x4-medium-replay | OMIGA-FT | 0.47 ± 0.01 | 7.42 ± 0.22 | 134.71 ± 4.09 |
|  | AWAC | 0.45 ± 0.00 | 6.30 ± 0.05 | 158.42 ± 1.26 |
|  | PEX | 1.50 ± 0.01 | 8.51 ± 0.09 | 117.38 ± 1.19 |
|  | Sim2O | 2.09 ± 0.02 | 9.14 ± 0.08 | 109.18 ± 0.98 |
| Ant-4x2-medium-replay | OMIGA-FT | 0.47 ± 0.00 | 12.19 ± 0.13 | 81.89 ± 0.88 |
|  | AWAC | 0.44 ± 0.00 | 5.95 ± 0.02 | 167.71 ± 0.67 |
|  | PEX | 1.42 ± 0.01 | 8.11 ± 0.11 | 123.10 ± 1.65 |
|  | Sim2O | 3.45 ± 0.02 | 10.05 ± 0.06 | 99.34 ± 0.56 |
| Ant-8x1-medium-replay | OMIGA-FT | 0.51 ± 0.01 | 13.19 ± 0.39 | 75.72 ± 2.27 |
|  | AWAC | 0.47 ± 0.01 | 6.46 ± 0.18 | 154.56 ± 4.29 |
|  | PEX | 1.51 ± 0.01 | 8.65 ± 0.06 | 115.41 ± 0.77 |
|  | Sim2O | 6.74 ± 0.11 | 13.90 ± 0.21 | 71.85 ± 1.06 |

Table 2. Average episode returns of OMIGA-Finetune after 1 million online steps (mean ± std over 5 seeds).

| Environment | OMIGA-Offline | OMIGA-Finetune | Sim2O |
|---|---:|---:|---:|
| HalfCheetah-6x1-medium | 1992.63 ± 888.20 | 2499.59 ± 47.34 | 3543.84 ± 227.67 |
| HalfCheetah-6x1-medium-replay | 2581.69 ± 91.54 | 710.46 ± 629.25 | 3145.98 ± 109.50 |
| Ant-4x2-medium-replay | 1287.25 ± 22.59 | 1187.17 ± 60.34 | 2024.66 ± 93.21 |
| Ant-8x1-medium-replay | 1346.42 ± 18.04 | 1340.37 ± 21.29 | 1546.51 ± 12.34 |

Table 3. Average episode returns on Ant-8x1-medium-replay after 0.5 million online steps (mean ± std over 3 seeds).

| Method | Episode return |
|---|---:|
| Exhaustive selection | 118.22 ± 5.14 |
| Sim2O | 123.45 ± 6.78 |

Table 4. Average episode returns under different agent orderings after 0.5 million online steps (mean ± std over 3 seeds).

| Ordering | Episode return |
|---|---:|
| Forward | 3539.36 ± 94.19 |
| Reverse | 3623.12 ± 30.28 |
| Random | 3562.66 ± 25.94 |

Table 5. Average episode returns under different offline pretraining steps after 0.5 million online steps (mean ± std over 3 seeds).

| Environment | Offline pretraining steps | Episode return |
|---|---:|---:|
| Ant-4x2-medium-replay | 250000 | 2392.01 ± 682.28 |
|  | 500000 | 1902.65 ± 17.56 |
|  | 1000000 | 1629.69 ± 2.92 |
| HalfCheetah-6x1-medium-replay | 250000 | 3225.29 ± 79.46 |
|  | 500000 | 2360.26 ± 965.24 |
|  | 1000000 | 1686.85 ± 1008.67 |

Table 6. Average episode returns under different temperature τ values after 0.5 million online steps (mean ± std over 3 seeds).

| Environment | τ | Episode return |
|---|---:|---:|
| HalfCheetah-6x1-medium-replay | 1.0 | 3024.89 ± 52.26 |
|  | 5.0 | 3495.16 ± 7.28 |
|  | 10.0 | 3759.66 ± 101.25 |
| Ant-4x2-medium-replay | 1.0 | 1550.10 ± 29.83 |
|  | 5.0 | 1900.82 ± 138.67 |
|  | 10.0 | 1684.00 ± 22.18 |

Table 7. Average episode returns under different replay mixing ratios ρ after 0.5 million online steps (mean ± std over 3 seeds).

| Environment | ρ | Episode return |
|---|---:|---:|
| Ant-4x2-medium-replay | 0.25 | 1735.82 ± 194.43 |
|  | 0.5 | 1809.06 ± 178.69 |
|  | 0.75 | 1517.59 ± 55.55 |
| HalfCheetah-6x1-medium-replay | 0.25 | 2394.11 ± 887.12 |
|  | 0.5 | 1661.54 ± 884.23 |
|  | 0.75 | 2269.06 ± 1156.42 |
