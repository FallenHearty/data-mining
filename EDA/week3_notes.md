# week 3

[cleaned data](../data/week3_knime_clean.csv)
[knime workflow](week3_submission.knwf)

the workflow uses heart.csv. the file paths might need to be changed on another computer since we only tested this locally on one of our computers. 

there were some cases of zero cholesterol and zero resting blood pressure so they were marked as missing. the variable 'HeartDisease' is the target variable as well. all of the missing values were left blank and have to be handled before training a model. this workflow also adds another collumn as (MaxHR / (220 - Age)).

it is worth mentioning that the data does not include a diabetes diagnosis and we cannot confirm whether someone has diabetes.

noteworthy mentions:

88.4% of the people that had zero cholesterol had heart disease and compared to the other 47.7% that had a value of nonzero cholesterol. there were also 172 people in the zero group and 746 in the other group. however, the zero values likely mean the cholesterol reading is missing.

if we disregard the zeros, the cholesterol groups would have disease rates of 41.7%, 45.2%, 46.8% and 57.3%; the group cutoffs were 207.25, 237 and 275. 

for the under 50 group with our blood pressure, cholesterol and fasting blood sugar filters, 8 had heart disease, 7 of those 8 had asymptomatic chest pain, and there were also 9 people without heart disease in this group. 1 had asymptomatic chest pain. to find this, we used resting blood pressure from 90 to 119, cholesterol above 0 and below 200, and fasting blood sugar = 0.

within the people with asymptomatic chest pain the exercise angina showed up in 68.4% of those with heart disease and 27.9% of those without heart disease. this group had 392 people with heart disease and 104 without. the average MaxHR was 125.8 with heart disease and 138.5 without heart disease. average Oldpeak was 1.33 with heart disease and 0.53 without.

MaxHR had a -0.400 correlation with heart disease. the heart rate ratio was -0.335.
