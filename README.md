# GlucoseLo Stats 📈

Welcome to the statistical analysis repository for the **GlucoseLo** project — a translational health data science initiative focused on improving glycaemic outcomes in people with type 1 diabetes (T1D), especially around physical activity.

This repo contains code and workflows for preprocessing, statistical modelling, and visualisation of CGM and clinical data used in the GlucoseLo project.

---

## 💡 Project Overview

**GlucoseLo** seeks to predict and understand glucose dynamics in people with T1D during and after exercise. Our approach integrates:

- 🧬 Matched-pair analysis of activity vs rest periods  
- 📉 Multilevel models of CGM response  
- 🚨 Detection and labeling of hypoglycaemic events  
- 🧠 Model simplification & SHAP-based interpretation  
- 🧪 Subgroup validation and external benchmarking  
- 🧰 Visualisation and deployment of interpretable decision tools  

---

## 🗂️ Repository Structure
glucoselo-stats/
├── preprocessing/ # CGM interpolation, resampling, cleaning
├── pairing/ # Matching physical activity and non-activity bouts
├── models/ # Mixed-effects models (e.g. lmer)
├── visualisation/ # Margins plots, heatmaps, auto-export
├── reports/ # R Markdown summaries and draft outputs
├── utils/ # Helper functions and constants
└── data/ # Cleaned + derived datasets (excluded from repo)


---

## ⚙️ Technologies Used

- **R**: `lme4`, `emmeans`, `ggplot2`, `dplyr`, `tidyr`
- **Python** (for preprocessing & SHAP): `pandas`, `xgboost`, `shap`
- **R Markdown**: for reproducible reporting
- **VSCode** + GitHub: collaborative analysis & version control

---

## 📊 Key Features

- **Multilevel modelling**: glucose nested within bouts, pairings, participants  
- **Margins plots**: estimated marginal means with `emmeans`, saved via `ggsave`  
- **Time-in-range events**: based on ATTD/ADA consensus definitions  
- **Imputation**: Linear interpolation of CGM at 15-min intervals  
- **Model simplification**: e.g. 3-feature models for real-world deployment  
- **Subgroup analysis**: age, sex, insulin type, baseline HbA1c, activity type  

---

## 🔐 Data Access

This repo does **not** contain raw CGM or clinical data due to ethical/privacy restrictions. To request access, please submit a data request via [Vivli.org](https://vivli.org) (Vivli ID: **8766**), or contact the project team.

---

## 🧑‍💻 Contributing

We welcome contributions! To contribute:

1. Fork the repo  
2. Make your changes in a new branch  
3. Submit a pull request  
4. Follow the existing directory and documentation style

---

## 📜 License

Distributed under the **MIT License**. See `LICENSE` file for details.

---

Built with ❤️ by the GlucoseLo team.
