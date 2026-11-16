# week 2 data notes

The heart disease dataset has 918 rows and 12 columns. There are no blank cells in the raw file.

Cholesterol is 0 in 172 rows (18.7%). Resting blood pressure is 0 in one row (0.1%). These values are likely missing and need to be accounted for in the analysis.


## summary

After treating the zero values as missing:

| column | mean | median | standard deviation |
| --- | ---: | ---: | ---: |
| Age | 53.51 | 54 | 9.43 |
| RestingBP | 132.54 | 130 | 18.00 |
| Cholesterol | 244.64 | 237 | 59.15 |
| MaxHR | 136.81 | 138 | 25.46 |

Oldpeak has 13 negative values. We kept them for further review.
