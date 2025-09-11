# **Estimation of Obesity Levels Based On Eating Habits and Physical Condition**
This project presents a machine learning approach to a multiclass classification problem. The goal is to classify each individual in the dataset into one of seven obesity levels, ranging from insufficient weight to obesity type III, based on the target variable NObesity.
The dataset consists of 2,111 instances (individuals) from Mexico, Peru, and Colombia, described by 17 features related to lifestyle habits and physical conditions that may influence the obesity level. 

| Feature | Description |
|---------|-------------|
| **Gender** | Biological sex of the individual |
| **Age** | Age of the individual (14–61 years) |
| **Height** | Height of the individual in meters |
| **Weight** | Weight of the individual in kilograms |
| **Family history with overweight** | Binary variable indicating whether any family member has suffered or suffers from overweight |
| **FAVC (Frequent consumption of high caloric food)** | Frequency of consuming high-calorie foods |
| **FCVC (Frequency of consumption of vegetables)** | Frequency of consuming vegetables |
| **NCP (Number of main meals)** | Number of main meals consumed daily |
| **CAEC (Consumption of food between meals)** | Indicates whether the individual eats between main meals |
| **SMOKE** | Indicates whether the individual smokes |
| **CH2O (Consumption of water daily)** | Daily water consumption in liters |
| **SCC (Calories consumption monitoring)** | Indicates whether the individual monitors calorie intake |
| **FAF (Physical activity frequency)** | Frequency of physical activity or exercise |
| **TUE (Time using technology devices)** | Daily time spent using technology devices |
| **CALC (Consumption of alcohol)** | Indicates whether the individual consumes alcohol |
| **MTRANS (Transportation used)** | Main mode of transportation used (bike, motorbike, walking, automobile, public transportation) |
| **NObeyesdad (Target)** | Classification of the individual’s obesity level |

### Obesity Levels (Target Classes)
The **NObeyesdad** variable includes the following 7 categories:
- **Insufficient Weight**  
- **Normal Weight**  
- **Overweight Level I**  
- **Overweight Level II**  
- **Obesity Type I**  
- **Obesity Type II**  
- **Obesity Type III** 


The dataset used can be found in the **UC Irvine Machine Learning Repository**:
[Estimation of Obesity Levels Based On Eating Habits and Physical Condition](https://archive.ics.uci.edu/dataset/544/estimation+of+obesity+levels+based+on+eating+habits+and+physical+condition).

More information about the creation of the dataset can be found in this [article](https://doi.org/10.1016/j.dib.2019.104344).


## **Project Pipeline**

1. **Data Loading and Exploration**
   - Load the dataset into a Pandas DataFrame  
   - General functions to explore the dataset  

2. **Exploratory Data Analysis (EDA)**
   - Visualize the distribution of obesity levels  
   - Analyze skewness of variables  
   - Use histograms, box plots, density plots for feature distributions  
   - Generate a correlation matrix to identify feature relationships  

3. **Data Preparation**
   - Split data into training and test sets  
   - Apply preprocessing: StandardScaler (numerical features) and OneHotEncoder (categorical features)  
   - Perform feature selection (RFE, SelectKBest)  

4. **Baseline Model Training and Evaluation**
   - Train Logistic Regression (LR) on:  
     - Full feature set  
     - Reduced feature set (after selection)  
   - Compare performance to decide which feature set to use for subsequent models  

5. **Model Training, Comparison & Hyperparameter Tuning**
   - Training with multiple algorithms:  
     - Linear Discriminant Analysis (LDA)
     - Logistic Regression (LR)  
     - K-Nearest Neighbors (KNN)  
     - Decision Tree (CART)  
     - Gaussian Naive Bayes (NB)  
     - Support Vector Machine (SVM)  
   - Apply hyperparameter tuning  
   - Compare performance with metrics: Accuracy, Log Loss, AUC 

6. **Final Model Evaluation on Test Set**
   - Evaluate the selected model (**Logistic Regression**) on the test set  
   - Report performance metrics: Accuracy, Log Loss, AUC  
   - Visualize results with ROC curve and Confusion Matrix 


## Author

Martina Marotta

Project for AML Baic Course of Bioinformatics Master's degree at Bologna University
     








