# Titanic Data Cleaning and EDA (Python / Pandas)

A beginner-friendly, step-by-step notebook where I clean the Titanic passenger dataset and explore it with charts. Every step has a short note explaining what the code does and why.

**Dataset:** 1,309 passengers, 11 columns (`pclass`, `name`, `sex`, `age`, `sibsp`, `parch`, `ticket`, `fare`, `cabin`, `embarked`, `survived`). Missing values: `age` (263), `cabin` (1,014), `embarked` (2), `fare` (1).

## What I did

| Stage | Details |
|---|---|
| Inspect | `head`, `tail`, `info`, duplicate check, missing values |
| Handle missing values | filled with the mean or mode, or dropped rows and columns where it made sense |
| Clean text | split `name` into surname and title, fixed casing, renamed columns |
| Tidy numbers | rounded `age` and `fare`, sorted records, reset the index |
| New features | family-size groups with a custom function and `apply()`, age groups with `cut()` |
| Combine tables | passengers per ticket with `groupby` and `merge()` |
| Explore | countplot, pie chart, bar plot, subplots, histogram, scatter plot, correlation heatmap, FacetGrid |

## Files

| File | Description |
|---|---|
| `titan_explained.ipynb` | Full notebook with explanations, code and charts |
| `titanic.csv` | Dataset (1,309 rows) |

## How to run

```
pip install pandas matplotlib seaborn jupyter
jupyter notebook titan_explained.ipynb
```

Keep `titanic.csv` in the same folder as the notebook.

## Limitations

- This is a practice project focused on data cleaning and charts, not a prediction model.
- Missing ages were filled in simply, which affects age-based results.
- `cabin` is missing for most passengers, so it was not used for analysis.

## Tools

Python, Pandas, Matplotlib, Seaborn, Jupyter Notebook

## Author

**Varshini Ganesan**: [GitHub](https://github.com/vrshy) | [LinkedIn](https://www.linkedin.com/in/varshiganesan)
