# Energy Optimization through End-User Behavior and Technology Integration

# Overview

This project models a residential household energy system using linear programming to analyze how end-user behavior and technology integration affect total energy consumption and cost eventually contributing to carbon emission.

We simulate two main contexts:
1. Behavioral Variation – Users may be careless or efficient in how they use lighting and hot water.
2. Technology Setup – Smart sensors automatically reduce unnecessary consumption (e.g. lights turn off in daylight, water heating matches actual use).

The optimization model is built using [Linopy](https://linopy.readthedocs.io/) in Python.

---

# 🔧 Model Components

#✔️ Decision Variables
- `x_light[t]` – Energy used for lighting at time `t`
- `x_water[t]` – Energy used for hot water at time `t`
- `x_total[t]` – Total energy required at time `t`
- `x_grid[t]` – Energy drawn from the grid at time `t`
- (Optional: `x_pv[t]`, `x_batt[t]` for future extensions)

# 📊 Parameters
- `base_light`, `base_water` – Baseline consumption profiles (hourly)
- `β_light`, `β_water` – Behavior multipliers (careless vs. efficient)
- `τ_light`, `τ_water` – Technology efficiency (smart sensors, etc.)
- `price_grid` – Electricity cost per time step (e.g. €/kWh)

---

📈 Objective
Energy Optimization through End-User Behavior and Technology Integration.