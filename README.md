# AutoJudge-Predicting-Programming-Problem-Difficulty
## 📌 Project Overview

 AutoJudge is an AI-powered system that predicts the difficulty level of competitive programming problems as Easy, Medium, or Hard.
 
 It analyzes the problem statement, input description, and output description using Natural Language Processing (NLP) and Machine Learning models.
 
 In addition to classification, AutoJudge also generates a continuous difficulty score, making the system more informative and closer to real-world judging platforms.

## 📊 Dataset Used

 The dataset consists of competitive programming problems with:
 
    - Problem description
    
    - Input description
    
    - Output description
    
    - Constraints
    
    - Difficulty label (Easy / Medium / Hard)
    
    - Difficulty score (numerical)

## 📌Preprocessing performed:

    -Text cleaning and normalization
    
    -Stopword removal
    
    -Lemmatization
    
    -Class distribution analysis
    
    -Feature selection using Random Forest importance

## 🧠 Approach & Models Used

### 🔹 Feature Engineering

    -TF-IDF Vectorization for textual features
    
    -Handcrafted numerical features:
    
        -Text length
        
        -Count of mathematical symbols
        
        -Constraint magnitude extraction
        
    -Keyword-based features (DP, graph, tree, greedy, etc.)

### 🔹 Models
    -Classifier: Random Forest Classifier
    
      → Predicts difficulty category (Easy / Medium / Hard)
    
    -Regressor: Machine Learning Regression Model
    
      → Predicts a continuous difficulty score
    
  -Feature selection using Random Forest significantly improved model performance.

## 📈 Evaluation Metrics

    Classification: Accuracy ~ 54%
    
    Regression:
    
      Mean Absolute Error (MAE) ~ 2.5
      
      Root Mean Squared Error (RMSE) ~ 3.1
    
    Performance improvements were observed after feature selection and engineered features.

## 🖥️ Web Interface (Streamlit)

   The project includes an interactive Streamlit web application that:
   
       Accepts problem description, input format, and output format
       
       Predicts:
       
          Difficulty Level (Easy / Medium / Hard)
          
          Difficulty Score
          
       Displays results using a modern glassmorphism UI
   
   UI Highlights:
   
     Gradient-based theme
     
     Real-time predictions
     
     Visual progress indicator for difficulty score

## 🚀 Steps to Run the Project Locally

  1️⃣ Clone the Repository
  
      git clone <repo-link>
      
      cd AutoJudge
  
  2️⃣ Install Dependencies
  
     pip install -r requirements.txt
  
  3️⃣ Run the Streamlit App
  
     streamlit run app.py
  
  4️⃣ Open in Browser
  
     http://localhost:8501

## 🎥 Demo Video

📌 2–3 Minute Demo Video:

  👉 

## 👩‍💻 Author Details

    Name: Sushma
    
    Domain: Machine Learning, NLP, Web Deployment
    
    Tools Used: Python, Scikit-learn, NLTK, Streamlit
    
