# 📡 Telecom Customer Churn Analysis

> Exploratory data analysis on 7,000+ telecom subscriber records to identify the behavioral, contractual, and service patterns that drive customer churn — and what the business can do about it.

---

## 📌 Project Overview

Customer churn is one of the most costly problems in the telecom industry. Acquiring a new customer costs **5–7× more** than retaining an existing one. This project digs into subscriber data to answer:

- Which contract types and payment methods are most associated with churn?
- Do value-added services (tech support, online security, device protection) reduce churn?
- How does tenure affect the likelihood of a customer leaving?
- What customer profile is most at risk?

---

## 🛠️ Tools & Technologies

| Tool | Purpose |
|------|---------|
| Python (Pandas) | Data loading, exploration, and manipulation |
| Matplotlib & Seaborn | Churn pattern visualizations |
| Jupyter Notebook | Development and narrative environment |

---

## 📂 Dataset

- **Source:** IBM Telco Customer Churn Dataset (via Kaggle)
- **Records:** 7,043 customers
- **Features:** 21 columns including demographics, account info, subscribed services, and churn label
- **Target Variable:** `Churn` (Yes / No)

### Key Features Analyzed

| Feature | Type | Description |
|---------|------|-------------|
| Contract | Categorical | Month-to-month, One year, Two year |
| PaymentMethod | Categorical | Electronic check, Mailed check, Bank transfer, Credit card |
| InternetService | Categorical | DSL, Fiber optic, None |
| TechSupport | Binary | Whether customer has tech support |
| OnlineSecurity | Binary | Whether customer has online security add-on |
| OnlineBackup | Binary | Whether customer has online backup |
| DeviceProtection | Binary | Whether customer has device protection |
| tenure | Numeric | Months the customer has been with the company |
| Dependents | Binary | Whether customer has dependents |
| Partner | Binary | Whether customer has a partner |

---

## 🔍 Key Findings

### 📋 Contract Type — Strongest Churn Predictor
Month-to-month subscribers churn at dramatically higher rates than annual or two-year contract holders. Longer commitments create switching friction and signal customer satisfaction.

> **Implication:** Incentivize contract upgrades through loyalty discounts or bundled perks.

### 💳 Payment Method Matters
Electronic check users show the highest churn rate. Customers on automatic payment methods (bank transfer, credit card auto-pay) are significantly less likely to churn.

> **Implication:** Nudge customers toward auto-pay enrollment — it reduces churn AND reduces billing friction.

### 🌐 Fiber Optic = High Churn Risk
Surprisingly, fiber optic internet subscribers churn more than DSL customers. This may signal unmet expectations around price-to-performance ratio.

> **Implication:** Review pricing, speed guarantees, and service quality perception among fiber users.

### 🛡️ Value-Added Services Retain Customers
Customers **without** tech support, online security, online backup, or device protection show consistently higher churn rates — often double those with these add-ons.

> **Implication:** Bundle these services into onboarding packages to improve retention from day one.

### ⏱️ Tenure is Critical — The First Month is the Danger Zone
Churn is highest in the first month of subscription and declines sharply with tenure. Long-term customers almost never leave.

> **Implication:** Invest heavily in the first 90-day customer experience. Early churn prevention has the highest ROI.

### 👨‍👩‍👧 Dependents Anchor Customers
Customers with dependents are far less likely to churn. Customers without partners show elevated churn risk.

> **Implication:** Family plans and multi-line bundling can significantly improve retention.

---

## 📊 Visualizations

The notebook includes **11 countplot visualizations** covering churn distribution across:

- Contract type
- Payment method
- Internet service type
- Partner status
- Dependents
- Phone service
- Tech support
- Online security
- Online backup
- Device protection
- Customer tenure

---

## 💡 Business Recommendations

| Priority | Recommendation | Target Segment |
|---------|---------------|----------------|
| 🔴 High | Launch early-tenure retention program (first 90 days) | Month-to-month, new subscribers |
| 🔴 High | Incentivize auto-payment enrollment | Electronic check users |
| 🟡 Medium | Bundle tech support + security in onboarding | Customers without value-add services |
| 🟡 Medium | Audit fiber optic pricing and service quality | Fiber optic subscribers |
| 🟢 Low | Promote family/multi-line plans | Single subscribers without partners |

---

## 📁 Project Structure

```
telecom-churn-analysis/
│
├── data/
│   └── Telco-Customer-Churn.csv       # Source dataset
│
├── notebooks/
│   └── TelecomChurn.ipynb             # Main analysis notebook
│
├── visuals/                           # Exported churn charts
│
└── README.md
```

---

## 🚀 How to Run

```bash
# Clone the repository
git clone https://github.com/ShradhaPai/telecom-churn-analysis.git
cd telecom-churn-analysis

# Install dependencies
pip install pandas matplotlib seaborn jupyter

# Launch the notebook
jupyter notebook notebooks/TelecomChurn.ipynb
```

---

## 🔮 Future Scope

- [ ] Build a churn prediction model (Logistic Regression, Random Forest, XGBoost)
- [ ] Calculate feature importance scores for each churn driver
- [ ] Add customer lifetime value (CLV) estimation
- [ ] Create an interactive dashboard in Tableau or Power BI

---

## 👩‍💻 Author

**Shradha R Pai** — Data Analyst  
[LinkedIn](https://www.linkedin.com/in/shradha-pai/) • [GitHub](https://github.com/ShradhaPai)
