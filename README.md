# chronic_disease_prediction
In this project, it is done a correlation study between the incidence of the chronic kidney disease and the searched terms on Google related to this disease, the income and the health insurance coverage of the population in United states. It was created a model that predicts the incidence of the disease based on the these features.
__________________________________________________________________________________________________________________________________




DIGITAL EPIDEMIOLOGY
The goal of this assignment is to set up a machine learning framework that predicts the prevalence of a specific chronic disease or health risk factor from digital records of online behavior.

You will need:

GROUND TRUTH DATA For this assignment you will use data from the Behavioral Risk Factor Surveillance System (BRFSS, https://www.cdc.gov/brfss/) database of the US Center for Disease Control and Prevention. The Web interface to find and download specific datasets is available at: https://www.cdc.gov/brfss/brfssprevalence/index.html Data is spatially aggregated at different levels (US, state, county, etc.) and temporally aggregated at the yearly scale. Select "Chronic Health Indicators" and then select a chronic condition of your choice (e.g., asthma) and download the corresponding data in CSV (click on the gear icon) for the available years and different indicators (e.g., raw prevalence, age-adjusted prevalence, etc.)

DIGITAL PROXY DATA You will use Google Trends data available at https://trends.google.com Select the relevant keyword(s) for your prediction problem, and select "United States" (or go directly to https://trends.google.com/trends/explore?geo=US). Scroll down to "subregion" (the default spatial regions are US states, matching the ground truth spatial aggregation) and download your data in CSV format. Make sure that you collect data for the same time intervals for which you have ground truth data (choose "custom time range" and then "full year" to select for a specific year). Keep in mind that the same lexical term might refer to multiple meaning of entities in the Google Trends interface (e.g., "asthma" as a search engine query, "occupational asthma" in the news, "Asthma" the movie, etc.)

PART 1: CORRELATION STUDY
1.1 - Study the correlation between the ground truth data and the Google Trends data. Explore multiple features of the ground truth data (e.g., crude prevalence, age-adjusted prevalence, etc.), and multiple keywords or entity types for querying the Google Trends data. Check for stability (or lack there of) across different years.

1.2 - Download US state-level data on income and poverty from the US Census Bureau. The data is available at: https://www.census.gov/data/tables/2017/demo/income-poverty/p60-259.html Study the correlation of your target ground truth feature with income/poverty features.

PART 2: PREDICTION MODEL
2.1 - Set up a regression model that predicts your chosen ground truth indicator(s) on the basis of Google Trends data for several keywords. Discuss the strategy you use for selecting additional keywords and for selecting which ones you include in the model. Select the model via temporal and spatial cross-validation, and discuss its generalizability across states and years on the basis of your results.

2.2 - Add to your model census features at the US state level (e.g., income data) and discuss how adding them impacts the predictive performance of the model.

2.3 - Look for data on health insurance coverage across US states (any source you can find) and integrate it in your model. Repeat the above evaluation.
