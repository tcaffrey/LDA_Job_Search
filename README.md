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

- Job Title
- Company
- Location
- Contract Type*
- Salary*
- Job Description

*not included in every job advert. Contract Type (permanent, contract etc.) was only provided 40% of the time and Salary approximately 50% of the time.

## 2. Analysing the data
Within this section I've allocated new job title and contract type categories based on words contained in the role or contract columns.

### Job Titles 
Job titles into the following categories:

- Lead: Any title containing lead, chief, head or manager
- Senior: Any title containing senior or principal
- Graduate: Any title containing graduate
- Regular: Will class anything else as a regular role

### Contract Type
Contract types are classed as the following:

Contract: Anything that has 'contract' or 'temporary' associated with it <br/>
- Apprenticeship
- Internship
- Part-Time
- Permanent: Any contract that is classed as 'Full-time' or 'Permanent'

## 3. Topic Modelling

Testing a variety of LDA models using a range of topic numbers resulted in the chosen model containing 9 topics with a coherence score
of 0.475.

2 of the 9 topics are related to recruiter information (such as equal opportunities or referral schemes). However the remaining topics are related to Data Science and cover the following areas:

- Analytics & Statistical Modelling
- Deep Learning, NLP & Computer Vision
- Machine Learning, Big Data & Cloud Computing
- Building Products
- Project Management and supporting clients

