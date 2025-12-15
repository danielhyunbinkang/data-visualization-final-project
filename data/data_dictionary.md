# Data Dictionary

This document describes the variables used in the analysis examining the relationship between healthcare infrastructure and life expectancy across countries. All data are sourced from the World Bank Open Data repository and are reported at the country-year level.

---

## Variables

|       Variable Name    |               Description                |             Units           |          Source             |                Transformations / Notes                  |
|------------------------|------------------------------------------|-----------------------------|-----------------------------|---------------------------------------------------------|
|          country       |           Name of the country            |                —            |          World Bank         |       Standardized across datasets prior to merging     |
|           year         |      Calendar year of observation        |               Year          |          World Bank         | Filtered to years with available data across indicators |
|     life_expectancy    |         Life expectancy at birth         |              Years          | World Bank (SP.DYN.LE00.IN) |              Used as primary outcome variable           |
|   physicians_per_1000  |  Number of physicians per 1,000 people   | Physicians per 1,000 people | World Bank (SH.MED.PHYS.ZS) | Missing values present for some countries and years     |
| hospital_beds_per_1000 | Number of hospital beds per 1,000 people |    Beds per 1,000 people    | World Bank (SH.MED.BEDS.ZS) | Used as proxy for healthcare infrastructure capacity    |

---

## Notes on Data Quality and Coverage

- Data availability varies by country and year, particularly for healthcare infrastructure indicators in low-income regions.
- Life expectancy estimates are modeled by the World Bank using demographic and mortality data and may lag real-time changes.
- Healthcare infrastructure indicators measure quantity, not quality, and should be interpreted accordingly.
- This analysis is descriptive and does not adjust for confounding factors such as income, education, or public health policy.

---

## Intended Use

These variables are used to support exploratory data analysis and visualization of global health patterns. The data are not intended for causal inference or predictive modeling.

