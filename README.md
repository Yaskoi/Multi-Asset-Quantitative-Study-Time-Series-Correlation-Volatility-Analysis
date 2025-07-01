# Multi-Asset Quantitative Study: Time Series, Correlation & Volatility Analysis

> Quantitative modeling of ETF volatility and dynamic dependencies using GARCH, BEKK, and VAR in Python.

Empirical study of volatility dynamics and inter-asset dependencies using three ETFs (VTI, ENOR, XRT) over a 10-year period (2015–2025). The project applies univariate and multivariate time series models to understand risk behavior and contagion during market stress.

## Summary

- **Goal**: Model volatility persistence and quantify cross-asset interactions.
- **Models**:
  - GARCH(1,1) for capturing conditional heteroskedasticity.
  - BEKK(1,1) multivariate GARCH for joint volatility and time-varying correlations.
  - VAR with impulse response functions (IRF) for analyzing dynamic spillovers.
- **Key Results**:
  - High volatility persistence across all assets.
  - Significant correlation spikes during crises (e.g., COVID-19), limiting diversification.
  - Asymmetric shock propagation, with retail sector ETF (XRT) reacting more strongly to external shocks.

## Highlights

- Implemented a **custom Python library** for estimating BEKK models (no suitable package was available).
- Comprehensive volatility diagnostics: conditional variances, covariances, correlations.
- VAR-based IRFs reveal structural dependencies and lagged cross-impacts.
- All modeling and statistical inference done in Python.

## Assets Analyzed

- **VTI**: US Total Market ETF – broad equity benchmark.
- **ENOR**: MSCI Norway ETF – energy-heavy exposure.
- **XRT**: SPDR Retail ETF – equal-weighted US retail stocks.

## Dependencies

- Python 3.12
- `numpy`, `pandas`, `statsmodels`, `matplotlib`

## Authors

- **Yassine Housseine**: Built all Python code including custom BEKK implementation.  

- **Hamid Lahjaji & Aymen Mehdid**: Statistical interpretation, graphics & reporting
