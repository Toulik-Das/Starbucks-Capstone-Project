# Starbucks-Capstone
![1_YWVTNTQwh6dpI21k7vc1VA](https://user-images.githubusercontent.com/39211262/82521307-e8daf800-9b43-11ea-97f5-1e65affca8c0.png)

## Introduction
This Analysis is based on simulated data that mimics customer behavior on the Starbucks rewards mobile app. Once every few days, Starbucks sends out an offer to users of the mobile app. An offer can be merely an advertisement for a drink or an actual offer such as a discount or BOGO (buy one get one free). Some users might not receive any offer during certain weeks.

Not all users receive the same offer, and that is the challenge to solve with this data set.

Task is to combine transaction, demographic and offer data to determine which demographic groups respond best to which offer type. This data set is a simplified version of the real Starbucks app because the underlying simulator only has one product whereas Starbucks actually sells dozens of products.

Every offer has a validity period before the offer expires. As an example, a BOGO offer might be valid for only 5 days. You'll see in the data set that informational offers have a validity period even though these ads are merely providing information about a product; for example, if an informational offer has 7 days of validity, you can assume the customer is feeling the influence of the offer for 7 days after receiving the advertisement.

Given transactional data showing user purchases made on the app including the timestamp of purchase and the amount of money spent on a purchase. This transactional data also has a record for each offer that a user receives as well as a record for when a user actually views the offer. There are also records for when a user completes an offer.

# Installation
Make sure you have already installed library sklearn, seaborn and tqdm. Except for these, the code should run with no issues using Python versions 3.*.

# Project Motivation
For this project, given the Starbucks offer, customer profile, customer transaction data, I am going to:
1. Combine transaction, demographic and offer data to analyze which demographic groups respond(i.e.view&complete) best to which offer type;
2. Build a model that predicts whether or not someone will respond to an offer.


# Results
#### Customers Data Frame
This data frame is intended to aggregate offer and transactional data on a per customer basis. This should facilitate the analysis of each customer’s transactional behavior.
![download (1)](https://user-images.githubusercontent.com/39211262/82524901-b0d8b280-9b4d-11ea-9901-b959d8e7beb5.png)

Population distributions by gender, income and age. The sample provides significantly more males. Both the income and the age distribution seem to approach a normal distribution

![download (3)](https://user-images.githubusercontent.com/39211262/82524962-df568d80-9b4d-11ea-8b88-225b41962884.png)

Expenses and average transaction value grow as the income grows, which is expected.

![download (4)](https://user-images.githubusercontent.com/39211262/82524964-e1205100-9b4d-11ea-9496-3fb26dcdd105.png)

Similarly to income, as people get older, the value of their transactions and the total expense increase as they get older. This might be to the fact that there is a direct correlation between age and income.


# Licensing, Authors, Acknowledgements
You can the Licensing for the data and other descriptive information is available at Udacity Data Science Nanodegree project. Otherwise, feel free to use the code here as you wish.
