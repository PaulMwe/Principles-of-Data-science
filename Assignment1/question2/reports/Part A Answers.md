# Visualization Interpretations

## V1 — Gender boxplots
The boxplots compare math and reading score distributions across the gender categories in the dataset. For each gender, the median indicates the center of the corresponding score distribution. Reading scores are generally positioned higher than math scores for both groups, while the amount of spread can be seen from the box and whiskers. The mean math score is 63.63 for female and 68.73 for male. The mean reading score is 72.61 for female and 65.47 for male. Thus, the figure shows differences in the observed score distributions, rather than establishing that gender causes those differences.

## V2 — Test preparation impact on math
This chart compares average math scores for students who completed the test-preparation course and students who did not. The completed group has a mean math score of 69.70, while the none group has a mean of 64.08. The difference between these group means is 5.62 points. The bars therefore provide a direct descriptive comparison of math performance between the two preparation categories. The sample sizes are 358 completed and 642 none. This visualization describes an association in this dataset and does not by itself establish a causal effect of test preparation.

## V3 — Lunch type and average performance
The grouped comparison uses overall_avg, calculated as the mean of math, reading, and writing scores for each student. Students with standard lunch have an average overall score of 70.84. Students with free/reduced lunch have an average overall score of 62.20. The difference between the two lunch categories is 8.64 points. The chart therefore shows that overall performance varies across the observed lunch categories. Lunch type is a descriptive grouping variable here, so the chart should not be interpreted as proof that lunch type itself causes the score difference.

## V4 — Subject correlations
The heatmap shows Pearson correlation coefficients among math, reading, and writing scores. Math and reading have a correlation of 0.82. Math and writing have a correlation of 0.80. Reading and writing have a correlation of 0.95. All three relationships are positive, meaning higher scores in one subject tend to be associated with higher scores in the other subject in this dataset. The coefficients summarize linear association and do not imply causation.

## V5 — Math vs reading with trend lines
The scatter plot places reading score on the x-axis and math score on the y-axis, as required. The fitted line slope is 0.84 for students who completed test preparation and 0.86 for students who did not. Both slopes are positive, indicating that higher reading scores are associated with higher math scores in both groups. The difference in slopes is 0.02 points of math score per reading-score point. The legend reports the sample size for each group so the two fitted relationships can be interpreted in context. These fitted lines describe the observed linear association and should not be treated as evidence that test preparation causes a particular slope.
