# Explainable AI Credit Scoring POC

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1OT7B57bneJuPouTW1KzFPT_wMDcew-QH?usp=sharing)

**Demo:**  
[![Watch the Demo](https://i.imgur.com/J2WWxwF.gif)](https://www.youtube.com/watch?v=nZNtefjyC_M)  
*Click the animation to view the full YouTube walkthrough.*

---

## 📌 Project Overview
Build and compare **glass-box** (EBM) and **black-box** (RF, XGB, LGBM) credit-scoring models on a 32 581-loan dataset.  
– Measure accuracy, F₁ & F₂ metrics.  
– Apply native (EBM) and post-hoc (SHAP, Anchors, DICE) explainability.  
– Deliver three role-based UIs:  
  - **Data Scientist / Regulator View**  
  - **Loan Officer View**  
  - **Client View**  

---

## 🔑 Key Features
**Dataset:** [Kaggle Credit Risk](https://www.kaggle.com/datasets/laotse/credit-risk-dataset)  

| Feature                       | Description                                 |
|-------------------------------|---------------------------------------------|
| `person_age`                  | Applicant’s age                             |
| `person_income`               | Annual income                               |
| `person_home_ownership`       | RENT / MORTGAGE / OWN / OTHER                |
| `person_emp_length`           | Employment length (years)                   |
| `loan_intent`                 | Purpose (EDUCATION, MEDICAL, etc.)          |
| `loan_grade`                  | Credit grade (A–G)                          |
| `loan_amnt`                   | Requested amount                            |
| `loan_int_rate`               | Interest rate                               |
| `loan_status`                 | Target (0 = non-default, 1 = default)        |
| `loan_percent_income`         | Loan-to-income ratio                        |
| `cb_person_default_on_file`   | Prior defaults (Y/N)                        |
| `cb_person_cred_hist_length`  | Credit history length (years)               |

---

## 📓 Notebook Summary
1. **Load & Explore**: inspect missingness, distributions, correlations  
2. **Clean & Preprocess**: impute, cap outliers, one-hot encode, scale  
3. **Baseline Models**: Logistic, RF, XGBoost, LightGBM  
4. **Explainability**:  
   - **Glass-Box**: EBM global & local explanations  
   - **Post-Hoc**: SHAP summaries, surrogate & GIRP trees, PDP  
5. **Role-Based App**: interactive dashboards for each user type  
6. **Business Impact**: ROI projection on a €1 B portfolio  

_Link to notebook:_  
https://colab.research.google.com/drive/1OT7B57bneJuPouTW1KzFPT_wMDcew-QH?usp=sharing

---

## 💻 Explain Credit Platform
An external web app showcasing three separate, color-coded views:

- **Data Scientist / Regulator**  
  Global feature importance, bias checker, surrogate & GIRP rule exports.  

- **Loan Officer**  
  PDP sliders, “what-if” simulations, similar-case prototype comparisons.  

- **Client**  
  Anchor-style “IF…THEN…” rules, waterfall charts, actionable improvement tips.  

▶️ Demo: https://www.youtube.com/watch?v=nZNtefjyC_M

---

## 📚 References

- Shahee, A. & Patel, R. (2025). *An explainable ADASYN-based focal loss approach for credit assessment.* Journal of Forecasting.  
- Demajo, L. M., Vella, V., & Dingli, A. (2020). *Explainable AI for interpretable credit scoring.* CS & IT Conf.  
- Dessain, J., Bentaleb, N., & Vinas, F. (2023). *Cost of explainability in AI: credit scoring models.* xAI 2023, CCIS 1901.  
- Esna-Ashari, M. (2025). *Beyond the black box: quantitative metrics for NN interpretability.* IJISASE.  
- Garcin, M. & Stéphan, S. (2025). *Credit scoring using neural nets and SURE calibration.* arXiv.  
- Guégan, D. & Hassani, B. (2018). *Regulatory learning: supervising ML in credit scoring.* J. Finance & Data Science.  
- Idbenjra, K., Coussement, K., & De Caigny, A. (2024). *Segmentation-based modelling for credit scoring.* DSS.  
- Talaat, F. M. et al. (2023). *Interpretable credit scoring: XAI with deep learning.* Neural Computing & Applications.  
