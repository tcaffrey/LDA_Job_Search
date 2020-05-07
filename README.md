# Improving a Data Science job search with NLP and LDA
*Scraping Indeed for job adverts and applying NLP and LDA modelling

The notebook is divided into 3 sections:

1. Scraping data from indeed using Beautiful Soup
2. Analysing the job postings
3. Cleaning the data and applying topic modelling

For now I've only scraped jobs in Greater London as that's relevant to myself but I could also scrape jobs 
from other locations in the UK to increase the data set. 

## 1. Scraping Job Adverts

The information in each job advert on Indeed includes:
Job Title
Company
Location
Contract Type*
Salary*
Job Description

\*not included in every job advert. Contract Type (permanent, contract etc.) was only provided 40% of the time and Salary approximately 50% of the time.
