# Intelecta Cup Telkom University 2025 – Data Mining Competition

By **Cognivio Team**

<img width="60" height="60" src="https://github.com/user-attachments/assets/f1a75b2f-d46a-492b-88ec-820a78530ad9">

---

This repository contains our submission for the **Data Mining Competition** held during the **Intelecta Cup Telkom University 2025** in the **qualifying round**.

The main objective of this case study is to **forecast future climate conditions** based on **multivariate time-series data**.  
We experimented with several ensemble-based approaches consisting of multiple weak learners.  
Below is a summary of our simplified experiment results:

| No | Model | MAPE (%) |
| --- | --- | --- |
| 1. | Linear Regression, Naive Drift, Naive Seasonal | 146.533 |
| 2. | LightGBM, Naive Drift, Naive Seasonal | 151.973 |
| 3. | LightGBM, XGBModel, Naive Drift, Naive Seasonal | **129.088** |
| 4. | XGBModel, Linear Regression, Naive Drift, Naive Seasonal | 142.532 |

Among these configurations, the **LightGBM + XGBModel + Naive Drift + Naive Seasonal** ensemble (Experiment 3) achieved the best performance.

You can view the corresponding notebook here:  
[`notebooks/final/cognivio-final-notebook.ipynb`](notebooks/final/cognivio-final-notebook.ipynb)

---

## Paper

We also prepared a paper explaining our full methodology and findings.  
You can find it in the `paper` directory under the filename:  
[`PENYISIHAN_MAKALAH_INTELECTA2025_DATAMINING_COGNIVIO.pdf`](paper/PENYISIHAN_MAKALAH_INTELECTA2025_DATAMINING_COGNIVIO.pdf)

The paper is fully written in **Bahasa Indonesia**.

---

## Results

In the qualifying round, our team ranked **30th out of 90 participants**,  
with a final score of **58.152 / 100**.

You can view the complete scoreboard using the link below:  
[Competition Scoreboard](https://docs.google.com/spreadsheets/d/11UPCvRbv1Ie1-NSEhEHN3U3oUMBVrBlcEzJ9Epq8MKI/edit?usp=sharing)
