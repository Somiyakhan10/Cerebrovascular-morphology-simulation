# Stroke Vessel Morphology Simulation  
Normal vs. Post-Stroke Cerebrovascular Geometry Changes

A simple Python simulation that models and compares the geometric structure of a cerebral blood vessel in **normal (healthy)** and **post-stroke** conditions.  
The project demonstrates two common post-stroke vascular changes:  
- **Stenosis** (localized narrowing of the vessel)  
- **Increased tortuosity** (wavier, more irregular vessel path)

These morphological alterations are critical in stroke research as they influence blood flow resistance, collateral circulation, tissue perfusion, and clinical outcomes.

## Why This Project?
Post-stroke cerebrovascular remodeling (e.g., vessel narrowing, tortuosity increase, altered radius/area) is a key focus in patient-specific modeling and stroke triage using medical imaging.  
This simulation serves as a foundational proof-of-concept for quantifying such changes — inspired by research on automatic vessel segmentation, morphological feature extraction, and predictive modeling in acute ischemic stroke.

Relevant to studies on:
- Cerebrovascular morphology in healthy vs. stroke patients
- Quantitative analysis of post-stroke vessel changes
- Collateral flow assessment and tissue viability prediction

## Features
- Synthetic generation of vessel radius profiles with natural curvature
- Simulation of 50% stenosis in the central segment
- Addition of increased tortuosity via higher-frequency oscillations
- Calculation of two key morphological metrics:
  - Mean cross-sectional area reduction (%)
  - Tortuosity index (arc length / straight length approximation)
- Clear visualizations of radius profiles, area distribution, and metric comparison

## Example Results
- Mean cross-sectional area reduction post-stroke: ~14.8%  
- Tortuosity index:  
  - Normal: ~1.004  
  - Post-Stroke: ~1.128  

![Vessel Radius and Area Profiles](vessel_radius_and_area_profiles.png)  
*Radius profile (top) and cross-sectional area along the vessel (bottom)*

![Morphological Changes Bar Plot](metrics_bar.png)  
*Comparison of area reduction and tortuosity between normal and post-stroke conditions*

## Requirements
- Python 3.x  
- NumPy  
- Matplotlib  

No external datasets or additional libraries needed — fully synthetic.

## How to Run
1. Clone the repository:
   ```bash
   git clone https://github.com/YOUR_USERNAME/stroke-vessel-morphology-simulation.git
   cd stroke-vessel-morphology-simulation
