# Forest Fire Simulator

This project models the spread of forest fires using a 2D grid-based simulation. It incorporates factors such as tree density and wind conditions to analyze and predict high-risk areas, providing actionable insights for forest fire prevention and management strategies.

## Table of Contents
1. [Overview](#overview)
2. [Features](#features)
3. [Setup and Installation](#setup-and-installation)
4. [Usage](#usage)
5. [Simulation Details](#simulation-details)
6. [Analysis and Insights](#analysis-and-insights)
7. [Limitations and Future Work](#limitations-and-future-work)
8. [Contributors](#contributors)

---

## Overview

The Forest Fire Simulator uses a 150x150 grid to represent a forest. Each cell in the grid has a density value representing the amount of fuel available for a fire. Fires spread based on:
- **Tree density**: Higher density increases the probability of fire spread.
- **Wind conditions**: Direction and strength influence fire behavior.

The simulation identifies high-risk areas and evaluates the effectiveness of different fire management strategies.

GitHub Repository: [Forest Fire Simulator](https://github.com/khasochirb/forest_fire_simulator)

---

## Features

- **Fire Spread Modeling**: Simulates fire behavior using the Moore neighborhood approach.
- **Impact of Wind**: Considers the influence of wind direction and strength.
- **Risk Analysis**: Identifies high-risk areas prone to fire spread.
- **Management Strategies**: Evaluates strategies like enhanced surveillance and preemptive control measures.
- **Statistical Insights**: Provides histograms, heatmaps, and confidence intervals to assess strategy effectiveness.

---

## Setup and Installation

### Prerequisites
- Python 3.8 or higher
- Required libraries: `numpy`, `matplotlib`, `seaborn`

### Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/khasochirb/forest_fire_simulator.git
   cd forest_fire_simulator
   ```
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

---

## Usage

1. Configure simulation parameters in `config.py`:
   - Grid size, number of simulation steps, wind conditions, etc.
2. Run the simulation:
   ```bash
   python simulate_forest_fire.py
   ```
3. Visualize results:
   - Use `plot_heatmap.py` to generate heatmaps.
   - Use `analyze_results.py` for statistical analysis.

---

## Simulation Details

- **Grid Size**: Represents a 40 sq. km forest (150x150 cells).
- **Tree Density**: Each cell's density determines the fire spread probability.
- **Wind Conditions**: Randomized direction and strength for each run.
- **Fire Spread Mechanism**: 
  - Moore neighborhood approach evaluates adjacent cells.
  - Probability of spread depends on tree density and wind effects.

---

## Analysis and Insights

1. **Baseline Scenario**: Average burnt cells ≈ 6312.
2. **Enhanced Surveillance**:
   - Focuses on early detection in high-risk areas.
   - Minor reduction in burnt cells (≈ 6236).
3. **Preemptive Control**:
   - Implements firebreaks in high-risk areas.
   - Significant reduction in burnt cells (≈ 4189).

### Key Visualizations
- **Histogram**: Distribution of burnt cells across multiple runs.
- **Heatmap**: Highlights high-risk areas based on simulation results.

---

## Limitations and Future Work

### Current Limitations
- Assumes static tree density and uniform wind across the grid.
- Ignores external factors like topography, human intervention, or changing weather conditions.
- Simplifies fire spread dynamics without accounting for real-world complexities.

### Future Enhancements
- Incorporate dynamic tree density and real-time weather data.
- Simulate the impact of topography and human activities.
- Expand strategy evaluation to include resource optimization.

---

## Contributors

- **Khas Bayar**

Feel free to contribute by submitting issues or pull requests!
