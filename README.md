# Workforce Analytics Project  

## 📌 Overview  
This project investigates **employee attrition** and **workforce segmentation** using a combination of statistical analysis, predictive modelling, and clustering. The goal is to help organisations understand **who is leaving, who is leading, and what interventions can be taken** to improve retention and engagement.  

The work draws on a dataset of ~9,000 employees (2023 snapshot), combining demographic, career, and engagement features to:  
1. Identify key drivers of voluntary attrition.  
2. Segment employees into actionable clusters for targeted talent strategies.  

---

## 🗂 Project Structure  
- **latest_employee_records.xlsx** → Cleaned dataset with one record per employee.  
- **Technical Document.docx** → Methodology, EDA, statistical testing, and modelling details.  
- **Workforce Analytics (PDF)** → Final report with findings, insights, and recommendations.  
- **Visualisations & Models** → Attrition trends, logistic regression outputs, clustering (K-modes, t-SNE).  
- **Code Notebooks (Python)** → Scripts for preprocessing, EDA, statistical testing, logistic regression, and clustering.  

---

## 🔑 Key Use Cases  

### 1. **Voluntary Attrition Analysis**  
- **Problem:** Identify why employees resign voluntarily.  
- **Approach:**  
  - Compared characteristics of leavers vs stayers.  
  - Applied t-tests, chi-square, correlation, logistic regression, and random forest.  
- **Findings:**  
  - Leavers have fewer promotions (1.62 vs 2.47 for stayers).  
  - Attrition risk peaks in **1–3 years tenure** and dips after 10+ years.  
  - Managers & ERG (Employee Resource Group) members show **60–70% lower quit risk**.  
- **Recommendations:**  
  - Build **structured career pathways**.  
  - Strengthen **ERG membership & visibility**.  
  - Treat managers as **retention anchors**.  

---

### 2. **Workforce Segmentation (Clustering)**  
- **Problem:** Understand natural employee segments for personalised talent strategies.  
- **Approach:**  
  - K-modes clustering on categorical features.  
  - Chose **7 clusters** after elbow method and validation.  
- **Employee Segments Identified:**  
  - **Early Career Explorers** – high attrition risk, low tenure.  
  - **Consistent Managers** – stable, 5–10 yrs tenure, 3–4 promotions.  
  - **Legacy Leaders** – longest-tenured, highly promoted, influential.  
  - **Cultural Stewards** – engaged in BRGs, drive culture.  
  - **Emerging Talent** – top young employees, high flight risk.  
  - **Senior Talent Hires** – new senior recruits adapting to culture.  
  - **Emerging Leaders** – high-potential managers, key to future leadership pipeline.  

- **Why Prioritise Emerging Leaders?**  
  - 3–5 years tenure, already managers with 3–4 promotions.  
  - At risk of plateauing, but high ROI if engaged.  
  - Attrition drops significantly after 3+ promotions (protective factor).  
- **Recommendations:**  
  - Offer **strategic growth pathways** (cross-functional rotations, consulting sprints).  
  - Accelerate leadership readiness with **curated academies**.  
  - Recognise & increase **visibility in org-wide forums**.  

---

## 🛠️ Methodology  

1. **Data Processing**  
   - Collapsed monthly HR snapshots into one row per employee.  
   - Filtered out involuntary terminations.  
   - Converted features into categorical bands (tenure, age, promotions).  

2. **Exploratory Data Analysis (EDA)**  
   - Attrition rates by age, tenure, promotions, commute distance, ERG membership, manager role.  
   - Dual bar plots for headcount vs exits.  

3. **Statistical Testing**  
   - **t-tests** (continuous variables) and **chi-square** (categorical variables).  
   - Correlation analysis for practical significance.  

4. **Modelling**  
   - Logistic Regression: odds ratios for attrition drivers.  
   - Random Forest: non-linear interactions and feature importance.  

5. **Clustering**  
   - K-modes with Huang initialisation.  
   - Optimal k = 7 clusters.  
   - t-SNE visualisation for interpretability.  

---

## 🚀 How to Use  

1. **Dataset**: Load `latest_employee_records.xlsx`.  
2. **Preprocessing**: Run data cleaning pipeline (Python script).  
3. **Attrition Analysis**: Execute statistical tests and models (logistic, random forest).  
4. **Clustering**: Run K-modes script to generate 7 clusters.  
5. **Visualisation**: Review charts for attrition trends and cluster profiles.  
6. **Interpret Results**: Refer to the final report (`Workforce Analytics.pdf`) for insights and recommendations.  

---

## 📊 Tools & Technologies  
- **Languages**: Python (Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn).  
- **Statistical Methods**: T-test, Chi-square, Correlation, Logistic Regression, Random Forest.  
- **Clustering**: K-modes, t-SNE.  
- **Visualisation**: Tableau & Matplotlib.  
- **Data Source**: HRIS employee records (2023 snapshot).  


---

## 📌 Future Work  
- Expand analysis to include environmental & external labour market data.  
- Track **involuntary attrition** separately.  
- Deploy interactive dashboards for HR leaders.  
- Extend segmentation to other regions & survey data.  

