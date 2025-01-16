# **Deterministic Simulation of a 900 MW PWR**

## **Project Description**

This repository contains a series of notebooks and Python scripts dedicated to the deterministic neutron simulation of a 900 MW French Pressurized Water Reactor (PWR). The objective is to provide an educational and practical approach to understanding and implementing diffusion models and numerical solvers applied to neutron physics.

### **Main Content:**
1. **Educational Notebooks:**
   - Introduction to deterministic methods.
   - Simulation of a simplified 1D model and extension to 2D.
   - Presentation of the neutron diffusion equation and its numerical resolution.

2. **Python Scripts:**
   - Solvers for solving discretized equations.
   - Mesh generators for 2D simulations.
   - Visualization tools for results.

3. **Scientific Data:**
   - Multigroup cross sections.
   - Simplified geometric models for a PWR.

---

## **Objectives**

This project aims to:
- Illustrate the operation of deterministic methods for neutron physics.
- Present a clear and reproducible workflow for simulations.
- Provide a base that students, researchers, or engineers can extend to more complex models (e.g., thermal-hydraulic coupling).

---

## **Repository Structure**

```
├── notebooks/
│   ├── 01_Introduction.ipynb        # Theory of deterministic methods
│   ├── 02_Modeling_1D.ipynb         # 1D Simulation (diffusion equation)
│   ├── 03_Modeling_2D.ipynb         # 2D Extension
│   └── 04_Results_Analysis.ipynb    # Analysis and visualization of results
├── src/
│   ├── diffusion_solver.py          # Diffusion equation solver
│   ├── mesh_generator.py            # 2D mesh generator
│   ├── visualization.py             # Visualization tools
├── data/
│   ├── cross_sections.csv           # Neutron data (multigroup)
│   ├── reactor_geometry.json        # Geometry files
├── results/
│   ├── flux_1D.png                  # 1D neutron flux graphs
│   └── flux_2D.png                  # 2D flux visualization
├── README.md                        # Project description
├── requirements.txt                 # Required Python dependencies
├── environment.yml                  # Conda environment file
```

---

## **Usage**

### **Prerequisites:**
- Python 3.8+ with the following libraries:
  - `numpy`, `matplotlib`, `scipy`, `pandas`.

### **Run Simulations:**
1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/simulation-pwr-900mw.git
   cd simulation-pwr-900mw
   ```
2. Install the environment:
   ```bash
   conda env create -f environment.yml
   conda activate simulation-pwr
   ```
3. Explore the notebooks:
   ```bash
   jupyter notebook
   ```

---

## **Contributions**

Contributions to enrich the model (e.g., adding a transport solver, thermal coupling) or improve visualizations are welcome! Feel free to submit an **issue** or a **pull request**.

---

For any questions or suggestions, please contact the repository maintainer. Happy simulating!
