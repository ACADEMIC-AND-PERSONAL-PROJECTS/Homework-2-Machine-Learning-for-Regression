<div align="center">

<!-- HERO BANNER -->
<img src="https://capsule-render.vercel.app/api?type=waving&color=0:1a1a2e,30:16213e,70:0f3460,100:1a1a2e&height=300&section=header&text=HW2%20:%20Regression&fontSize=38&fontColor=ffffff&animation=twinkling" width="100%"/>

<!-- TYPING INTRO -->
<img src="https://readme-typing-svg.demolab.com/?font=Fira+Code&size=16&pause=1000&color=00d4ff&center=true&vCenter=true&width=600&lines=Machine+Learning+Zoomcamp+2026;DataTalks+Club;Homework+2+-+Linear+Regression+%26+Regularization&center=true" alt="Typing SVG" />

</div>

<!-- FLOATING ANIMATION CSS -->
<style>
@keyframes float {
  0%, 100% { transform: translateY(0px); }
  50% { transform: translateY(-10px); }
}
.anime-float {
  animation: float 3s ease-in-out infinite;
  display: inline-block;
}
</style>

<!-- TECH ICONS -->
<p align="center">
<img width="40" height="40" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/python/python-original.svg" alt="Python" />
<img width="40" height="40" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/numpy/numpy-original.svg" alt="NumPy" />
<img width="40" height="40" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/pandas/pandas-original.svg" alt="Pandas" />
<img width="40" height="40" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/matplotlib/matplotlib-original.svg" alt="Matplotlib" />
<img width="40" height="40" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/jupyter/jupyter-original.svg" alt="Jupyter" />
</p>

---

<!-- ABOUT -->
<table>
<tr>
<td width="60%">

### About

Second assignment of the **Machine Learning Zoomcamp 2026** organized by **DataTalks Club**. You can enroll in the course here: [courses.datatalks.club/ml-zoomcamp-2026](https://courses.datatalks.club/ml-zoomcamp-2026/).

This project covers **linear regression** and **regularization** for predicting car fuel efficiency. We explore missing value imputation strategies, hyperparameter tuning with Ridge regression, and seed sensitivity analysis to build robust models.

The **car_fuel_efficiency_2026.csv** dataset contains 10,000 vehicle records with technical specifications (displacement, horsepower, weight, etc.) and their fuel efficiency in MPG.

</td>
<td width="40%" align="center">

<img src="avatar.gif" width="220" alt="Avatar" style="border-radius: 20px; object-fit: cover;">

</td>
</tr>
</table>

---

<!-- STATS BAR -->
<table>
<tr>
<td align="center" width="120">

**10K**
Rows

</td>
<td align="center" width="120">

**5**
Features

</td>
<td align="center" width="120">

**6**
Questions

</td>
<td align="center" width="120">

**2.236**
Final RMSE

</td>
</tr>
</table>

---

<!-- QUESTIONS -->
### Homework Questions

<table>
<tr>
<td width="50%">

#### Q1 - Q2 : Exploration & Missing Values

- **Q1** : Column with missing values (`horsepower` : 877 NA)
- **Q2** : Median horsepower (`254`)

</td>
<td width="50%">

#### Q3 - Q4 : Imputation & Regularization

- **Q3** : Best imputation strategy (`With mean` : RMSE 2.202)
- **Q4** : Best regularization parameter (`r = 0` : RMSE 2.2045)

</td>
</tr>
</table>

<table>
<tr>
<td width="50%">

#### Q5 - Q6 : Stability & Final Evaluation

- **Q5** : Seed sensitivity std (`0.029`)
- **Q6** : Test RMSE with seed 9 & r=0.001 (`2.236`)

</td>
<td width="50%">

#### Key Takeaways

- Mean imputation slightly outperforms zero-fill
- Regularization hurts on this dataset (r=0 is optimal)
- Model is stable across random seeds (low std)

</td>
</tr>
</table>

---

<!-- KEY CONCEPTS -->
### Key Concepts

<table>
<tr>
<td width="33%">

#### Linear Regression
- Normal equation: `(X^T X)^-1 X^T y`
- Closed-form solution
- Baseline for comparison

</td>
<td width="34%">

#### Regularization (Ridge)
- L2 penalty: `XTX + rI`
- Prevents overfitting
- Hyperparameter `r` tuning

</td>
<td width="33%">

#### Model Evaluation
- RMSE metric
- Train / Validation / Test split
- Seed sensitivity analysis

</td>
</tr>
</table>

---

<!-- STRUCTURE -->
### Project Structure

```
HW2/
├── car_fuel_efficiency_2026.csv   # Dataset (10K vehicles)
├── notebook.ipynb                 # Notebook with solutions
├── main.py                        # Entry point
├── pyproject.toml                 # Project configuration
├── avatar.gif                     # Avatar image
└── README.md
```

---

<!-- SETUP -->
### Installation

```bash
# Clone the repo
git clone <repo-url>
cd HW2

# Install dependencies (with uv)
uv sync

# Launch the notebook
uv run jupyter notebook notebook.ipynb
```

---

<!-- DATASET PREVIEW -->
### Dataset Preview

| engine_displacement | horsepower | vehicle_weight | model_year | fuel_efficiency_mpg |
|:---:|:---:|:---:|:---:|:---:|
| 2180 | 243.0 | 3870 | 2006 | 31.9 |
| 2390 | 272.0 | 4210 | 2008 | 31.3 |
| 2320 | 267.0 | 4240 | 1996 | 27.5 |
| 2130 | 258.0 | 4490 | 1989 | 28.5 |
| 2580 | 304.0 | 4510 | 1994 | 31.0 |

---

<!-- RESULTS -->
### Results Summary

| Question | Answer | Detail |
|:---:|:---:|:---|
| Q1 | `horsepower` | 877 missing values |
| Q2 | `254` | Median of horsepower |
| Q3 | `With mean` | RMSE 2.202 vs 2.205 (zero) |
| Q4 | `r = 0` | RMSE 2.2045 (no regularization) |
| Q5 | `0.029` | Low std = stable model |
| Q6 | `2.236` | Final test RMSE |

---

<!-- FOOTER -->
<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:0f3460,50:16213e,100:1a1a2e&height=100&section=footer" width="100%"/>

**Machine Learning Zoomcamp 2026 -- DataTalks Club**

</div>
