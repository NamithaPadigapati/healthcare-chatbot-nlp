🏥 Healthcare Chatbot for Symptom Analysis
![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![spaCy](https://img.shields.io/badge/spaCy-09A3D5?style=flat-square&logo=spacy&logoColor=white)
![Scikit-learn](https://img.shields.io/badge/Scikit--learn-F7931E?style=flat-square&logo=scikitlearn&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white)
📌 Project Overview
An intelligent healthcare chatbot that analyzes user-reported symptoms to predict possible conditions and triage urgency, supporting both text and voice input across mobile and web platforms.
---
🎯 Problem Statement
Patients often struggle to assess the urgency of their symptoms before seeking care. This project aimed to:
Provide instant symptom-based triage to guide users toward appropriate care
Support voice input for accessibility across devices
Deliver structured, reliable output using NLP pipelines
---
🛠️ Tech Stack
Layer	Tools
NLP Pipeline	spaCy
ML Models	SVM, Decision Tree
Speech Input	Speech-to-Text API
Data Processing	Python, pandas
Routing & API	Dynamic routing logic
---
📊 Approach
1. NLP Pipeline
Used spaCy for text preprocessing and entity extraction
Built structured output mapping from symptom text to condition categories
Handled varied user input formats (casual, clinical, abbreviated)
2. ML Models
Trained two classification models on symptom-condition pairs:
SVM (Support Vector Machine) — effective for high-dimensional text classification
Decision Tree — interpretable model for triage rule mapping
Evaluation metrics: Accuracy, Precision, Recall per condition class
3. Voice Input Integration
Integrated Speech-to-Text API for voice-based symptom input
Built dynamic routing to handle both voice and text input seamlessly
Optimized for mobile and web access
---
📈 Results
Feature	Outcome
Input Types	Text + Voice
Models	SVM + Decision Tree
NLP Framework	spaCy pipelines
Platform Support	Mobile + Web
---
📁 Project Structure
```
healthcare-chatbot-nlp/
│
├── data/
│   └── symptom_condition_pairs.csv   # Training dataset
│
├── notebooks/
│   └── symptom_analysis.ipynb        # Model training notebook
│
├── app/
│   ├── chatbot.py                    # Core chatbot logic
│   ├── nlp_pipeline.py               # spaCy NLP pipeline
│   └── voice_input.py                # Speech-to-text integration
│
├── models/
│   └── svm_model.pkl                 # Saved trained model
│
└── README.md
```
---
🚀 How to Run
```bash
# 1. Clone the repo
git clone https://github.com/NamithaPadigapati/healthcare-chatbot-nlp.git

# 2. Install dependencies
pip install -r requirements.txt

# 3. Download spaCy model
python -m spacy download en_core_web_sm

# 4. Run the chatbot
python app/chatbot.py
```
---
💡 Key Takeaways
NLP pipelines significantly improve symptom extraction accuracy over keyword matching
SVM outperforms Decision Tree on unseen symptom variations
Voice input dramatically improves accessibility for non-technical users
