week 5

open week5_model_comparison.knwf in knime 5.12 and run all nodes. the workflow includes heart.csv.

the branches compare the original model with a lower cutoff, extra weight for women with heart disease, and both changes together. the scorer and roc nodes show the results.

this uses one test split that was reviewed while making changes. female recall improved with both changes, but female roc-auc did not. more testing is needed.
