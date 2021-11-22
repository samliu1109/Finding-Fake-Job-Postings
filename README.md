# Finding-Fake-Job-Postings

Executive Summary 
Problem 
Finding a perfect job is always a challenging task for every user on the website. However, what is worse is that there are job positions from fake offers from scammers that are hard to discern and easily deceived, which detriment the user experience. Therefore, as a data analyst in the company, it is important to discover the underlying characteristics in the job posting that can be identified as a high probability of a fake job to mitigate the number of fake jobs on the website and improve user experience.

Key Findings  
1.	Salary range is the most important variable in the model. It shows that some salary ranges show high frequency in the fraud. For instance, the salary range formats appear as "15 -19", "1234 -12345", and "1517-1517" are two times more likely to be a fraud than other formats of salary ranges. 
2.	A company has a company logo or not is the third important variable in the model. The company that does not possess a company logo is roughly 2 time more likely to post a fake job than the company having a logo.
3.	A company that has a question is not a significant variable in the model.
4.	The industry is an influential variable in the model. For example, military and ranching is 2 time more likely to post a fake job than the animation industry and 3 time than the computing networking, oil & energy, and accounting industry.
5.	Location is an effective variable in the model. For example, a company in Houston is 20 percent more likely to post a fake job than a company in New York.
6.	The job title is also an effective variable in the model. For example, a job title such as work from home or administrative & office assistant is 2 times more likely to be a fake job than a job title such as customer service representative or data entry.

Model Performance Summary & Interpretation 
1.	Comparing the random forest and xgboost in the analysis, the random forest shows the highest area under the curve, roughly 99%, which means only a 1% misclassification rate. 
2.	The random forest has higher accuracy than xgboost. 
3.	The random forest has the lowest misclassification rate between the two models, indicating the best model to fit the data. In addition, the lowest mean of log loss shows a little error rate.
4.	Looking at the precision rate, how many are fake jobs in all the jobs labeled as fake. The random forest has the highest precision rate to label the right fake job.
5.	Looking at the recall rate, in all real fake jobs, how many have been identified. The random forest has the highest recall rate to identify the most real fake jobs.

Recommendations  
1.	Identify the strange salary range formats in the job posting and take some precautions to prevent these salary range formats appear in the job posting. 
2.	Require a company that wants to post a job on the website must include its company logo.
3.	Pay attention to the specific industry job post such as military and ranching, which have more probability than other industries to post a fake job.
4.	Identifying the location contains a higher ratio of a fake job posting.
5.	Deleting the job titles such as work from home or administrative & office assistant that most likely are fake job posting on the website.
