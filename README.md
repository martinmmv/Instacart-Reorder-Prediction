# Instacart Reorder Prediction

Predicting whether a user will reorder a given product in their next order,
using the Instacart Online Grocery Shopping Dataset 2017.

## Project Structure

| Step | Notebook | Description |
|---|---|---|
| Steps 1–3 | `DTSC870_Steps1_3.ipynb` | EDA, feature engineering, data preparation |
| Step 4 | `DTSC870_Step4.ipynb` | Logistic Regression (baseline) |
| Step 5 | `DTSC870_Step5.ipynb` | Decision Tree |
| Step 6 | `DTSC870_Step6.ipynb` | LightGBM (ensemble) |
| Step 7 | `DTSC870_Step7.ipynb` | Model comparison and recommendation |
| Step 8 | `DTSC870_Step8_Part1.ipynb` | Deployment — prediction function |

## Setup

1. Clone this repository
2. Download the dataset from Kaggle:
   https://www.kaggle.com/datasets/yasserh/instacart-online-grocery-basket-analysis-dataset
3. Place the zip file in a `data/` folder as `data/archive.zip`
4. Create and activate a virtual environment:
```bash
   python -m venv .venv
   source .venv/bin/activate  # Mac/Linux
   .venv\Scripts\activate     # Windows
```
5. Install dependencies:
```bash
   pip install -r requirements.txt
```
6. Run notebooks in order (Steps 1–3 first, then 4, 5, 6, 7, 8)

## Models & Results

| Model | ROC-AUC | PR-AUC | Brier Score | F1 |
|---|---|---|---|---|
| Logistic Regression | 0.9689 | 0.9841 | 0.0472 | 0.9520 |
| Decision Tree | 0.9685 | 0.9834 | 0.0466 | 0.9530 |
| **LightGBM** | **0.9710** | **0.9851** | **0.0458** | **0.9533** |

**Recommended model: LightGBM**

## Dataset
Instacart Online Grocery Shopping Dataset 2017
https://www.kaggle.com/datasets/yasserh/instacart-online-grocery-basket-analysis-dataset


---

## Author

| Martin Milon | M.S. Data Science | B.A. Economics & Political Science

---

## License

This project is submitted for academic purposes. All rights reserved by the respective author.
