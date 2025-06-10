# A/B Test Analysis

This repository contains Python code for conducting an A/B test analysis using statistical methods to compare conversion rates across different test groups. Below is an overview of the analysis process and findings:

## Overview

The Python script performs the following tasks:
- Imports necessary libraries for data analysis (`pandas`, `numpy`, `scipy.stats`, `statsmodels.stats.proportion`).
- Mounts Google Drive to access the CSV file containing test data.
- Reads and preprocesses the data from `Portfolio Project 2.csv`.
- Defines a list of relevant events for analysis and pivots the data to aggregate event counts per test group.
- Conducts statistical tests (two-sided z-test for proportions) to compare conversion rates between test groups for specified events.
- Calculates metric changes and determines statistical significance based on p-values (alpha = 0.05).

## Findings

Based on the analysis:
- **Group 1** showed statistically significant improvements in conversion rates for events "add_payment_info," "add_shipping_info," and "begin_checkout."
- **Group 2** and **Group 3** did not exhibit statistically significant differences in conversion rates across any events.
- **Group 4** demonstrated statistically significant decreases in conversion rates for events "begin_checkout" and "new_account."

## Conclusion

The results indicate that Group 1 experienced notable improvements in user conversion for specific events, while other groups did not show significant changes or exhibited declines in conversion rates. Further iterations of testing or adjustments may be needed to refine strategies for Groups 2, 3, and 4.

For detailed numerical results and statistical outputs, refer to the formatted data frame and styled output in the Python script.

Feel free to explore the code for detailed implementation and adjust parameters as necessary for future A/B testing analyses.

