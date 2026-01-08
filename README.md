# AutoJudge-Predicting-Programming-Problem-Difficulty
## 📌 Project Overview

 AutoJudge is an AI-powered system that predicts the difficulty level of competitive programming problems as Easy, Medium, or Hard.
 
 It analyzes the problem statement, input description, and output description using Natural Language Processing (NLP) and Machine Learning models.
 
 In addition to classification, AutoJudge also generates a continuous difficulty score, making the system more informative and closer to real-world judging platforms.

## 📊 Dataset Used

 The dataset consists of competitive programming problems with:
 
  • Problem description
  
  • Input description
  
  • Output description
  
  • Constraints
  
  • Difficulty label (Easy / Medium / Hard)
  
  • Difficulty score (numerical)

## 📌Preprocessing performed:

  • Text cleaning and normalization
  
  • Stopword removal
  
  • Lemmatization
  
  • Class distribution analysis
  
  • Feature selection using Random Forest importance

## 🧠 Approach & Models Used

### 🔹 Feature Engineering

  • TF-IDF Vectorization for textual features
  
  • Handcrafted numerical features:
  
   -Text length
   
   -Count of mathematical symbols
   
   -Constraint magnitude extraction
    
  • Keyword-based features (DP, graph, tree, greedy, etc.)

### 🔹 Models
  • Classifier: Logistic Regression & Random Forest Classifier
  
   → Predicts difficulty category (Easy / Medium / Hard)
  
  • Regressor: Linear Regression Model
  
   → Predicts a continuous difficulty score
   
 • Feature selection using Random Forest significantly improved model performance.

## 📈 Evaluation Metrics

  • Classification: Accuracy ~ 54% by Random Forest Classifier  & ~ 50% by Logistic Regression
  
  • Regression: Linear Regression Model
  
  -Mean Absolute Error (MAE) ~ 2.5
   
  -Root Mean Squared Error (RMSE) ~ 3.1
  
  • Performance improvements were observed after feature selection and engineered features.

## 🖥️ Web Interface (Streamlit)

 • The project includes an interactive Streamlit web application that:
 
   • Accepts problem description, input format, and output format
   
   • Predicts:
   
   -Difficulty Level (Easy / Medium / Hard)
    
   -Difficulty Score
      
   • Displays results using a modern glassmorphism UI

 • UI Highlights:
 
   -Gradient-based theme
   
   -Real-time predictions
   
   -Visual progress indicator for difficulty score

## Project Structure & Pipeline
     AutoJudge-Predicting-Programming-Problem-Difficulty/
     │
     ├── Dataset/
     │   ├── problems_data.jsonl
     ├── Results/
     │   ├── Screenshot_2026-01-08_012240.png
     │   ├── Screenshot_2026-01-08_012305.png
     │   ├── Screenshot_2026-01-08_012313.png
     │   ├── Screenshot_2026-01-08_012322.png
     │   ├── Screenshot_2026-01-08_021056.png
     │   └── Screenshot_2026-01-08_021107.png
     │
     ├── models/
     │   ├── classifier.pkl      # Trained difficulty classification model
     │   ├── regressor.pkl       # Trained difficulty score regression model
     │   └── vectorizer.pkl      # TF-IDF text vectorizer
     │
     ├── src/
     │   └── Complete_Source_Code_Notebook.ipynb     # Data Preprocessing and Feature Extraction along with model training are done in this notebook.
     │
     ├── ACM_Report.pdf
     ├── README.md
     ├── app.py
     └── requirements.txt

## 🚀 Steps to Run the Project Locally

  1️⃣ Clone the Repository
  
      git clone https://github.com/sushma077/AutoJudge-Predicting-Programming-Problem-Difficulty-.git
      
      cd AutoJudge-Predicting-Programming-Problem-Difficulty-
  
  2️⃣ Install Dependencies
  
     pip install -r requirements.txt
  
  3️⃣ Run the Streamlit App
  
     streamlit run app.py
  
  4️⃣ Open in Browser
  
     http://localhost:8501

## 🎥 Demo Video

📌 Demo Video link:

  👉 https://drive.google.com/file/d/1eEXUlQe-tlfCeS1N8ralLS-UGqcSy-Ld/view?usp=drivesdk

## 👩‍💻 Author Details

  • Name: Sushma

  • Enrollment Number: 23115149
  
  • Domain: Machine Learning, NLP, Web Deployment
  
  • Tools Used: Python, Scikit-learn, NLTK, Streamlit
    
