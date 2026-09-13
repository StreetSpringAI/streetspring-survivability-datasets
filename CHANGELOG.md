# Changelog, StreetSpring Survivability Datasets 2026

Versions are dated. A version changes when any file, header, README or page sentence changes; score changes are called out explicitly.

## 2026.09.13

- SCORE COLUMNS CHANGED SCALE. Every score column (avg, max, min and the four bounds) is now the projected chance of lasting two or more years, converted with the same per-sector calibration the metro rankings pages use, so a file and the page that links to it show one number for one business type and place. Before this version the files carried the model's raw 0 to 100 scale under the same column names (Denver, Parker, dermatology clinic: 56.3 in the file, 73 to 75 on the hub). Ranks and tiers that compare across business types were recomputed on the converted scale; ranks inside one business type are unchanged except for ties. The failure-rate columns are 100 minus the converted max and min.
- Every page sentence (key findings, counts, dates) is now generated from the file it describes, so the page cannot disagree with its download.
- Column dictionary corrected to the units the values use: employment_rate, vacancy_rate, pct_high_income, poverty_rate, pct_bachelor_plus and pct_housing_post_2000 are fractions of 1; income_score is dollars; income_tier values are Affluent, Upper-Middle, Middle, Working, Low-Income; rank tiers are Great, Good, Average, Below-average, Poor; income_rank is empty in this release.
- methodology_url now points at the page directly instead of a redirect.
- Files: 24 metro files and one national file; 158,010 rows in total.

## 2026.09.03

- Column dictionary, three recipes and a link to this README added to every file header. README published beside the files. Datasets mirrored to Zenodo (DOI 10.5281/zenodo.22287997), Hugging Face, Kaggle and GitHub.

## 2026.04

- First public release: 24 metro files (neighborhood by business type) and one national file (metro by business type), CC BY 4.0.
