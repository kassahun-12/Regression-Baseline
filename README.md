# Regression Baseline and Diagnostics: Summary

This project evaluates baseline approaches for fingerprint verification using the DB1_B and DB2_B image datasets. The task is formulated as binary classification of genuine and impostor fingerprint pairs. Three image-comparison features are considered: mean absolute pixel difference, pixel correlation, and structural similarity (SSIM).

To reduce identity leakage, fingerprint identities are grouped before the data are divided into training, validation, and test partitions. Genuine and impostor pairs are generated within their assigned partitions. A naive baseline is compared with logistic regression models using L1 and L2 regularization. Model selection is based on validation performance, while the test set is reserved for final evaluation.

The evaluation focuses on ROC-AUC and balanced accuracy, alongside comparisons with the naive baseline and diagnostic inspection of classification errors. The final model and its numerical performance should be reported from the actual experimental outputs. No numerical results or claims of improvement are included here without verified measurements.

Several limitations affect the interpretation of the results. The datasets are limited in size, and pairwise comparisons reuse source images, meaning that individual pairs are not statistically independent. Performance may also depend on image alignment, preprocessing, and the selected similarity features. Therefore, the results provide an initial experimental baseline rather than evidence of generalization to unseen acquisition conditions or readiness for real-world deployment.

The repository documents the experimental workflow, dependency requirements, data-split audit, model comparison, diagnostic outputs, and reproduction instructions. The final committed version should correspond to the notebook and code used to generate the reported results.
