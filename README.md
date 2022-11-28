# Loan-Default-Prediction

## Goal

The goal is to help a client determine whether they should invest in p2p loans, and how to go about doing this by devising investment strategies with the help of machine learning models. We will analyze, explore and process the data, develop and evaluate various classification and regression models to provide strategies for high returns with low risk for investors.

## Overview

Lending Club is an online lending marketplace for peer-to-peer loans. Peer to peer lending is the practice of lending loans from investor to borrowers without any involvement of banks or other Non-banking financial company.  The reason customers opt for such a platform is that investors get higher returns on the amount funded and borrowers can easily secure personal loans hassle free and at low operational cost. 

It allows borrowers to get unsecured loans in the range of $1000 to $40,000 in a timely manner. The loan period usually lasts 3 years. The easy-to-use mobile application lets investors select from a variety of loan listings along with the information provided about the borrower including loan amount, grade and purpose. Through this, investors reap profit from the interest gained from these loans. 

## Dataset

The information available for each loan consists of all the details of the loans at the time of their issuance as well as more information relative to the latest status of loan such as how much principal has been paid so far, how much interest, if the loan was fully paid or defaulted, or if the borrower is late on payments etc. 

Loan data – The level of data is at loan ID level. If a person borrowed a loan from LC, then a row of data along with the loan characteristics and borrower characteristics are present in the data. 

## Exploratory Data Analysis and Insights

•	On first impressions we see that the classes are imbalanced. We have 13.8% of charged off loans compared to 86.2% of fully paid loans.

<img width="500" alt="image" src="https://user-images.githubusercontent.com/99356847/204199112-0272a2ef-cc86-4a77-a31c-d241929bd5b0.png">

•	The loans are divided into grades (A-G) with the best interest rate being offered on the A category of the loan and the worst being offered at G.

<img width="500" alt="image" src="https://user-images.githubusercontent.com/99356847/204199151-5741f790-a34e-4f1b-846a-16c60e269267.png">

•	We find that the majority of loans are given for the purpose of debt consolidation which we know is a common occurrence because majority of people have different kind of loans that they are paying such as car, home, credit card etc so to have them under one bracket would be highly beneficial for the ease of paying back multiple loans. 

<img width="500" alt="image" src="https://user-images.githubusercontent.com/99356847/204199200-9d075cc6-3cd1-4a47-8549-99e2402a23d9.png">

•	We also noticed that the majority of features have missing values. Such features can be removed in further prediction tasks as they would not be beneficial to the model

•	We also detected some outliers and removed them such that not much of the data is lost

## Model Development and Evaluation

We have taken a few different approaches to design the best investment strategies for investors.

1. Classification models to predict default risk

       • Decision Tree

       • GLM (Regression)

       • Random Forest Regression

       • GBM

    Best Model -GBM with highest specificity

2.  Regression models to predict annual returns

         • GLM

         • Random Forest Regression

    Best Model – Random Forest with lowest MSE


## Conclusion

Investors are hesitant to invest in lower grade loans which can yield high returns with high risk. We can minimize the risk factor by predicting lower grade loans that are less likely to default while also giving high returns.


