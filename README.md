## **Project Scope Document**

### Fraud Detection Case Study

### Nov 8-10, 2017


**Fraud Detection**

The fraud problem is actually semi-supervised in a way. We will not use the model to declare a ground truth about fraud or not fraud, but simply to flag which transactions need further manual review. We will essentially be building a triage model of what the most pressing (and costly) transaction we have seen.

**Project scope statement**

We will cross validate within this dataset to find the best model.

This is event data and we need to determine if it's fraud. We start by taking a look at the data and doing some EDA. There are 55 columns! What do these all mean? Many of them won't be useful for us, so a big part of the task is feature extraction.

We will use the “acct_type” column to get the label. There are a few different possibilities for this value, but all we care about is fraud or not fraud.

Many of these columns may be useful to us. We will use Beautiful Soup and NLP techniques to get features out of the description column.

**Introduction / Background to project**

We are a contract data scientist/consultant team hired by a new e-commerce site to try to weed out fraudsters. The company unfortunately does not have much data science expertise... so we must properly scope and present our solution to the manager before we embark on our analysis. Also, we will need to build a sustainable software project that we can hand off to the companies engineers by deploying our model in the cloud. Since others will potentially use/extend our code we will properly encapsulate our code and leave plenty of comments.

**Business case**

The "Product" of Fraud:

Something that we will have to think about throughout this case study is how the product of our client fits into the given technical process. A few points to note about the case of fraud:

* Failures are not created equal
    * False positives decrease customer/user trust
    * False negatives cost money
        * Not all false negative cost the same amount of $$$
* Accessibility
    * Other (non-technical) people may need to interact with the model/machinery
    * Manual review

**Deliverables**

* EDA - Looking at the data
* Scoping the problem
* Comparing models
* Model description and code
* Pickled model
* Prediction script
* Prediction script backed by a database
* ‘Hello World’ app
* Fraud scoring service
* Web front end to present results

**Constraints**

Rough timeline:

* Wednesday afternoon: Project scoping
* Thursday morning: Model building
* Thursday afternoon: Intro to Web apps with Flask
* Friday: Web based front-end app and deployment

**Key people / Key stakeholders**

> **Zack, Meghan, Jake S, Aaron**

> [quandary classroom]

> Responsible for …predicting fraudsters

> **new e-commerce site**

> [sensitive]

> Responsible for …supplying data

> **Taryn, Jon**

> [Galvanize 17-01-DS-BD-g53]

> Responsible for …moral support

**In scope**

We want to present potentially fraudulent transactions with their probability scores from our model. The transactions should will be segmented into 3 groups: low risk, medium risk, or high risk (based on the probabilities).

**Out of scope**

We will not use the model to declare a ground truth about fraud or not fraud, but simply to flag which transactions need further manual review.

**Project administration, monitoring and reporting**

* Wed 2pm Case study overview
* Thurs 9am Case study check-in
* Fri 9am Case study check-in
* Fri 2pm Case study presentation
