# End to End Machine Learning Project

This project demonstrates an end-to-end Machine Learning workflow using Python and scikit-learn.  
The main goal is to build a modular ML pipeline for predicting students' math scores based on demographic and academic features.

The project focuses on:
- Clean project structure
- Modular components
- Data preprocessing and transformation
- Model training and evaluation

---

## Project Overview

The model predicts **math_score** using the following features:

- gender  
- race_ethnicity  
- parental_level_of_education  
- lunch  
- test_preparation_course  
- reading_score  
- writing_score  

The project is organized as a real-world style ML system with separate modules for data ingestion, transformation, training and utilities.

---

## ML Workflow

1. Data Ingestion  
2. Data Transformation  
   - Handling missing values (SimpleImputer)  
   - Scaling numerical features  
   - One-hot encoding categorical features  
3. Model Training  
4. Model Evaluation  
5. Saving trained artifacts  

---

## Project Structure
```
│
├── artifacts/
├── logs/
├── src/
│ ├── components/
│ │ ├── data_ingestion.py
│ │ ├── data_transformation.py
│ │ └── model_trainer.py
│ │
│ ├── pipeline/
│ │ └── predict_pipeline.py
│ │
│ ├── notebook/
│ │ └── EDA.ipynb
│ │ └── Model_Training.ipynb
│ │
│ ├── exception.py
│ ├── logger.py
│ └── utils.py
│
├── requirements.txt
├── setup.py
└── README.md
```

---

## Tech Stack

- Python  
- NumPy  
- Pandas  
- Scikit-learn  
- Seaborn  
- Matplotlib  

---

## Dataset

Student Performance Dataset containing demographic information and exam scores.

Target variable:
- math_score  

---

## How to Run the Project

1. Clone the repository:
```
git clone https://github.com/katarinatomasevic/ml-project.git
cd mlproject
```
2. Create and activate environment
```
conda create -p venv python=3.10 -y
conda activate ./venv
```
3. Install dependencies
```
pip install -r requirements.txt
```
4. Run training pipeline
```
python src/pipeline/train_pipeline.py
```


---

## Key Features

- Modular code structure
- Pipelines for preprocessing and training  
- Handling missing values  
- Prevents data leakage  
- Logging and custom exception handling  
- Easily extendable  

---

## Models Used

- Linear Regression  
- Gradient Boosting
- K-Nearest Neighbors  
- Decision Tree  
- Random Forest  
- AdaBoost  
- XGBoost  
- CatBoost  

---
