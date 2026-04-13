# Scope

This project was created in the academic year 2021-2022 as part of the Computational Statistics Modeling specialization course at the University of Porto.

# FIFA 19 Forward Players Linear Regression

This repository contains a multiple linear regression analysis of FIFA 19 forward players. The goal is to explain and predict player `Overall` ratings using a combination of physical characteristics and mentality-related attributes.

## Project Overview

The analysis focuses on players in forward positions:

- `ST`
- `RS`
- `LS`
- `CF`
- `RF`
- `LF`

The response variable is `Overall`, and the candidate predictors include:

- `Age`
- `Height`
- `Weight`
- `Preferred Foot`
- `Aggression`
- `Interceptions`
- `Positioning`
- `Vision`
- `Penalties`
- `Composure`

The work is presented in the notebook [FIFA19_Forward_Players_Linear_Regression.ipynb](./FIFA19_Forward_Players_Linear_Regression.ipynb).

## Dataset

The dataset used in this project comes from the FIFA 19 Complete Player Dataset on Kaggle and is stored locally in [data/data.csv](./data/data.csv).

## Analysis Workflow

The notebook includes:

- data loading and filtering for forward players
- variable type inspection and transformation
- exploratory data analysis
- correlation analysis and multicollinearity assessment
- multiple linear regression model building
- interpretation of coefficients and adjusted effects
- model diagnostics and interaction assessment

## Main Findings

- `Positioning` is the strongest predictor of `Overall` among forward players.
- `Vision` and `Penalties` also contribute positively to explaining player quality.
- `Composure` was removed from the final model due to multicollinearity with `Positioning`.
- No statistically significant interaction was found between `Height` and `Positioning`.
- The final model explains a large proportion of the variability in `Overall` for forward players.

## Repository Structure

```text
.
|-- FIFA19_Forward_Players_Linear_Regression.ipynb
|-- README.md
`-- data/
    `-- data.csv
```

## How To Use

Open the notebook in Jupyter Notebook or JupyterLab and run the cells in order to reproduce the analysis.

## Author

Project by Susana Meiras.
