# DATA_607_Project_3

## Team

Gabrielle Bartomeo

Binish Chandry

Zach Dravis

Burcu Kaniskan

Niteen Kumar

Betsy Rosalen

## Project Description
This project will answer this globalresearch question **“Which are the most valued data science skills?”**

Grading rubric:
+ You will need to determine what tool(s) you’ll use as a group to effectively collaborate, share code and any project documentation (such as motivation, approach, findings).
+ You will have to determine what data to collect, where the data can be found, and how to load it.
+ The data that you decide to collect should reside in a relational database, in a set of normalized tables.
+ You should perform any needed tidying, transformations, and exploratory data analysis in R.
+ Your deliverable should include all code, results, and documentation of your motivation, approach, and findings.
+ As a group, you should appoint (at least) three people to lead parts of the presentation.
+ While you are strongly encouraged (and will hopefully find it fun) to try out statistics and data models, your
grade will not be affected by the statistical analysis and modeling performed (since this is a semester one
course on Data Acquisition and Management).
+ Every student must be prepared to explain how the data was collected, loaded, transformed, tidied, and
analyzed for outliers, etc. in our Meetup. This is the only way I’ll have to determine that everyone actively participated in the process, so you need to hold yourself responsible for understanding what your class-size team did! If you are unable to attend the meet up, then you need to either present to me one-on-one before the meetup presentation, or post a 3 to 5 minute video (e.g. on YouTube) explaining the process. Individual students will not be responsible for explaining any forays into statistical analysis, modeling, data mining, regression, decision trees, etc.
You are encouraged to start early, ask many questions, actively post on the provided discussion forum, etc.

## Division of Responsibilities

Web Scraping: Niteen and Binish

Cleaning and Tidying Data from Kaggle and from the web: Zach, Burcu, Betsy, and others?

Storing data in MySQL: Zach

EDA: Burcu

Visualizations: Betsy, Burcu

## Proposed potential specific research questions?

 1. Is there any interaction between the Kaggle survey takers' program language use (R or Python) and their recommended program languages? (e.g. R users recommending R more than Python users recommending Python)  (Burcu)
 2. Does survey takers' formal education has any relationship to the ML/DS method he or she is most excited about learning in the next year? (Binish)
 3.  Of those receiving pay in US Dollars, is Python or R overall most profitable for a Kaggle survey taker? (Gabby)
 4. Is there a difference between what 'Learners' think are the important skills to learn and what employed Data Scientists say are the skils and tools they are using? (Betsy)

## Process to answer the potential specific research questions?

### Question 1

### Question 2

### Question 3

*Columns used:*
+ CompensationCurrency (check that it's USD)
+ CompensationAmount (the money being paid)
+ WorkToolsSelect (the language being used)

*Process:*
+ Use select and filter to get only those who receive their pay in USD
+ Make sure the CompensationAmount column is regex'd properly so it can be put into numeric format
+ Remove all rows where the values for CompensationAmount are NA
+ Remove all rows where the values for WorkToolsSelect are NA
+ Make the values in WorkToolsSelect into lists; using strsplit should be adequate
+ Remove all rows where the WorkToolsSelect lists do not contain either "Python" or "R"
+ Plot it using ggplot2... not sure which plot yet.
 
### Question 4

See DRAFT_Proj_3_Ques_4.Rmd file.
