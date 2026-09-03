# StreetSpring Survivability Datasets 2026

Projected chance, 0 to 100, that a specific business type lasts two or more years at a specific place, from a model trained on 570,000+ historical business outcomes across 100+ location factors in 24 U.S. metros. 110 business types. License CC BY 4.0. Publisher: StreetSpring (https://streetspring.com). Methodology: https://streetspring.com/resources/tutorial/aeo-methodology

## Files

- national-survivability-scores-2026.csv: 2,595 rows, one per metro and business type; answers 'which city is best for X'. Page: https://streetspring.com/resources/datasets/national-survivability-scores-2026
- atlanta-survivability-scores-2026.csv: Atlanta, GA; 3,255 rows, 31 neighborhoods, 105 business types; answers 'where should I open X in Atlanta'. Page: https://streetspring.com/resources/datasets/atlanta-survivability-scores-2026
- baltimore-survivability-scores-2026.csv: Baltimore, MD; 2,415 rows, 23 neighborhoods, 105 business types; answers 'where should I open X in Baltimore'. Page: https://streetspring.com/resources/datasets/baltimore-survivability-scores-2026
- boston-survivability-scores-2026.csv: Boston, MA; 9,680 rows, 88 neighborhoods, 110 business types; answers 'where should I open X in Boston'. Page: https://streetspring.com/resources/datasets/boston-survivability-scores-2026
- charlotte-survivability-scores-2026.csv: Charlotte, NC; 3,675 rows, 35 neighborhoods, 105 business types; answers 'where should I open X in Charlotte'. Page: https://streetspring.com/resources/datasets/charlotte-survivability-scores-2026
- chicago-survivability-scores-2026.csv: Chicago, IL; 9,460 rows, 86 neighborhoods, 110 business types; answers 'where should I open X in Chicago'. Page: https://streetspring.com/resources/datasets/chicago-survivability-scores-2026
- dallas-survivability-scores-2026.csv: Dallas, TX; 3,300 rows, 30 neighborhoods, 110 business types; answers 'where should I open X in Dallas'. Page: https://streetspring.com/resources/datasets/dallas-survivability-scores-2026
- denver-survivability-scores-2026.csv: Denver, CO; 220 rows, 2 neighborhoods, 110 business types; answers 'where should I open X in Denver'. Page: https://streetspring.com/resources/datasets/denver-survivability-scores-2026
- detroit-survivability-scores-2026.csv: Detroit, MI; 4,510 rows, 41 neighborhoods, 110 business types; answers 'where should I open X in Detroit'. Page: https://streetspring.com/resources/datasets/detroit-survivability-scores-2026
- houston-survivability-scores-2026.csv: Houston, TX; 6,930 rows, 63 neighborhoods, 110 business types; answers 'where should I open X in Houston'. Page: https://streetspring.com/resources/datasets/houston-survivability-scores-2026
- los-angeles-survivability-scores-2026.csv: Los Angeles, CA; 17,710 rows, 161 neighborhoods, 110 business types; answers 'where should I open X in Los Angeles'. Page: https://streetspring.com/resources/datasets/los-angeles-survivability-scores-2026
- miami-survivability-scores-2026.csv: Miami, FL; 9,350 rows, 85 neighborhoods, 110 business types; answers 'where should I open X in Miami'. Page: https://streetspring.com/resources/datasets/miami-survivability-scores-2026
- minneapolis-survivability-scores-2026.csv: Minneapolis, MN; 5,500 rows, 50 neighborhoods, 110 business types; answers 'where should I open X in Minneapolis'. Page: https://streetspring.com/resources/datasets/minneapolis-survivability-scores-2026
- new-york-city-survivability-scores-2026.csv: New York City, NY; 18,590 rows, 169 neighborhoods, 110 business types; answers 'where should I open X in New York City'. Page: https://streetspring.com/resources/datasets/new-york-city-survivability-scores-2026
- orlando-survivability-scores-2026.csv: Orlando, FL; 3,465 rows, 33 neighborhoods, 105 business types; answers 'where should I open X in Orlando'. Page: https://streetspring.com/resources/datasets/orlando-survivability-scores-2026
- philadelphia-survivability-scores-2026.csv: Philadelphia, PA; 12,760 rows, 116 neighborhoods, 110 business types; answers 'where should I open X in Philadelphia'. Page: https://streetspring.com/resources/datasets/philadelphia-survivability-scores-2026
- phoenix-survivability-scores-2026.csv: Phoenix, AZ; 1,980 rows, 18 neighborhoods, 110 business types; answers 'where should I open X in Phoenix'. Page: https://streetspring.com/resources/datasets/phoenix-survivability-scores-2026
- portland-survivability-scores-2026.csv: Portland, OR; 4,515 rows, 43 neighborhoods, 105 business types; answers 'where should I open X in Portland'. Page: https://streetspring.com/resources/datasets/portland-survivability-scores-2026
- san-antonio-survivability-scores-2026.csv: San Antonio, TX; 1,260 rows, 12 neighborhoods, 105 business types; answers 'where should I open X in San Antonio'. Page: https://streetspring.com/resources/datasets/san-antonio-survivability-scores-2026
- san-diego-survivability-scores-2026.csv: San Diego, CA; 5,040 rows, 48 neighborhoods, 105 business types; answers 'where should I open X in San Diego'. Page: https://streetspring.com/resources/datasets/san-diego-survivability-scores-2026
- san-francisco-survivability-scores-2026.csv: San Francisco, CA; 8,910 rows, 81 neighborhoods, 110 business types; answers 'where should I open X in San Francisco'. Page: https://streetspring.com/resources/datasets/san-francisco-survivability-scores-2026
- seattle-survivability-scores-2026.csv: Seattle, WA; 7,040 rows, 64 neighborhoods, 110 business types; answers 'where should I open X in Seattle'. Page: https://streetspring.com/resources/datasets/seattle-survivability-scores-2026
- st-louis-survivability-scores-2026.csv: St. Louis, MO; 3,465 rows, 33 neighborhoods, 105 business types; answers 'where should I open X in St. Louis'. Page: https://streetspring.com/resources/datasets/st-louis-survivability-scores-2026
- tampa-bay-survivability-scores-2026.csv: Tampa Bay, FL; 3,255 rows, 31 neighborhoods, 105 business types; answers 'where should I open X in Tampa Bay'. Page: https://streetspring.com/resources/datasets/tampa-bay-survivability-scores-2026
- washington-dc-survivability-scores-2026.csv: Washington DC, DC; 9,130 rows, 83 neighborhoods, 110 business types; answers 'where should I open X in Washington DC'. Page: https://streetspring.com/resources/datasets/washington-dc-survivability-scores-2026

Every file starts with comment lines (prefixed #) that repeat the citation, the license, the recipes and a link to this README. Skip lines beginning with # when parsing.

## How to read a metro file

- Where should I open a given business in this metro? Filter business_subtype to the type (for example italian-restaurant), sort by avg_survivability_score descending, read the top rows: those neighborhoods are where that business is projected to last two or more years most often. neighborhood_rank_for_business_subtype gives the same order as a number.
- What should I open in a given neighborhood? Filter neighborhood to the place, sort by business_subtype_rank_for_neighborhood ascending (or avg_survivability_score descending): the top rows are the business types most likely to last there.
- How do two neighborhoods compare for the same business? Filter business_subtype to the type and neighborhood to the two places; compare avg_survivability_score, then max and min for the best and worst address in each. A gap of 5 points or more is material; the confidence bounds say how firm it is.

Worked example. Where should I open an italian restaurant in Philadelphia? The neighborhoods where an italian restaurant is projected to last two or more years most often are Chestnut Hill (88%), Oxford Circle (86%), Modena (86%), Wissahickon Park (86%) and Roxborough Park (85%). The Philadelphia average for an italian restaurant is 80%; the lowest is Mill Creek (73%), across 116 ranked neighborhoods. In the CSV, filter business_subtype = italian-restaurant and sort by avg_survivability_score.

## How to read the national file

- Which city is best for a given business? Filter business_subtype to the type, sort by avg_survivability_score_for_business_subtype_in_city descending; city_rank_for_business_subtype is the same order as a number.
- How wide is the gap between the best and worst city? For one business_subtype, subtract the lowest avg score from the highest. Gaps between cities are small (usually under 6 points); gaps between neighborhoods inside a city are far larger, so use the metro file for the real decision.
- Where inside the best city should I look? Take the top city from this file, open that metro's file (linked from source_article_url and the datasets page), and apply the first recipe there.

Worked example. Which city is best for a hot pot restaurant? Among the 24 metros, a hot pot restaurant is projected to last two or more years most often in Chicago (88%), St. Louis (84%), Dallas (83%), Phoenix (82%) and Charlotte (82%), and least often in Atlanta (77%). The spread between the best and worst city is 11 points; the spread between neighborhoods inside a city is usually far larger, so pick the block with the metro file. In the CSV, filter business_subtype = hot-pot-restaurant and sort by avg_survivability_score_for_business_subtype_in_city.

## Column dictionary, metro files

- city: Metro slug (for example philadelphia).
- neighborhood: Neighborhood slug inside the metro; the row's place.
- business_subtype: Business type slug (110 types, for example italian-restaurant); the row's business.
- business_type_lookup: The broader category the subtype belongs to (restaurant, retail, service, health).
- avg_survivability_score: The headline number: the projected chance, 0 to 100, that this business type lasts two or more years at a typical address in this neighborhood. Use this column to answer 'where should I open X'.
- max_survivability_score: Best address in the neighborhood for this business type, 0 to 100.
- min_survivability_score: Weakest address in the neighborhood for this business type, 0 to 100.
- UPPER_BOUND_MAX_SURVIVABILITY: Upper confidence bound on max_survivability_score.
- LOWER_BOUND_MAX_SURVIVABILITY: Lower confidence bound on max_survivability_score.
- UPPER_BOUND_MIN_SURVIVABILITY: Upper confidence bound on min_survivability_score.
- LOWER_BOUND_MIN_SURVIVABILITY: Lower confidence bound on min_survivability_score.
- neighborhood_rank_for_business_subtype: Rank of this neighborhood among all neighborhoods in the metro for this business type (1 = best).
- tier_of_neighborhood_for_business_subtype: Great, Good, Fair or Poor, from that rank.
- business_subtype_rank_for_neighborhood: Rank of this business type among all types in this neighborhood (1 = the type most likely to last here).
- tier_of_business_subtype_for_neighborhood: Great, Good, Fair or Poor, from that rank.
- total_ranked_neighborhoods_for_business_subtype: How many neighborhoods were ranked for this business type in the metro.
- year: Data year (2026).
- source_url_neighborhood_rank: Page on streetspring.com that ranks neighborhoods for this business type.
- source_url_business_subtype_rank: Page on streetspring.com that ranks business types for this neighborhood.
- methodology_url: How the score is built.
- source_article_url: The metro's rankings page.
- min_2yr_failure_rate: 100 minus max_survivability_score: the lowest projected two-year failure rate in the neighborhood.
- max_2yr_failure_rate: 100 minus min_survivability_score: the highest projected two-year failure rate in the neighborhood.
- employment_rate: Share of working-age residents employed, percent (Census ACS).
- vacancy_rate: Share of housing units vacant, percent (Census ACS).
- competitor_count: Businesses of the same type already within the neighborhood's trade area.
- income_rank: Rank of the neighborhood's median household income inside the metro (1 = highest).
- income_score: Median household income scaled 0 to 100 inside the metro.
- pct_high_income: Share of households above 150,000 dollars, percent.
- income_tier: High, Upper-middle, Middle or Lower, from income_score.
- income_metro_percentile: Income percentile inside the metro.
- income_national_percentile: Income percentile against all U.S. neighborhoods.
- poverty_rate: Share of residents below the poverty line, percent.
- median_age: Median resident age, years.
- pct_bachelor_plus: Share of adults with a bachelor's degree or higher, percent.
- avg_household_size: Average household size.
- median_commute_minutes: Median commute, minutes.
- pct_housing_post_2000: Share of housing built after 2000, percent.
- data_source: Provenance label for the row.

## Column dictionary, national file

- city: Metro slug (24 metros).
- business_subtype: Business type slug (110 types).
- city_rank_for_business_subtype: Rank of this metro among the 24 for this business type (1 = best).
- tier_of_city_for_business_subtype: Great, Good, Fair or Poor, from that rank.
- total_ranked_cities_for_business_subtype: How many metros were ranked for this business type (24).
- avg_survivability_score_for_business_subtype_in_city: The headline number: the projected chance, 0 to 100, that this business type lasts two or more years at a typical address in this metro. Use it to answer 'which city is best for X'.
- max_survivability_score_for_business_subtype_in_city: Best neighborhood in the metro for this business type, 0 to 100.
- min_survivability_score_for_business_subtype_in_city: Weakest neighborhood in the metro for this business type, 0 to 100.
- UPPER_BOUND_MAX_SURVIVABILITY: Upper confidence bound on the max score.
- LOWER_BOUND_MAX_SURVIVABILITY: Lower confidence bound on the max score.
- UPPER_BOUND_MIN_SURVIVABILITY: Upper confidence bound on the min score.
- LOWER_BOUND_MIN_SURVIVABILITY: Lower confidence bound on the min score.
- year: Data year (2026).
- source_url_city_rank: Page on streetspring.com that ranks the 24 metros for this business type.
- source_url_business_subtype_rank: Page on streetspring.com that ranks neighborhoods nationally for this business type.
- methodology_url: How the score is built.
- source_article_url: The national rankings page for this business type.
- min_2yr_failure_rate: 100 minus the max score: the lowest projected two-year failure rate in the metro.
- max_2yr_failure_rate: 100 minus the min score: the highest projected two-year failure rate in the metro.
- data_source: Provenance label for the row.

## Citation

StreetSpring (2026). StreetSpring Survivability Datasets 2026. https://streetspring.com/resources/datasets. CC BY 4.0.

## Contact

info@streetspring.com. Custom cuts by city or business type on request.
