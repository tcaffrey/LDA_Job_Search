# Improving a Data Science job search with NLP and LDA
*Scraping Indeed for job adverts and applying NLP and LDA modelling*

The notebook is divided into 3 sections:

1. Scraping data from indeed using Beautiful Soup
2. Analysing the job postings
3. Cleaning the data and applying topic modelling

For now I've only scraped jobs in Greater London as that's relevant to myself but I could also scrape jobs 
from other locations in the UK to increase the data set. 

## 1. Scraping Job Adverts

The information in each job advert on Indeed includes:
Job Title <br/>
Company <br/>
Location <br/>
Contract Type* <br/>
Salary* <br/>
Job Description <br/>

*not included in every job advert. Contract Type (permanent, contract etc.) was only provided 40% of the time and Salary approximately 50% of the time.

## 2. Analysing the data

### Job Titles 
Data Scientist or machine learning engineer are the highest returning results for job title. However of the approximate 600 results returned from the search it seems there's a lot of variation in titles used and approximately 400 job titles only used once. 

Job titles into the following categories:

Lead: Any title containing lead, chief, head or manager <br/>
Senior: Any title containing senior or principal <br/>
Graduate: Any title containing graduate <br/>
Regular: Will class anything else as a regular role <br/>

### Contract Type
A mixture of contract and permanent roles are contained on Indeed. 
40% of roles have a type of contract associated with them. It may be possible to further investigate the ones without a contract type and find out more from their description. For now I will class contract types as the following:

Contract: Anything that has 'contract' or 'temporary' associated with it <br/>
Apprenticeship <br/>
Internship <br/>
Part-Time <br/>
Permanent: Any contract that is classed as 'Full-time' or 'Permanent' <br/>

