# Student-performance-prediction-project

Student Performance Prediction App

A web-based application built using **Streamlit** and **Machine Learning** to predict student performance based on various academic and socio-demographic features. This project enables both **classification (Pass/Fail)** and **regression (score prediction)** using a **Random Forest model**, and provides powerful **data visualization** tools.

## Features
* Predicts whether a student will **Pass** or **Fail**
* Estimates the **exam score**
* Uses **Random Forest** for classification and regression
* Offers interactive **data visualizations** (heatmaps, bar charts, scatter plots, etc.)
* Supports **custom input** for prediction
* Uses preprocessed CSV dataset with added target column
* Displays GIFs based on prediction results (Pass/Fail)

## Tech Stack
| Tool                     | Usage                        |
| ------------------------ | ---------------------------- |
| **Python**               | Core programming language    |
| **Streamlit**            | Web app interface            |
| **Pandas**               | Data manipulation            |
| **Seaborn & Matplotlib** | Data visualization           |
| **Scikit-learn**         | ML algorithms and evaluation |
| **NumPy**                | Numerical computations       |

## Dataset
Two datasets were used:
1. UCI Student Performance Dataset
   * Source: [UCI Repository](https://archive.ics.uci.edu/ml/datasets/Student+Performance)
   * Attributes: demographics, academics, lifestyle (33 features)

2. Kaggle Student Performance Dataset
   * Source: [Kaggle](https://www.kaggle.com/datasets/spscientist/students-performance-in-exams)
   * Attributes: scores in math/reading/writing, demographics

The combined CSV file used in this app is `StudentPerformanceFactors.csv`.

## Installation

git clone https://github.com/your-username/student-performance-prediction.git
cd student-performance-prediction
pip install -r requirements.txt
streamlit run app.py

## File Structure
├── app.py                         # Main Streamlit application
├── StudentPerformanceFactors.csv  # Dataset used for training/prediction
├── style.css                      # Custom Streamlit styling
├── image_home.jpeg                # Image for home page
├── pass.gif                       # GIF shown on successful prediction
├── fail.gif                       # GIF shown on failed prediction
├── requirements.txt               # Python package dependencies

## Models Used
* Classification: `RandomForestClassifier` (Pass/Fail)
* Regression: `RandomForestRegressor` (Score prediction)
* Evaluation Metrics:

  * Accuracy for classification
  * RMSE for regression

## Results
| Model Type     | Algorithm     | Metric   | Result |
| -------------- | ------------- | -------- | ------ |
| Classification | Random Forest | Accuracy | \~87%  |
| Regression     | Random Forest | RMSE     | \~1.75 |

## Team
Developed as part of a Mini Project for B.E. in Artificial Intelligence & Machine Learning at **Canara Engineering College**.
* Reeshal Dsouza (4CB23AI079)
* Sanjana Mahale (4CB23AI087)
* Vrinda Bhaskar Kumtakar (4CB23AI125)

Under the guidance of:
Mr. Arjun K, Assistant Professor, Dept. of AIML

## Future Work
* Add real-time prediction APIs
* Integrate psychological or behavioral metrics
* Deploy on cloud platforms
* Improve model accuracy using ensemble techniques

