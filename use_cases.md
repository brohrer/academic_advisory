# Data science use cases, by topic

## Advertising
* **Ad relevance**: given an individual's purchase history and demographics, return a set of advertisements ordered by relevance.

## Agriculture
* **Yield prediction**: given crop type, soil type, soil treatment, temperature, and moisture, predict the weight in harvested grain. 

## Astronomy

### Relevant data sets
* **[HyperLEDA](http://leda.univ-lyon1.fr/intro.html)**: a database and a collection of tools to study the physics of galaxies and cosmology. 

## Bioinformatics
* Given certain proeprties of a gene how one can predict its expression?
* Impute the missing characteristics in a gene expression

### Relevant data sets
* **[Human epidermal growth factor receptor 2-positive breast cancer brain metastases](https://www.ncbi.nlm.nih.gov/sites/GDSbrowser?acc=GDS5306)**: Analysis of HER2+ breast cancer brain metastasis specimens and HER2+ nonmetastatic primary breast tumors. Samples were matched for patient age upon primary tumor detection and ER status of primary tumor. Results provide insight into the molecular basis of HER2+ breast cancer outgrowth in the brain. Given these information, how one can recognize HER-2 type genes from the dataset? Also, how one can determine whether a predictive classifier adds predictive value to standard prognostic factors?

## Correspondence
* **Topic summarization**: given a set of messages, identify major topics.

### Relevant data sets
* **[Enron emails](https://www.cs.cmu.edu/~./enron/)**: a set of about 500K emails from Enron executives. Enron is a US energy company that was the subject of a federal investigation.

## Customer service
* **Request triage**: given request text and the customer's history with the company (purchases and previous communications) categorize the request by topic. 

## Cyber Security
* **Privacy Preservance**
* **Privacy Assurance**
* **Intrusion Detection**
* **Phishing Detection**

### Relevant data sets
* **[KDD CUP 99](http://kdd.ics.uci.edu/databases/kddcup99/kddcup99.html)**: The task is to develop to detect network intrusions that protects a computer network from unauthorized users, including perhaps insiders.  The intrusion detector learning task is to build a predictive model (i.e. a classifier) capable of distinguishing between _bad_ connections, called intrusions or attacks, and _good_ normal connections. The 1998 DARPA Intrusion Detection Evaluation Program was prepared and managed by MIT Lincoln Labs. The objective was to survey and evaluate research in intrusion detection.  A standard set of data to be audited, which includes a wide variety of intrusions simulated in a military network environment, was provided.  The 1999 KDD intrusion detection contest uses a version of this dataset.
* **[NSL-KDD](https://www.unb.ca/cic/datasets/nsl.html)**: NSL-KDD is a data set suggested to solve some of the inherent problems of the KDD'99 data set. Although, this new version of the KDD data set still suffers from some of the problems discussed by McHugh and may not be a perfect representative of existing real networks, because of the lack of public data sets for network-based IDSs, the authors of this data set believe it still can be applied as an effective benchmark data set to help researchers compare different intrusion detection methods. Furthermore, the number of records in the NSL-KDD train and test sets are reasonable. This advantage makes it affordable to run the experiments on the complete set without the need to randomly select a small portion. Consequently, evaluation results of different research work will be consistent and comparable.
* **[UNSW-NB15](https://www.unsw.adfa.edu.au/unsw-canberra-cyber/cybersecurity/ADFA-NB15-Datasets/)**: This data set is an advancement over the above-mentioned two data sets i.e. KDD CUP 99 and NSL-KDD. It captures more realistic features and way more instances than the other two. 
* **[Phishing Websites](https://archive.ics.uci.edu/ml/datasets/phishing+websites)**: In this dataset, the authors shed light on the important features that have proved to be sound and effective in predicting phishing websites. In addition, they proposed some new features.

## Economic development

## Finance
* **Loan repayment**: given an individual's financial history, predict the likelihood that they will successfully repay a loan.
* **Loan approval**: given an individual's information (such as Self_Employed, Loan_Amount_Term, Credit_History etc), predict if a loan application will be approaved or not. 
* **Credit card approval**: given an individual's information, predict a credit card application will be approved or not. 

### Relevant data sets
* **[Loan prediction](https://datahack.analyticsvidhya.com/contest/practice-problem-loan-prediction-iii)**
* **[Credit card approval data set](https://archive.ics.uci.edu/ml/datasets/credit+approval)**

## Humanitarian

## Information
* **Search**: given a set of search terms, return a set of documents ordered by relevance. 

## Insurance
* **Disaster modeling**: given the history of disaster occurrences, predict the likelihood that a similar disaster will occur again within a given time window.


## Internet of Things
* **Device health**: given a stream of device data, determine whether it is working as intended.
* **Predictive maintenance**: given a stream of device data, anticipate when repair or maintenance will be necessary.
* **Device comparisons**: given a collection of device data streams from two different hardware/software/environment conditions, determine which is working better.

### Relevant data sets
* **[Industrial Internet of Things Data](https://www.kaggle.com/pitasr/industrialiot): Industrial demand/response IoT data for IoT analytics.


## Legal
* **Topic retrieval**: given a topic, find documents and selections focused on it.
* **Hierarchical topic modeling**: given a set of documents, find major topics discussed and the subtopics under each.

### Relevant data sets
* **[Caselaw Access Project](https://case.law/)**: includes all official, book-published United States case law — every volume designated as an official report of decisions by a court within the United States.

## Media
* **Content recommendation**: given a set of recently viewed documents, return a set of documents ordered by relevance.

### Relevant data sets
* **[MovieLens 20M Dataset](https://www.kaggle.com/grouplens/movielens-20m-dataset)**: The datasets describe ratings and free-text tagging activities from MovieLens, a movie recommendation service. It contains 20000263 ratings and 465564 tag applications across 27278 movies. These data were created by 138493 users between January 09, 1995 and March 31, 2015. This dataset was generated on October 17, 2016. Some ideas worth exploring: 1. Which genres receive the highest ratings? How does this change over time? 2. Determine the temporal trends in the genres/tagging activity of the movies released

## Medicine
* **Detecting medical conditions in radiographs**: given a set of X-rays, determine whether each is indicative of the condition of interest.
* **Detecting malaria from blood smear**: given a patient’s blood smear predict if its malaria infected or not.
* **Predicting liklihood of medical condition**: given values for a set of patient risk factors, predict the likelihood that a given medical condition will manifest.

### Relevant data sets
* **[Breast Cancer Data Set](http://archive.ics.uci.edu/ml/datasets/Breast+Cancer)**: includes information about the breast cancer screening of several female patients. Hosted on UCI. 
* **[Diabetic retinopathy images](https://www.kaggle.com/c/diabetic-retinopathy-detection/data)**: a collection of retinal images, each labeled with its retinopathy scale score.
* **[The Human Microbiome Project](https://www.hmpdacc.org/)**: genetic sequences of microbes from hundreds of healthy individuals, across several different sites on the human body: nasal passages, oral cavity, skin, gastrointestinal tract, and urogenital tract.
* **[MIMIC-III Hospital admissions](https://mimic.physionet.org/)**: 58,000 hospital admissions for 38,645 adults and 7,875 neonates. [Access instructions](https://towardsdatascience.com/getting-access-to-mimic-iii-hospital-database-for-data-science-projects-791813feb735)(2012) 
* **[Pima diabetes database](https://www.kaggle.com/uciml/pima-indians-diabetes-database)**: includes BMI, insulin level, age, number of pregnancies, and diabetes diagnosis from female patients of Pima Indian heritage. Hosted on Kaggle.
* **[Malaria data set](https://ceb.nlm.nih.gov/repositories/malaria-datasets/)

## Politics
* **Voter turnout**: given an individual's voting history, predict whether they will vote in the next election.

## Retail
* **Product recommendation**: given a set of past purchases, return a set of products ordered by relevance.
* **Demand forecasting**: given a history of purchases, make predictions for future purchase volumes over time.

### Relevant data sets
* **[Instacart grocery purchases](https://www.instacart.com/datasets/grocery-shopping-2017)**: 3 Million Instacart Orders. (2017)
* **[UK retailer transactions](https://www.kaggle.com/carrie1/ecommerce-data)** "This is a transactional data set which contains all the transactions occurring between 01/12/2010 and 09/12/2011 for a UK-based and registered non-store online retail.The company mainly sells unique all-occasion gifts. Many customers of the company are wholesalers." From UCI ML lab, hosted on Kaggle. (2011)
* **[Sales by store](https://www.kaggle.com/manjeetsingh/retaildataset)** historical sales data for 45 stores located in different regions. Hosted on Kaggle. (2013)
* **[Black Friday sales](https://www.kaggle.com/mehdidag/black-friday)** 550,000 items, 100,000 customers. Hosted on Kaggle. (2018)

## Social networks
* **Connection recommendation**: given an individual's current connections, return a set of potential connections ordered by relevance.
### Relevant data sets
* **[Facebook](https://snap.stanford.edu/data/ego-Facebook.html)** 'Circles' (or 'friends lists') from Facebook, collected from survey participants using the Facebook app. (2012)
* **[Twitter](https://snap.stanford.edu/data/ego-Twitter.html)**:  'Circles' (or 'lists') from Twitter, crawled from public sources. (2012)

## Sports

### Relevant data sets

## Transportation
* **Predictive maintenance**: given a vehicle's usage and maintenance history, predict a given failure is likely to next occur.
* **On-Time Performance**: Identify problematic parts of a transportation network causing delays, the root causes, and recommendations to improve on-time performance. 

### Relevant data sets
* **[SBB Swiss Federal Railways On-Time Performance](https://github.com/crowdAI/train-schedule-optimisation-challenge-starter-kit)**: CrowdAI challenge and data set to optimize punctuality of train schedules
