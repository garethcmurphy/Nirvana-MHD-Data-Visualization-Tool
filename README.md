# Nirvana MHD Data Visualization Tool 🌌✨  

This repository provides Python tools to read Nirvana MHD (Magnetohydrodynamics) code files and generate visualizations using Line Integral Convolution (LIC). The tool is designed to explore vector fields and understand the flow structure within the MHD data.

---

## Features ✨  

- **Read Nirvana MHD data files** in standard formats.  
- **Generate LIC visualizations** to depict vector fields.  
- Support for customizable plots to analyze specific regions of interest.  

---

## Prerequisites 🛠️  

- Python 3.8+  
- Required Python libraries:
  - `numpy`
  - `matplotlib`
  - `h5py`
  - `scipy`  

Install dependencies:  
pip install numpy matplotlib h5py scipy  

---

## Installation  

1. Clone the repository:  
git clone https://github.com/your-username/nirvana-mhd-visualization.git  
cd nirvana-mhd-visualization  

2. Install required dependencies:  
pip install -r requirements.txt  

---

## Usage 🔧  

1. Load and visualize a Nirvana MHD data file:  
```python
from nirvana_reader import read_mhd_file
from lic_plotter import plot_lic

data = read_mhd_file("example_data.h5")
plot_lic(data["velocity_field"], resolution=500, save_as="lic_plot.png")
