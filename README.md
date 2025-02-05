# Neural-Network-Challenge-1

Columbia AI Bootcamp Week 18 Module

## By Sami Chowdhury


## Overview

This assignment focused on our abilities to create a deep learning neural network model to predict whether a borrower will repay on their student loans. We created the model using tensorflow and scikitlearn. The data can be found at [this link](https://static.bc-edx.com/ai/ail-v-1-0/m18/lms/datasets/student-loans.csv)

## Repository Structure

```
├── models/
├──── student_loans.keras
├── student_loans_with_deep_learning.ipynb
├── student_loans.keras
├── README.md
```

## Code Demonstration

To run the code, please run all the cells in the **student_loans_with_deep_learning.ipynb** notebook. Ensure that you have the following libraries installed:
1. *pandas*
2. *tensorflow*
3. *sklearn*
4. *pathlib* 

## Question Responses

Below is the summary of the assignment and its main takeaways.

**1. Describe the data that you would need to collect to build a recommendation system to recommend student loan options for students. Explain why this data would be relevant and appropriate.**

> The type of data I would need to collect to build a reccomendation system to recommend student loan options for students is the same type of data found in the featureset of this model. That means I need to collect the following fields from students before I can run my model to recommend student loan options:

1. Payment History (payment_history)
2. Location (Location Parameter)
3. STEM Degree Score (stem_degree_score)
4. GPA Ranking (gpa_ranking)
5. Alumni Success (alumni_success)
6. Major of Study (study_major_code)
7. Time to Completion of Program (time_to_completion)
8. Finance Workshop Score (finance_workshop_score)
9. Cohort Ranking (cohort_ranking)	
10. Total Loan Score (total_loan_score)	
11. Financial Aid Score (financial_aid_score)

> If any of these data fields are missing from the collection of input data, our model would be missing crucial data to predict the student loan option, and would therefore be less accurate in its predictions. 

**2. Based on the data you chose to use in this recommendation system, would your model be using collaborative filtering, content-based filtering, or context-based filtering? Justify why the data you selected would be suitable for your choice of filtering method.**

> Based on the data we chose to use in this recommendation system, our model would be using content-based filtering. This is because we are primarily building the recommendations and predictions from the specific data given. None of our features include socioeconomic factors of each student paying back their loans, so we do not have enough descriptive data to use the other two methods. Instead, we are strictly following the content and features given from each student to predict their student loan options, meaning we would focus on using content-based filtering. 

**3. Describe two real-world challenges that you would take into consideration while building a recommendation system for student loans. Explain why these challenges would be of concern for a student loan recommendation system.**

> One of the real world challenges with building a recommendation system for student loans is getting enough data to train our model and then test our model on. Keeping consistent data and having enough of it is difficult to attain, and there is no certainty that production data would be consistent with training data. As such, having quality data in large quantities is one of the biggest challenges for building this reccomendation system.

> Another real world challenge with building a recommendation system for student loans is whether our model is too biased onto the training data, or overfitting. If our model is overfitting on the training data, that means our model will not have acceptable accuracy scores or prediction scores for future production data. Ensuring that the model is not heavily biased to the training data is a big challenge for creating reccomendation systems like this that predict student loan options. 


