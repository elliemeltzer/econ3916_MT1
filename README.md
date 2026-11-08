# Interest Rates and Real Private Fixed Investment Growth

This project examines how the federal funds rate is associated with annual U.S. real private fixed investment growth, controlling for inflation and real GDP growth.

## Data

The analysis uses 57 annual observations from 1968–2024. Data come from FRED:

- [Real Private Fixed Investment — FPICA](https://fred.stlouisfed.org/series/FPICA)
- [Federal Funds Rate — FEDFUNDS](https://fred.stlouisfed.org/series/FEDFUNDS)
- [Real GDP Growth — A191RL1A225NBEA](https://fred.stlouisfed.org/series/A191RL1A225NBEA)
- [Inflation — FPCPITOTLZGUSA](https://fred.stlouisfed.org/series/FPCPITOTLZGUSA)

Investment growth is calculated as the annual percentage change in real private fixed investment. Monthly federal funds rates are averaged by year.

## Files

- `midterm_EM.ipynb`: Data preparation, figures, OLS models, and diagnostics.
- `data/`: The four source CSV files.

## How to Run

Open the notebook in Jupyter or VS Code with Python, pandas, NumPy, matplotlib, and statsmodels installed. Keep the `data` folder beside the notebook, restart the kernel, and run all cells from the top.

## Main Finding

The full model estimates a negative interest-rate coefficient, but it is not statistically significant at the 5% level using conventional or HC3 robust standard errors. The results describe associations rather than causal effects.
