## Data Science Project

## Background and Context

The superstore is gearing up for its year-end sale and introducing an enticing new offer - the Gold Membership. This exclusive membership grants existing customers a 20% discount on all purchases for just $499, down from the regular $999. To promote this offer, a targeted campaign via phone calls to existing customers will be executed. Management seeks to develop a predictive model to classify customers based on their likelihood of purchasing the Gold Membership. This will optimize resource allocation and minimize unnecessary expenses by targeting those most likely to participate.

## Objective

The superstore wants to predict the likelihood of the customer giving a positive response and wants to identify the different factors which affect the customer's response. The data provided is used to identify these factors and then build a prediction model to predict the probability of a customer who gives a positive response.

## Exploratory Data Analysis

**Data Cleaning**:
1) Created new features like total purchase amount and total number of purchases.<br><br>
2) Dropped unnecessary columns identified through data visualization.<br><br>

**Feature Engineering**:
1) Removed features correlated with most others<br><br>
2) Converted year of birth to age for better interpretation.<br><br>
3) Created dummy variables for categorical features.<br><br>

**Data Preprocessing**:
1) Removed outliers from features.<br><br>
2) Scaled the data for logistic regression modeling.<br><br>

**Notable Results**:
1) The overall membership rate stands at 15%, indicating a moderate level of participation in the membership program. <br><br>
2) Those who opted for membership exhibit a lower average recency of 35 days compared to non-members, who have an average recency of 51 days. <br><br>
3) Customers with a PhD degree show a higher proportion of Gold membership status, suggesting a potential correlation between PhD and membership tier. <br><br>
4) Only a minimal 1% of customers have lodged complaints, reflecting a generally satisfactory experience. <br><br>
5) Higher avg. purchase ($50) offsets long recency (49 days) - Focus on increasing order value. <br><br>


## Models Implemented
**Logistic Regression**: <br><br>
<img width="371" alt="image" src="https://github.com/user-attachments/assets/213ee184-7386-41f0-9dc3-a2bf91930989">

**Ensemble Model**: <br><br>

Utilizing logistic regression, KNN, and SVC, this approach combines models to improve accuracy. The ensomble model I have utilized is voting classifier with soft voting.<br><br>
Logistic Regression: Identifies linear relationships.<br><br>
KNN: Recognizes similar patterns based on past behavior.<br><br>
SVC: Defines clear boundaries between responses.<br><br>
<img width="368" alt="image" src="https://github.com/user-attachments/assets/8c57cca2-68d8-4251-bbd6-8bc319aa91ee">

## Conclusion 

- Successfully predicted customer response likelihood and identified influential factors. <br><br>
- Ensemble model achieved impressive results (95% recall, 91% F1-score) compared to Logistic Regression. <br><br>
- Hyperparameter tuning and oversampling techniques boosted model's ability to forecast positive responses. <br><br>
- Enables targeted gold membership offers and personalized marketing campaigns. <br><br>
- Drives business growth through improved customer targeting and engagement. <br><br>


## Recomendations

- Adjust the gap between recency and overall spending by upselling. <br><br>
- They need to address the highly important but negatively correlated "teen home" feature. <br><br>
- They can capitalize on the high importance "web visits per month" feature to drive even greater online traffic. <br><br>











