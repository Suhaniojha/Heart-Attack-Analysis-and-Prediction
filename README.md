# Heart Attack Analysis & Prediction

## 🧠 Project Overview
This project focuses on **predicting the likelihood of a heart attack** in patients using **machine learning techniques**. The model analyzes various health indicators and medical test results to assist in **early risk detection**.

The dataset includes features such as **age, cholesterol, chest pain type, blood pressure, maximum heart rate achieved, ST depression, thalassemia, and number of major blood vessels**, along with the **target variable** indicating whether the patient had a heart attack.

---

## 📊 Dataset Features
| Feature | Description |
|---------|-------------|
| `age` | Age of the patient in years |
| `sex` | Gender of the patient |
| `cp` | Chest pain type (0: Typical angina, 1: Atypical angina, 2: Non-anginal pain, 3: Asymptomatic) |
| `trestbps` | Resting blood pressure (mm Hg) |
| `chol` | Serum cholesterol (mg/dL) |
| `fbs` | Fasting blood sugar > 120 mg/dL (1 = true; 0 = false) |
| `restecg` | Resting ECG results |
| `thalachh` | Maximum heart rate achieved |
| `exang` | Exercise-induced angina (1 = yes, 0 = no) |
| `oldpeak` | ST depression induced by exercise relative to rest |
| `slope` | Slope of the peak exercise ST segment |
| `caa` | Number of major vessels colored by fluoroscopy (0-3) |
| `thall` | Thalassemia test result |
| `target` | Heart attack occurrence (0 = No, 1 = Yes) |

---

## 🛠 Technologies Used
- **Python**  
- **Pandas, NumPy** – for data handling and analysis  
- **Matplotlib, Seaborn** – for data visualization  
- **Scikit-learn** – for machine learning models  
- **Models implemented:**  
  - Logistic Regression  
  - Random Forest Classifier  

---

## 🚀 Project Workflow
1. **Data Preprocessing**
   - Handling missing values
   - Encoding categorical features
   - Feature scaling for models like Logistic Regression
   - Train-test split

2. **Model Training**
   - Logistic Regression as a baseline
   - Random Forest for better accuracy and handling non-linear relationships

3. **Model Evaluation**
   - Metrics used: **Accuracy, Precision, Recall, F1-Score, ROC-AUC**
   - Random Forest achieved **high recall for detecting heart attack cases**, which is crucial for medical applications

4. **Feature Importance**
   - Analyzed which health indicators contribute most to predictions
   - Features like `oldpeak`, `thalachh`, `chol`, and `age` were most important

---

## 📈 Results
| Model | Accuracy | Recall (Heart Attack) | ROC-AUC |
|-------|---------|----------------------|---------|
| Logistic Regression | ~84% | 97% | 0.91 |
| Random Forest | ~84% | 97% | 0.91 |

**Observation:**  
- Random Forest handled non-linear relationships better and provided feature importance insights.  
- High recall ensures **minimal false negatives**, critical in medical predictions.

---

## ⚡ How to Run
1. Clone the repository:
```bash
git clone https://github.com/Suhaniojha/Heart-Attack-Analysis-and-Prediction.git
