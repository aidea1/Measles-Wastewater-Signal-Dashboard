# Measles Wastewater Signal Dashboard

This repository contains an interactive dashboard that visualizes measles wastewater signals across U.S. counties using publicly available data from the Centers for Disease Control and Prevention (CDC).

The dashboard transforms raw wastewater surveillance data into an accessible, county-level visualization to support early detection, situational awareness, and public health decision-making.

Wastewater surveillance is an increasingly valuable tool for monitoring infectious diseases. By aggregating and visualizing these signals geographically and over time, this dashboard helps identify emerging trends and potential hotspots.

## Dashboard at: [Measles Wastewater Signal Dashboard](https://aidea1.github.io/Measles-Wastewater-Signal-Dashboard/)
---

## Data Source

This project uses the CDC’s **Wastewater Data for Measles** dataset.  
**Dataset ID:** `akvg-8vrb`

The dataset includes:

- Facility-level wastewater sample results  
- Detection status and viral concentration measurements  
- Sampling dates and associated metadata  
- County and state identifiers  

Dataset reference:  
https://data.cdc.gov/Public-Health-Surveillance/CDC-Wastewater-Data-for-Measles/akvg-8vrb

The dataset is updated periodically by the CDC. The dashboard will be updated to reflect the most recent data.

---

## Dashboard Overview

The file `[Measles Wastewater Signal Dashboard](https://aidea1.github.io/Measles-Wastewater-Signal-Dashboard/)` includes:

- An interactive county-level map showing wastewater signal presence or intensity  
- Time-series visualizations for counties or facilities with available data  
- Filtering options for exploring specific states, counties, or date ranges  
- Hover tooltips displaying sample metadata and detection details  

The dashboard is fully self-contained and can be opened locally in a browser or hosted online.

---

## Project Purpose

This project aims to:

- Translate raw wastewater surveillance data into a clear, interactive visualization  
- Provide county-level insights into measles viral signals  
- Support public health monitoring and early detection efforts  
- Offer a reproducible, open-source tool for researchers and analysts  

The dashboard is designed to be intuitive and accessible, even for users without technical backgrounds.

---

## How the Dashboard Was Built

The dashboard was generated using Python and common data-science libraries.

### Workflow Overview

**1. Data Acquisition**  
- Downloading or querying the CDC dataset from `data.cdc.gov`

**2. Data Cleaning & Transformation**  
- Handling missing or inconsistent values  
- Aggregating facility-level data to the county level  
- Formatting dates and geographic identifiers  

**3. Visualization**  
- Creating interactive charts and county maps  
- Exporting the final output as a standalone HTML file  

**4. Deployment**  
- Storing the HTML file in this repository  
- Hosting via GitHub Pages  

---

## 📁 Repository Structure
.
├── measles_county_dashboard.html # Final interactive dashboard
├── data/ # Optional: cached CDC data
├── scripts/ # Optional: data processing + dashboard generation
│ ├── fetch_data.py
│ ├── clean_data.py
│ └── build_dashboard.py
├── requirements.txt # Python dependencies
└── README.md # Project documentation


This structure keeps the project organized and easy to navigate for collaborators and contributors.

---

## Hosting with GitHub Pages

To make the dashboard publicly accessible:

1. Commit `measles_county_dashboard.html` to the repository root (or `/docs`).  
2. Navigate to **Settings → Pages**.  
3. Under **Build and Deployment**, select:
   - **Branch:** `main`  
   - **Folder:** `/root` (or `/docs`)  
4. Save settings.

Dashboard will be available at: [Measles Wastewater Signal Dashboard](https://aidea1.github.io/Measles-Wastewater-Signal-Dashboard/)


---
## License

This project is released under the MIT License (or another license of your choice).

Including a license clarifies how others may use, modify, or build upon your work.

Citation

If you use this dashboard or workflow in academic or policy work, please cite:

Bhagavathula A. Measles Wastewater Signal Dashboard. GitHub repository. Year. https://www.ndsu.edu/people/akshaya-bhagavathula

You may also cite the underlying CDC dataset:

Centers for Disease Control and Prevention. Wastewater Data for Measles. data.cdc.gov.
