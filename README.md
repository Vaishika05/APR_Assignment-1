# Titanic Survival Prediction using Logistic Regression

## Overview
This project predicts the survival of passengers on the Titanic using **Logistic Regression**. The dataset includes passenger information such as age, gender, ticket class, number of siblings/spouses aboard, fare, and port of embarkation.  

The goal is to build a model that can classify whether a passenger survived (`1`) or did not survive (`0`) the Titanic disaster.  

---

## Dataset
- **Number of Records:** 891 passengers  
- **Features:**
  - `Pclass`: Passenger class (1st, 2nd, 3rd)  
  - `Sex`: Male/Female  
  - `Age`: Passenger age  
  - `SibSp`: Number of siblings/spouses aboard  
  - `Parch`: Number of parents/children aboard  
  - `Fare`: Ticket fare  
  - `Embarked`: Port of embarkation (C, Q, S)  
- **Target:** `Survived` (0 = Did not survive, 1 = Survived)  

---

## Preprocessing
- Filled missing values:
  - `Age` → median value  
  - `Embarked` → mode value  
- Dropped columns with too many missing or irrelevant values: `Cabin`, `Ticket`, `Name`  
- Encoded categorical variables:
  - `Sex` → 0 = male, 1 = female  
  - `Embarked` → one-hot encoding  

---

## Model
- **Algorithm:** Logistic Regression  
- **Train/Test Split:** 80% train, 20% test  
- **Library:** Scikit-learn  

---

## Evaluation
- **Metrics Used:**  
  - Accuracy  
  - Confusion Matrix  

- **Training Accuracy:** ~80%  
- **Testing Accuracy:** ~78%  

- **Observations:**
  - The model performs well and generalizes properly.  
  - Gender, Age, and Passenger Class are significant features influencing survival.  

---

## How to Run
1. Clone this repository:  
   ```bash
   git clone https://github.com/Vaishika05/APR_Assignment-1.git
