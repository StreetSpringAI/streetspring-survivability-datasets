# Changelog, StreetSpring Survivability Datasets 2026

Versions are dated. A version changes when any file, header, README or page sentence changes; score changes are called out explicitly.

## 2026.10.04

- Scores are now produced by model v2-2026-08-22, replacing v1-2026-03-12. Every metro was rescored on one competitor registry vintage (the 2026-07-03 snapshot) so no metro's score depends on when its registry was last refreshed.
- Houston and Phoenix were rescored. Their previous files were unreadable from row group 794 of 918 and had never been converted to the published scale, so the earlier release described 22 metros rather than 24.
- All 24 metros were reconverted together. The two-year percentile maps are national, so correcting Houston and Phoenix changes the displayed score for every metro. This release supersedes the previous one for all 24, not only for the two.
- Published business types rise from 110 to 146, and rows from 389,135 to 516,548. The additional types were already scored by the model and are now carried in the published files.
- The gap between the strongest and weakest neighborhood inside a city is materially wider than in the previous release. The median city spread moves from about 5 points to about 21 points of two-year survival chance. The scores now use the full published 13 to 93 axis per business type, where the previous release was compressed; the ordering of places is substantially unchanged.
- Every row now carries a citation block: publisher, publisher_url, dataset_name, dataset_version, dataset_doi, as_of_date, license and license_url. A single row read on its own is now enough to attribute, pin the version and honour the license. dataset_doi is the concept DOI, which always resolves to the newest version.
- source_url_business_type is new and carries an absolute, verified link to the business type ranking page. It is empty where the page was not proven to exist, never a guess.
- source_url is present and deliberately empty in every row of this release. It can only be filled for about a third of rows until the remaining place pages are built, and a partly filled citation column is less useful than an absent one. It will be filled in a later release.
- Dallas and San Antonio remain held: their numbers are withheld from press and ranking surfaces. Pacific Palisades in Los Angeles keeps its scores and is excluded from rankings, because its inputs predate the January 2025 fire.
- Files: 24 metro files and one national file; 516,548 rows in total.

## 2026.09.25.1

- Same-day correction of 2026.09.25, released under its own version so a citation of either is unambiguous. 2026.09.25 (380,015 rows) stays available as its own Zenodo version.
- SCORES ADDED for bar, home-improvement-store, irish-pub and middle-eastern-restaurant. Until this version their rows kept April scores with an empty p90_survivability_score in every metro file and in the national file, because the calibration from the model's raw output to the two-year percentage had never been recovered for them. They now carry the same good-address and typical-address scores as every other type, every scored place is included (3,514 rows each across the 24 metro files, up from 1,234), and they are ranked. Other business types' scores are unchanged; their rank among the business types in a place, and each place's overall rank, move where these four enter the ranking.
- scored_locations_in_city in the national file now counts distinct scored locations. For the business types scored at 5 price points it counted each location once per price point, five times too many (Chicago afghan-restaurant 20,955, now 4,191). Scores and ranks did not change.
- New columns in the national file: city_overall_score, city_overall_avg_score, city_overall_rank, total_ranked_cities_overall and business_types_in_city_overall, one value per metro repeated on each of its rows, so every page reads the same overall metro rank.
- Column dictionary corrected: the ranks and tiers follow the good-address score (p90), and the tiers are cut at 10, 30, 70 and 90 percent of the list, not in fifths. The national header recipe now sorts by the rank, not by the average.
- Files: 24 metro files and one national file; 389,135 rows in total.

## 2026.09.25

- Rankings follow p90_survivability_score, the chance of lasting two or more years at a good address; avg_survivability_score is the typical address. Pages order their lists on the same column.
- New columns: neighborhood_overall_score, neighborhood_overall_avg_score, neighborhood_overall_max_score, neighborhood_overall_min_score, business_types_ranked_in_neighborhood, neighborhood_overall_rank and total_ranked_neighborhoods_overall. The overall rank is now a column of the file, so the city page and each neighborhood's page read the same number.
- Rank columns cover the business types StreetSpring publishes guides for; other scored types keep their scores with empty ranks.
- Geography: 1,317 neighborhoods added from city and county boundary files; place names audited metro by metro. Non-places (parks, airports, industrial parks, planning-area codes, owners' associations) removed from the public files; 358 names corrected (separators, capitals, spellings). URLs are unchanged.
- Column renamed: grid_points_in_neighborhood is now scored_locations_in_neighborhood, and grid_points_in_city is now scored_locations_in_city. Values unchanged. One unnamed San Diego place removed from the public file.
- Files: 24 metro files and one national file; 380,015 rows in total.

## 2026.09.13

- SCORE COLUMNS CHANGED SCALE. Every score column (avg, max, min and the four bounds) is now the projected chance of lasting two or more years, converted with the same per-sector calibration the metro rankings pages use, so a file and the page that links to it show one number for one business type and place. Before this version the files carried the model's raw 0 to 100 scale under the same column names (Denver, Parker, dermatology clinic: 56.3 in the file, 73 to 75 on the hub). Ranks and tiers that compare across business types were recomputed on the converted scale; ranks inside one business type are unchanged except for ties. The failure-rate columns are 100 minus the converted max and min.
- Every page sentence (key findings, counts, dates) is now generated from the file it describes, so the page cannot disagree with its download.
- Column dictionary corrected to the units the values use: employment_rate, vacancy_rate, pct_high_income, poverty_rate, pct_bachelor_plus and pct_housing_post_2000 are fractions of 1; income_score is dollars; income_tier values are Affluent, Upper-Middle, Middle, Working, Low-Income; rank tiers are Great, Good, Average, Below-average, Poor; income_rank is empty in this release.
- methodology_url now points at the page directly instead of a redirect.
- Files: 24 metro files and one national file; 158,010 rows in total.

## 2026.09.03

- Column dictionary, three recipes and a link to this README added to every file header. README published beside the files. Datasets mirrored to Zenodo (concept DOI 10.5281/zenodo.22287996, which always resolves to the newest version), Hugging Face, Kaggle and GitHub.

## 2026.04

- First public release: 24 metro files (neighborhood by business type) and one national file (metro by business type), CC BY 4.0.
