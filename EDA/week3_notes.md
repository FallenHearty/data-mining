# week 3

[cleaned data](../data/week3_knime_clean.csv)
[knime workflow](week3_submission.knwf)

open the workflow in knime 5.12. select your copy of heart.csv in the csv reader. choose an output path in the csv writer before running. the writer overwrites the file at its output path.

zero cholesterol and zero resting blood pressure were marked as missing. HeartDisease is the target.

missing values are left blank and need to be handled before training a model. the workflow also adds MaxHR / (220 - Age) as a new column.

the data does not include a diabetes diagnosis. fasting blood sugar alone cannot confirm whether someone has diabetes.

some things we found:

88.4% of the people with zero cholesterol had heart disease, compared to 47.7% of the others.

without the zeros, the cholesterol groups had disease rates of 41.7%, 45.2%, 46.8% and 57.3%. the group cutoffs were 207.25, 237 and 275.

for the under 50 group with our blood pressure, cholesterol and fasting blood sugar filters, 8 had heart disease. 7 of those 8 had asymptomatic chest pain. we used resting blood pressure from 90 to 119, cholesterol above 0 and below 200, and fasting blood sugar = 0.

among people with asymptomatic chest pain, exercise angina showed up in 68.4% of those with heart disease and 27.9% of those without.

MaxHR had a -0.400 correlation with heart disease. the heart rate ratio was -0.335.
