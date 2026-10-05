# Changelog, StreetSpring Survivability Datasets 2026

Versions are dated. A version changes when any file, header, README or page sentence changes; score changes are called out explicitly.

## 2026.10.05

- This release corrects 2026.10.04. No score changed: every score column in the 24 metro files and the national file carries the same value as in 2026.10.04.
- Dallas and San Antonio are now held out of every comparison in the national file. Their rows keep every score; the comparison columns (city rank, tier, list size and city overall) are left empty for them, and every list is numbered over the metros that are compared. 2026.10.04 still compared both.
- Ranks, counts and the year in the national file print as whole numbers (5, not 5.0).
- data_source and the Citation line in every file header use the dataset's name, StreetSpring Survivability Datasets 2026.
- The national file's Recipe 2 header now states the gap between cities as measured from the files on every build, replacing "usually under 6 points", which was false for 2026.10.04.
- The 2026.10.04 entry below was corrected; its Correction bullet says what changed and why.
- Files: 24 metro files and one national file; 516,548 rows in total.

## 2026.10.04

- Scores are now produced by model v2-2026-08-22, replacing v1-2026-03-12. Every metro was rescored on one competitor registry vintage (the 2026-07-03 snapshot) so no metro's score depends on when its registry was last refreshed.
- All 24 metros were converted to the two-year percentage together, through national percentile maps (one per business type), so every metro's displayed score changed. This release supersedes the previous one for all 24 metros.
- Published business types rise from 110 to 146, and rows from 389,135 to 516,548. The additional types were already scored by the model and are now carried in the published files.
- Scores spread much more widely inside a city. For one business type in one metro, the gap between the highest and lowest ranked neighborhood at a good address (p90_survivability_score) has a median of 22.6 points, against 7.6 in 2026.09.25.1. The comparison covers 2,046 type-and-metro pairs: each business type ranked by both releases in at least five of the same neighborhoods, in the 22 metros that rank neighborhoods and are not held.
- Scores in the metro files run from 48.0 to 90.0. For one business type, the typical-address score (avg_survivability_score) spans a median of 36.0 points across the metro files, against 12.7 in 2026.09.25.1.
- The order of places changed. Over those 2,046 pairs the median rank correlation between the two releases is 0.04; the top-ranked neighborhood for a business type is the same in 120 of them (6%), and the overall number one neighborhood is the same in 2 of 22 metros. Read these rankings as new, not as an update of the previous ones.
- Every row now carries a citation block: publisher, publisher_url, dataset_name, dataset_version, dataset_doi, as_of_date, license and license_url. A single row read on its own is now enough to attribute, pin the version and honour the license. dataset_doi is the concept DOI, which always resolves to the newest version.
- source_url_business_type is new and carries an absolute, verified link to the business type ranking page. It is empty where the page was not proven to exist, never a guess.
- source_url is present and deliberately empty in every row of this release. It can only be filled for about a third of rows until the remaining place pages are built, and a partly filled citation column is less useful than an absent one. It will be filled in a later release.
- rank_withheld_reason is new in the metro files. It is filled on the 1,022 rows of the 7 places that keep their scores and are deliberately left out of every ranking, and says why. A place left unranked for any other reason carries it empty.
- Dallas and San Antonio remain held. Their metro files carry every row and score, and dallas-survivability-scores-2026.csv also keeps its neighborhood and town ranks; the dataset pages and the README name no neighborhood, rank or score for them. This release's national file still gives them city ranks (city_rank_for_business_subtype and city_overall_rank), which the dataset pages leave out of every comparison. Pacific Palisades in Los Angeles keeps its scores and is excluded from rankings, because its inputs predate the January 2025 fire.
- Correction (2026-10-05): this entry was revised after publication because the files do not support three of its statements: the score axis, the ordering of places, and the history of the Houston and Phoenix files. The wider spread between neighborhoods is now stated with its measure, the statement about Dallas and San Antonio was made exact, and rank_withheld_reason is now listed. The bullets above say what the files hold.
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
