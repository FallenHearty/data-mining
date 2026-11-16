# week 2 data audit

The heart disease dataset has 918 rows and 12 columns. HeartDisease is the target. See the [data dictionary](data_dictionary.md) for column definitions.

## data quality

Cholesterol is 0 in 172 rows (18.74%). RestingBP is 0 in one row (0.11%). We treated these zeros as missing in the summary and box plots. Oldpeak includes negative values, which were kept for review.

## summary

The table uses adjusted values. Mean, median, and standard deviation do not apply to text categories.

| column | mean | median | standard deviation | missing % |
| --- | ---: | ---: | ---: | ---: |
| Age | 53.51 | 54 | 9.43 | 0 |
| Sex | n/a | n/a | n/a | 0 |
| ChestPainType | n/a | n/a | n/a | 0 |
| RestingBP | 132.54 | 130 | 18.00 | 0.11 |
| Cholesterol | 244.64 | 237 | 59.15 | 18.74 |
| FastingBS | 0.23 | 0 | 0.42 | 0 |
| RestingECG | n/a | n/a | n/a | 0 |
| MaxHR | 136.81 | 138 | 25.46 | 0 |
| ExerciseAngina | n/a | n/a | n/a | 0 |
| Oldpeak | 0.89 | 0.6 | 1.07 | 0 |
| ST_Slope | n/a | n/a | n/a | 0 |
| HeartDisease | 0.55 | 1 | 0.50 | 0 |

## observations

Age and MaxHR are slightly left-skewed. RestingBP, Cholesterol, and Oldpeak are right-skewed. The box plots show values outside the usual range.

The KNIME workflow reads the CSV and creates summary statistics, histograms, category charts, box plots, and a correlation heatmap. The histograms show the original values, including zeros. The statistics and box plots treat zero cholesterol and resting blood pressure as missing.
