# BTC-fraud-forecasting

This project was done for a Data Science in Practice course and sought to explore the relationship between public interest in Bitcoin, historical, Bitcoin pricing, and the prevalnece of Bitcoin-related fraud. Through the use of exploratory visualization and predictive modeling, several figures were created and explored.

Known Data Issue:
- The original btc_historical.csv file was lost and had to be replaced. The replacement file varies significantly from the original version used when the script was written and, unfortunately, the current code does NOT reflect that change. Variability in column names, date ranges, and values may not line up as expected and thus the "Average Yearly Bitcoin Price" and price-forecast chunks should be re-verified.
- HOWEVER, the figures in the pdf are representative of the correct data as the markdown was generated before the file loss. Discrepancies

R Packages:
library(readr)
library(dplyr)
library(lubridate)
library(ggplot2)
library(scales)
library(rvest)
library(stringr)
library(tidyverse)

* Required input files are in the working directory and need to be installed in the same directory as the rmd file in order to execute correctly

Key Findings:
- Bitcoin price stability between 2018-2020, 2021 surge, 2022-2023 correction, and a rebound in late 2024 (timed with the election)
- Correlation with search interest peaks and price surges (2017-2018, 2021, 2025)
- Simpe regression of price on search interest R² ≈ 0.458, p ≈ 0.065 — a moderate but not statistically significant relationship.
- Multivariate model captures upward trender better but forecast intervals widen substantially past 2025 and, as seen today, the actual price trajectory hs already diverged sharply from my model.
