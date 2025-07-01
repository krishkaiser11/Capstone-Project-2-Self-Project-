# 📊 Capstone Project 2 – AI Tool Usage by Indian College Students (2025)

This capstone project explores how Indian college students are using AI tools (e.g., ChatGPT, Gemini, Copilot) for academic purposes. The dataset was collected in May 2025 via a survey and includes 496 students across various streams and years of study.

---

## 📁 Dataset Overview

- **Rows**: 496
- **Columns**: 16
- **Source**: Google Forms Survey (May 2025)
- **File Used**: `Students.csv`

**Key Features:**
- `Year_of_Study`, `Daily_Usage_Hours`, `Trust_in_AI_Tools`, `Awareness_Level`, `Impact_on_Grades`
- AI tools used, use cases, professor approval, device type, internet quality

---

## 🧪 Project Workflow

This project follows a structured data science lifecycle:

### 1. Data Exploration & Cleaning
- Loaded and inspected dataset
- Handled missing values (median/mode imputation)
- Removed duplicate rows
- Applied one-hot encoding to categorical features

### 2. Visualization (Matplotlib/Seaborn)
- Distribution plots (histograms, boxplots)
- Categorical plots (bar, pie charts)
- Correlation heatmaps and pair plots

### 3. Feature Engineering
- Created interaction and polynomial features
- Removed binary columns from scaling
- Applied **StandardScaler** to continuous variables

### 4. Model Building & Evaluation
- Models used:
  - Linear/Logistic Regression (baseline)
  - Decision Tree
  - Random Forest
  - K-Nearest Neighbors
- Performance Metrics:
  - **Regression**: RMSE, R²
  - **Classification**: Accuracy, F1-Score
- Visual performance comparison using bar plots

### 5. Hyperparameter Tuning
- Used `RandomizedSearchCV` for regression models
- Used `GridSearchCV` for classification
- Evaluated tuned models against baseline

---

## 📈 Power BI / Tableau Visualization

The cleaned dataset was exported as: cleaned_preprocessed_students_data.csv (not getting uploaded in github due to its large size)
---

Imported into Tableau/Power BI to build interactive dashboards showing:
- Trust level vs. Usage Hours
- Distribution of Preferred AI Tools
- Year-wise awareness
- Impact of device and internet access on grades

---

## 📝 Final Results & Insights

- **2nd Year students** showed the highest AI tool usage.
- Most students preferred **ChatGPT** and trusted AI tools with high confidence (Trust = 5).
- Random Forest (tuned) achieved the best prediction performance.
- High AI awareness and usage hours were moderately correlated with grade improvement.

---

## 📂 Repository Structure

├── Capstone2_AI_Student_Usage.ipynb # Main Jupyter notebook
├── Students.csv # Raw dataset
├── cleaned_preprocessed_students_data.csv # Exported for visualization
├── README.md # Project overview

