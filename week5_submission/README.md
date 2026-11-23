# Week 5: Fairness Correction

We tested whether oversampling and a lower prediction cutoff for women could help the model catch more cases of heart disease.

To run the setup:

1. Import `week5_revised_model.knwf` into KNIME 5.12.0.
2. Open the workflow and select **Execute All**. The workflow includes `heart.csv`.
3. Open the Scorer and ROC Curve nodes for women and men to see recall, precision, and ROC-AUC.

To reproduce the five-fold comparison, run `week5_cv_baseline.knwf` and `week5_cv_missing_flag_v2.knwf`. To see the cutoff-only and oversampling-only tests, run `week5_model_comparison.knwf`.

The results are exploratory because we chose changes after looking at the data and had already seen the earlier test split.

[Week 5 report and screenshots](week5_report_current.pdf)
