# Time Series Analysis and Forecasting on Indian Agricultural Productivity

## Project Description
This project focuses on modeling and forecasting crop yields based on crop-wise, season-wise, state-wise, and year-wise data. The objective is to provide insights into agricultural productivity and aid farmers, agronomists, and policymakers in making data-driven decisions.

## Google Colab Notebook
You can access the interactive notebook [here](https://colab.research.google.com/drive/1z182Rm4veMni78ZnRL0rivRSAHtKQl2n?usp=sharing)

## Dataset Description
This dataset encompasses agricultural data for multiple crops cultivated across various states in India from the year 1997 until 2020. It provides crucial features related to crop yield prediction, including crop types, crop years, cropping seasons, states, areas under cultivation, production quantities, annual rainfall, fertilizer usage, pesticide usage, and calculated yields.

- **Total Observations**: 19,689
- **Columns**: 10 (9 independent variables + 1 response variable)

### Columns Description
1. **Crop**: The name of the crop cultivated.
2. **Crop Year**: The year in which the crop was grown.
3. **Season**: The specific cropping season (e.g., Kharif, Rabi, Whole Year).
4. **State**: The Indian state where the crop was cultivated.
5. **Area**: The total land area (in hectares) under cultivation for the specific crop.
6. **Production**: The quantity of crop production (in metric tons).
7. **Annual Rainfall**: The annual rainfall received in the crop-growing region (in mm).
8. **Fertilizer**: The total amount of fertilizer used for the crop (in kilograms).
9. **Pesticide**: The total amount of pesticide used for the crop (in kilograms).
10. **Yield**: The calculated crop yield (metric tons per hectare).

Please note that the dataset is placed in the `data/` directory.

## Objectives
1. **Yield Modeling and Forecasting**: 
   - Model and forecast crop yields based on crop-wise, season-wise, state-wise, and year-wise data.
   - Pre-process data to handle missing values and outliers for accuracy and reliability.
   - Conduct a stationarity check using statistical tests or visual inspection.
   - Apply appropriate transformations (e.g., differencing) to achieve stationarity.
   - Select suitable models (e.g., random walk for overall yield, MA(1) for specific crops) based on ACF and PACF analysis.
   - Evaluate model accuracy using AIC values and predict future yields with confidence intervals.

2. **Impact of Seasons on Crop Production and Yield**:
   - Examine the impact of seasons on crop production and yield.
   - Given the violation of ANOVA assumptions (normality and homogeneity of variances), utilize non-parametric methods for analysis.
   - Employ the Kruskal-Wallis test to assess differences between groups.
   - Conduct Dunn's test for pairwise comparisons to identify specific groups that differ significantly.

## Installation Instructions
To run this project locally, you need to have Python and the following libraries installed:

- pandas
- numpy
- matplotlib
- seaborn
- scikit-learn
- statsmodels
- plotly
- pmdarima
- scipy

You can install these packages using pip:
```bash
pip install pandas numpy matplotlib seaborn scikit-learn statsmodels plotly pmdarima scipy
