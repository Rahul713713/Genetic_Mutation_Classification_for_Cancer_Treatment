# Genetic Mutation Classification for Cancer Treatment : Project Overview
![Genetic_Mutation_Classification](https://github.com/Rahul713713/Genetic_Mutation_Classification_for_Cancer_Treatment/blob/main/CancerTreatment.jpg "Genetic Mutation Classification for Cancer Treatment")
- Created multiple charts,graphs,countplots,etc. in order to understand the data as this was a multiclass classification problem.
- Worked on a dataset consisting of 3321 rows of data for 4 different features.
- All the features are either categorical or text features.
- Performed univariate analysis on various features and also made machine learning models just with a specific feature  to understand the importance of every feature.
- Used Natural language techniques like TfifdVectorizer to converted text data into numerical data.
- Performed Data Analysi and Exploratory Data Analysis
- Used multiple Machine Learning Models like Naïve Bayes, KNN, Logistic Regression,etc. to solve this problem.

# Problem Statement
Once sequenced, a cancer tumor can have thousands of genetic mutations. But the challenge is distinguishing the mutations that contribute to tumor growth (drivers) from the neutral mutations (passengers).
Currently this interpretation of genetic mutations is being done manually. This is a very time-consuming task where a clinical pathologist has to manually review and classify every single genetic mutation based on evidence from text-based clinical literature.
For this competition MSKCC is making available an expert-annotated knowledge base where world-class researchers and oncologists have manually annotated thousands of mutations.
We need your help to develop a Machine Learning algorithm that, using this knowledge base as a baseline, automatically classifies genetic variations.

Classify the given genetic variations/mutations based on evidence from text-based clinical literature.

# Code and Resources Used
- Packages: pandas, numpy, matplotlib, seaborn, nltk,scikit-learn

# Data Cleaning and Preprocessing
## After reading the data, I needed to clean it up so that it would be fit for our data analysis. I made the following changes and created the following variables:
- Checked whether we have missing data for various columns.
- Replaced the missing values. 
- Cleaned the text data during text preprocessing
- Finally,the columns used for building the models are

 1   ID             
 2   Gene              
 3   Variation         
 4   Text        
 5   Class                 

# Machine Learning Models
- The Machine Learning Models that I've used are as follow:

 1   Naive Bayes             
 2   KNN              
 3   Logistic Regression With Class balancing            
 4   Logistic Regression Without Class balancing         
 5   Linear SVC With Class Balancing           
 6   Random Forest Classifier      

# Result
    +--------------------------------------------------------------------------------------------+
    |                    *** Model Summary *** [Performance Metric: Log-Loss]                    |
    +---------------------------------------------+-------+------+------+------------------------+
    |                  Model Name                 | Train |  CV  | Test | % Misclassified Points |
    +---------------------------------------------+-------+------+------+------------------------+
    |                 Naive Bayes                 |  0.94 | 1.21 | 1.24 |           43           |
    |                     KNN                     |  0.99 | 1.28 | 1.33 |           44           |
    |   Logistic Regression With Class balancing  |  0.50 |  1   | 1.08 |           37           |
    | Logistic Regression Without Class balancing |  0.5  | 1.03 | 1.09 |           36           |
    |       Linear SVC With Class Balancing       |  0.54 | 1.07 | 1.12 |           36           |
    |           Random Forest Classifier          |  0.65 | 1.16 | 1.18 |           38           |
    +---------------------------------------------+-------+------+------+------------------------+

### Confusion Matrix for Logistic Regression With Class balancing 
![Genetic_Mutation_Classification](https://github.com/Rahul713713/Genetic_Mutation_Classification_for_Cancer_Treatment/blob/main/Confusion_Matrix.png "Confusion Matrix for logistic Regression with class balancing")
