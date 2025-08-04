# Economic Indicators Analysis (1960–2022)

This project analyzes various economic and demographic indicators including GDP, inflation, urban/rural population, and merchandise exports from 1960 to 2022. Given that the dataset violates assumptions for parametric testing (like normality and homogeneity of variance), non-parametric methods were used throughout the analysis.

## 📊 Dataset Overview
The dataset includes:
- Gross Domestic Product (GDP)
- Population growth (urban and rural)
- Inflation rates
- Merchandise exports and imports

## 🔧 Data Preprocessing
- Missing values handled using mean/median imputation
- Outliers detected using IQR
- Log and square root transformations tested for normalization

## ✅ Assumptions Checked
- **Shapiro-Wilk Test** for normality
- **Levene’s Test** for homogeneity of variance

## 🧪 Non-Parametric Tests Applied
| Test | Purpose | Result |
|------|---------|--------|
| Mann-Whitney U | GDP vs. Population Growth | p < 0.05 |
| Mann-Whitney U | GDP vs. Merchandise Exports | p < 0.05 |
| Spearman's Rank | GDP vs. Urban Population | ρ ≈ 0.9966 |
| Wilcoxon Signed-Rank | GDP before vs. after 1971 | p < 0.05 |
| Kolmogorov-Smirnov | Urban vs. Rural Population | p < 0.05 |
| Kruskal-Wallis | Population Growth across Decades | p < 0.05 |
| Kruskal-Wallis | GDP across Political Periods | p < 0.05 |

## 🧾 Key Findings
- Strong positive correlation between urban population and GDP
- Significant GDP variation across growth categories and political periods
- Significant difference between urban and rural population distributions

## 🛠️ Tools Used
- R (Base, `ggplot2`, `dplyr`, `car`, `nortest`, `stats` packages)
- Data cleaned and analyzed in RStudio

## 📁 Files
- `gdp_population_statistical_analysis.R` – R script containing all data cleaning, transformations, assumptions testing, and non-parametric test implementations.

## 📌 Author
**Amna Amir**  
BS Data Science, Air University  
