# Interpretation and limitations

The portfolio preserves the original analytical methods. The following are opportunities for a revised analysis, not fixes already made.

- **Outliers may be valid diamonds.** High prices and large carat values are not automatically errors. Median replacement changes the distributions and can weaken genuine price–size relationships.
- **The tests use modified prices.** Hypothesis-test results apply to the prepared data after IQR-based median replacement. They should not be presented as conclusions about unaltered market prices. Compare raw valid data with alternative treatments before making business decisions.
- **Cut comparisons are unadjusted.** Differences in carat, colour and clarity may explain differences in mean prices. A higher Fair-cut mean does not establish a causal premium for poorer cut quality.
- **Check test assumptions.** Independent two-sample tests use SciPy's default equal-variance assumption. Independence, variance differences and sampling design require review. Consider Welch tests, confidence intervals, effect sizes and multiple-testing adjustments.
- **A displayed p-value of zero is numerical underflow.** It does not mean the true p-value is exactly zero.
- **Data validation can be expanded.** Missing records, duplicate rows and invalid cuts are removed, but colour/clarity categories and physical relationships among dimensions are not fully checked. Zero prices may survive IQR treatment; explicitly decide how to handle them.
- **No model or realised business impact is claimed.** The submitted notebook contains no regression model, random forest, model evaluation or deployment. Background links are retained from the original notebook and were not independently reverified during packaging.

## Packaging changes

- Renamed the notebook to `Diamond_Price_Analysis.ipynb`.
- Removed the student number and nonessential notebook metadata.
- Replaced assignment-template headings with project headings.
- Preserved the original AI declaration's historical meaning and separately disclosed later packaging assistance.
- Updated the data path to `data/data.csv`.
- Retained the notebook's saved outputs and checked the analysis by executing code cells in order.
- Added documentation and regenerated four chart images.
