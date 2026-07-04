
# Project Title: Evaluating the Predictive Power of Satellite Derived Chlorophyll a on Regional Fisheries Capture

---

## 🔍 Overview

This project establishes a robust data pipeline to investigate the relationship between oceanic environmental conditions and fisheries production. By merging complex NetCDF biogeochemical data from the **Copernicus Marine Environment Monitoring Service (CMEMS)** with annual fisheries capture statistics, this research evaluates whether satellite-derived chlorophyll-a concentrations can serve as predictive indicators for biological productivity in the **IBI (Iberia-Biscay-Ireland) region**.

## 🚀 Key Achievements

* **Automated Data Engineering**: Developed a pipeline to ingest and align heterogeneous data formats, including NetCDF and CSV.
* **Robust Preprocessing**: Resolved complex data issues, including spatial subsetting, handling of missing values, and type-sanitization of socioeconomic data.
* **Predictive Modeling**: Implemented a **Random Forest Regressor** to model environmental-biological interactions, providing a clear, evidence-based conclusion on the drivers of fisheries production.

## 📂 Repository Structure

```text
├── data/
│   ├── raw/                 # Original fisheries statistics
│   └── processed/           # Cleaned and merged analysis-ready data
├── main_notebook.ipynb      # The complete machine learning analysis
├── requirements.txt         # Dependencies for project reproducibility
└── README.md                # Project documentation

```

## 🛠 Getting Started

### Prerequisites

Ensure you have the required libraries installed:

```bash
pip install -r requirements.txt

```

### Data Note

This repository includes processed data in `data/processed/`. Due to file size constraints, raw NetCDF files (e.g., `cmems_mod_ibi_bgc_plankton_...`) are not included. Please download the corresponding datasets directly from the [Copernicus Marine Service](https://marine.copernicus.eu/) portal if you wish to re-run the full ingestion pipeline from scratch.

## 📊 Results & Conclusion

Our analysis yielded a model performance of $R^2 \approx 3.48 \times 10^{-5}$. This suggests that annual regional chlorophyll averages do not serve as a primary linear predictor for fisheries capture in the IBI region, indicating that local biological production is influenced by more complex, multi-factor environmental and anthropogenic dynamics.

---

*Created by Maham Taqi | Focused on Evolutionary Biology & Computational Genomics*

---
