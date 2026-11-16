# week 3

[cleaned data](../data/week3_knime_clean.csv)
[knime workflow](week3_submission.knwf)

open the workflow in knime 5.12. select your copy of heart.csv in the csv reader. choose an output path in the csv writer before running. the writer overwrites the file at its output path.

zero cholesterol and zero resting blood pressure were marked as missing. HeartDisease is the target.

missing values are left blank and need to be handled before training a model. the workflow also adds MaxHR / (220 - Age) as a new column.

the data does not include a diabetes diagnosis. fasting blood sugar alone cannot confirm whether someone has diabetes.

## findings

- heart disease was present in 88.4% of patients with zero cholesterol and 47.7% of the others.
- after excluding zeros, the disease rates across cholesterol quartiles were 41.7%, 45.2%, 46.8%, and 57.3%.
- among the under-50 patients who met our blood pressure, cholesterol, and fasting blood sugar filters, 8 had heart disease. 7 of those 8 had asymptomatic chest pain.
- among patients with asymptomatic chest pain, exercise angina appeared in 68.4% of those with heart disease and 27.9% of those without.
- MaxHR had a correlation of -0.400 with heart disease; the heart rate ratio had a correlation of -0.335.
