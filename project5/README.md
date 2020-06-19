# PROJECT 5 - Communicate Data Findings

Data visualization is an important skill that is used in many parts of the data analysis process. 

**Exploratory data visualization** generally occurs during and after the data wrangling process, and is the main method that you will use to understand the patterns and relationships present in your data. This understanding will help you approach any statistical analyses and will help you build conclusions and findings. This process might also illuminate additional data cleaning tasks to be performed. 

**Explanatory data visualization** techniques are used after generating your findings, and are used to help communicate your results to others. Understanding design considerations will make sure that your message is clear and effective. In addition to being a good producer of visualizations, going through this project will also help you be a good consumer of visualizations that are presented to you by others.


## Dataset 
**Prosper's Loan Dataset**

The analysis was performed for the examination of Prosper's loan dataset, a personal loan company that provides a peer-to-peer lending marketplace, with 65056 loans listings in the dataset with 15 variables. The dataset contains featured on loan applications, which are used by Prosper to render ratings on people that request a loan. A list of the attributes and their description can be found in this spreadsheet.

## Summary
* My analysis to the examination of Prosper's rating system was limited to some features. Specifically how some features present in the dataset may influence the rating given by Prosper to borrowers with no prior loans. Since 2009, Prosper has been using its own rating system, represented in the loans dataset by the variable Prosper Rating, which allegedly has two components: Prosper Score and Credit Score.


* In the exploration, I found that there was a strong relationship between Prosper Ratings, Prosper Score and Credit Score, but mainly between Prosper Rating and Prosper Score.


* I also found that other features, other than just Prosper Score and Credit Score, influences Prosper Ratings. By exploring the variables present in the dataset in relation to Prosper Rating, I could find that Income, Debt, Inquiries, Bankcard Utilization and Delinquencies are features considered in the Prosper rating system.


* I could not find out, however, in which moment these features influence Prosper Rating, whether they influence directly Prosper Rating, or they influence the Scores, influencing Prosper Rating indirectly. I found, however, by exploring with multivariate plots, hints that these variables may influence Credit Scores more than they influence Prosper Scores, and this makes sense as Prosper Scores are probably built on top of Prosper loans data, related to loans payments and delinquencies.


To conclude this analysis , I say that the loan approval status is heavily dependent on the applicant's information on IncomeRange, Homeownerstatus and employment status.

-----

Key Learnings from the project:

- Supplement statistics with visualizations to build understanding of data.

- Choose appropriate plots, limits, transformations, and aesthetics to explore a dataset, allowing you to understand distributions of variables and relationships between features.

- Use design principles to create effective visualizations for communicating findings to an audience.
