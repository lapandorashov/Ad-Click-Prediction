# Ad-Click-Prediction

## Business Problem
We would like to investigate if we can predict if a customer will open and click through an advertisement sent to their email. Being able to predict if customers will click through an advertisement or knowing which advertisements certain customers are more likely to click on would be useful as it would allow businesses to predict the number of customers who would click on an ad before starting the ad campaign. Knowing how customers respond to different emails would allow companies to tailor their emails based on what they hope to gain from each ad campaign. This prediction could be used before a company launches a new product or ad campaign giving the business an estimate of people who will open and click through their new ad.

## Modeling Ideas
To approach the business problem, our target variable will be if the customer who received the advertisement email has clicked through the link or not before the campaign ended. We will use classification for this prediction task. Since we have a clear target variable in mind, and the dataset provides historical info on the target variable, our model will fall into supervised learning. One data instance in the dataset is one customer who received the email campaign. To predict if the customer clicks, we can refer to their past purchasing behaviors, their user profile, the characteristics of the email, and the time the email was sent.

## Data Details
The dataset comes from a website (https://datamasked.com/) for data science interview. After browsing the data by loading the data into Python, we find that the dataset has 100,000 rows and 9 variables (4 categorical variables, 2 binomial variables, 3 integer variables). Our target attribute (if_click) has 2 values, 2% for 1 and 98% for 0. The other variables of the dataset can be divided into 2 parts. The first part is about the characteristics of the email; the second part is about the customer’s features, as is mentioned in the modeling part. Here are all the variables we wil use for prediction:
- email_text: if the email is long or short
- email_version: if email is generic or tailored for the customer
- Hour: the hour sending the email
- Weekday: the weekday sending the email
- User_country: the country of user
- User_past_purchase: the number of past purchases of the customer
