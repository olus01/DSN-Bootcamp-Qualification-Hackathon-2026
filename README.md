# DSN Bootcamp Qualification Hackathon 2026 — ML Track

> Predicting total product sales across DSN Mart stores in Nigeria.

[![Competition](https://img.shields.io/badge/Kaggle-Competition-20BEFF?logo=kaggle&logoColor=white)](https://www.kaggle.com/competitions/dsn-bootcamp-qualification-hackathon-2026-ml-track/overview)
[![Python](https://img.shields.io/badge/Python-3.8%2B-3776AB?logo=python&logoColor=white)](https://www.python.org/)
[![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-F37626?logo=jupyter&logoColor=white)](https://jupyter.org/)

## Overview

This repository contains a machine learning solution for the **DSN Bootcamp Qualification Hackathon 2026 — Machine Learning Track**.

The objective is to build a regression model that predicts the **total sales** of a product at a particular DSN Mart store, using information about the product and the outlet where it is sold.

DSN Mart operates stores across Nigeria, ranging from small corner shops to flagship hypermarkets in major urban centres, state capitals, and smaller towns. Reliable product-level sales forecasts can help the business make better decisions about:

- Stock planning and replenishment
- Pricing and promotion
- Store investment
- Product and outlet performance

## Business and Machine Learning Problem

Given historical product-store sales records, the task is to predict `total_sales` for every row in the test dataset.

This is a **supervised regression problem**:

- **Input:** Product attributes and outlet/store attributes
- **Target:** `total_sales`
- **Output:** One sales prediction for each row in `test.csv`
- **Evaluation metric:** Root Mean Squared Error (RMSE)
- **Goal:** Achieve the lowest possible RMSE; lower scores are better

## Project Workflow

The solution follows the data science workflow:

1. **Understand** the product-store dataset and the business context
2. **Explore** sales patterns across products, stores, locations, and outlet types
3. **Clean** missing values, inconsistent categories, and other data-quality issues
4. **Engineer features** from product and outlet information
5. **Train and evaluate** regression models using an appropriate validation strategy
6. **Predict** `total_sales` for the competition test data
7. **Communicate** findings, modelling decisions, and results clearly

## Key Areas of Analysis

The analysis focuses on factors that may influence product sales, including:

- Product characteristics and categories
- Product visibility and other available product measurements
- Outlet size, type, and location
- Store establishment information
- Differences between urban centres, state capitals, and smaller towns
- Relationships and interactions between products and outlets

## Repository Contents

Typical project files are organised as follows:

```text
DSN-Bootcamp-Qualification-Hackathon-2026/
├── README.md                 # Project documentation
├── data/                     # Competition data (not committed if restricted or large)
│   ├── train.csv             # Historical records with the target
│   └── test.csv              # Records requiring predictions
├── notebooks/                # Exploration, modelling, and prediction notebooks
├── src/                      # Reusable preprocessing and modelling code
├── submissions/              # Generated competition submission files
└── requirements.txt          # Python dependencies
```

> The exact files and folder names may vary depending on the local competition setup. Do not commit private credentials or restricted competition data.

## Getting Started

### 1. Clone the repository

```bash
git clone https://github.com/olus01/DSN-Bootcamp-Qualification-Hackathon-2026.git
cd DSN-Bootcamp-Qualification-Hackathon-2026
```

### 2. Create and activate a virtual environment

```bash
python -m venv .venv

# macOS/Linux
source .venv/bin/activate

# Windows
.venv\Scripts\activate
```

### 3. Install dependencies

```bash
pip install -r requirements.txt
```

### 4. Add the competition data

Download the competition files from Kaggle and place them in the expected data directory. The training data should contain the target column, while the test data should contain the same predictor fields without `total_sales`.

### 5. Run the analysis

```bash
jupyter notebook
```

Open the relevant notebook in `notebooks/` and run the cells from data loading through prediction generation.

## Submission

Predictions should be generated for every row in `test.csv` and uploaded to the competition platform in the required format.

Before submitting, confirm that:

- Every test row has exactly one prediction
- The prediction column has the expected name and order
- No prediction values are missing
- The submission file follows the competition's required format

Competition page: [DSN Bootcamp Qualification Hackathon 2026 — ML Track](https://www.kaggle.com/competitions/dsn-bootcamp-qualification-hackathon-2026-ml-track/overview)

## Qualification Context

This hackathon is also the qualification challenge for the DSN AI Bootcamp. Leaderboard performance is one of the inputs considered when selecting participants, but participation or a leaderboard position does not automatically guarantee selection.

The project therefore emphasises both model performance and sound data science practice: understanding the problem, justifying preprocessing and feature engineering decisions, evaluating models responsibly, and communicating results clearly.

## Expected Skills Demonstrated

This project demonstrates the ability to:

- Translate a business problem into a machine learning problem
- Perform exploratory data analysis
- Prepare mixed product and outlet data for modelling
- Engineer meaningful features
- Compare and validate regression models
- Use RMSE to assess prediction quality
- Produce a competition-ready submission
- Explain technical work to a broader audience

## Acknowledgements

- [Data Science Nigeria (DSN)](https://dsnghana.com/) for organising the bootcamp qualification hackathon
- [Kaggle](https://www.kaggle.com/) for hosting the competition
- The DSN mentors and the wider data science community

## Author

**Olus01** — [GitHub](https://github.com/olus01)

---

*This repository is an educational and competition project for the DSN Bootcamp Qualification Hackathon 2026 ML Track.*
