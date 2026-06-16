# HCI Project: Analyzing Key Determinants of Chatbot-Human Interaction

This repository contains the complete workflow for an HCI (Human-Computer Interaction) research project aimed at understanding which target variables most significantly affect the quality and outcomes of human-chatbot interactions. By compiling existing academic literature, binary-coding qualitative factors, and evaluating multiple machine learning models, this project identifies the strongest predictors of successful human-AI engagement.

## Project Overview
Human-Chatbot Interaction is highly dependent on a variety of design, psychological, and contextual factors. This project systematic reviews existing literature to extract these variables, preprocesses the data through binary encoding, and utilizes predictive modeling to determine which specific variables yield the highest predictive accuracy regarding interaction success.

The workflow consists of:
1. **Literature Synthesis:** Reviewing research papers across multiple platforms to build a comprehensive literature matrix.
2. **Data Engineering:** Binary coding the extracted qualitative metrics for machine learning readiness.
3. **Model Evaluation:** Training and simulating multiple ML models to identify the highest-performing architecture and uncover the most impactful target variables.

---

## Repository Structure

* `Research Proposal (1).docx` - The foundational research framework, objectives, and methodology for this HCI study.
* `electronics-11-01579-with-cover.pdf` - Core reference literature utilized in the research scaffolding.
* `Literature Matrix.xlsx` - Compiled data extracted from various academic research papers across multiple platforms.
* `Preprocessing.ipynb` & `preprocessing simulation.html` - Jupyter notebook and HTML simulation showing the data cleaning, feature extraction, and binary encoding process.
* `Dataset after Preprocessing.xlsx` & `Chatbot_Binary_Dataset.xlsx` - The finalized, cleaned, and binary-coded datasets used for model training.
* `Chatbot_ML_Models.ipynb` & `ML_Models_Simulation.html` - Notebook and simulation containing the machine learning pipeline, model training, evaluation metrics, and accuracy comparisons.

---

## Methodology and Workflow

### 1. Literature Review & Matrix Extraction
We compiled papers from major academic repositories focusing on conversational AI and HCI. Key factors influencing user experience, trust, error rates, and engagement were systematically logged into the **Literature Matrix**.

### 2. Binary Encoding & Preprocessing
To transform qualitative research insights into a machine-readable format, the variables were converted into binary features ($0$ or $1$) representing the absence or presence of specific interaction attributes. 
* Details can be tracked in `Preprocessing.ipynb`.

### 3. Machine Learning & Accuracy Evaluation
We trained multiple classification models to determine which setup best predicts optimal chatbot-human interaction outcomes. The models evaluated include:
* Logistic Regression
* Decision Trees / Random Forests
* Support Vector Machines (SVM)
* Gradient Boosting
* Neural Networks

The feature importance metrics from the highest-accuracy model were used to isolate the core target variables that influence human-chatbot dynamics the most.

---

## How to Use This Repository

### Prerequisites
To run the notebooks locally, ensure you have Python installed along with the following libraries:
```bash
pip install pandas numpy scikit-learn matplotlib seaborn openpyxl
