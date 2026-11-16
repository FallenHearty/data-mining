# week 3

[cleaned data](../data/week3_knime_clean.csv)
[knime workflow](week3_submission.knwf)

open the workflow in knime 5.12. select your copy of heart.csv in the csv reader. choose an output path in the csv writer before running. the writer overwrites the file at its output path.

zero cholesterol and zero resting blood pressure were marked as missing. HeartDisease is the target.

missing values are left blank and need to be handled before training a model. the workflow also adds MaxHR / (220 - Age) as a new column.
