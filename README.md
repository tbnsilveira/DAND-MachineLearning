# Identifying fraud from Enron e-mails
This project is part of the Udacity Data Analyst Nanodegree and refers to *Intro to Machine Learning* module. Its main scope is to build a *person of interest (POI)* identifier based on financial and email data made public as a result of the Enron scandal, as explained below.

In 2000, Enron was one of the largest companies in the United States. By 2002, it had collapsed into bankruptcy due to widespread corporate fraud. In the resulting Federal investigation, a significant amount of typically confidential information entered into the public record, including tens of thousands of emails and detailed financial data for top executives. 


## Project details
This project is build on python and sklearn. Part of the code is available from [Udacity](https://github.com/udacity/ud120-projects.git). Following the most relevant files are described:

* *poi_id.py*: Starter code made available by Udacity for the POI identifier which contains now the code I used for my analysis. 

* *tester.py*: evaluation code used by Udacity to check the analysis result. 

* *emails_by_address*: this directory contains many text files, each of which contains all the messages to or from a particular email address. It is for reference in the case of more advanced features based on the details of the emails dataset. This data is not processed yet in this project.

* *final_project_dataset.pkl*: the dataset for the project. It combines the Enron email and financial data into a dictionary, where each key-value pair in the dictionary corresponds to one person. The dictionary key is the person's name, and the value is another dictionary, which contains the names of all the features and their values for that person. The features in the data fall into three major types, namely financial features, email features and POI labels.

> financial features: ['salary', 'deferral_payments', 'total_payments', 'loan_advances', 'bonus', 'restricted_stock_deferred', 'deferred_income', 'total_stock_value', 'expenses', 'exercised_stock_options', 'other', 'long_term_incentive', 'restricted_stock', 'director_fees'] (all units are in US dollars)

> email features: ['to_messages', 'email_address', 'from_poi_to_this_person', 'from_messages', 'from_this_person_to_poi', 'shared_receipt_with_poi'] (units are generally number of emails messages; notable exception is ‘email_address’, which is a text string)

> POI label: [‘poi’] (boolean, represented as integer)

