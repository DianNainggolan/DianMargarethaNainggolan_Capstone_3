# Customer Churn Prediction for Telkom Indonesia

This project focuses on predicting **customer churn** at Telkom Indonesia using machine learning, enabling more efficient and targeted retention strategies. Telkom, as a major telecommunications company, relies heavily on subscription-based revenue models. Reducing churn means maintaining revenue stability and lowering customer acquisition costs.

---

## 🧠 Business Understanding

Telkom Indonesia provides broadband, telephony, IPTV, and digital solutions to residential and business customers across Indonesia. Its business model depends on:

* **Long-term customer retention**, especially for broadband and bundled services.
* **Early churn detection** to minimize revenue loss.
* **Targeted campaigns** to reduce marketing costs.

Churn prediction models help Telkom identify **which customers are at high risk of leaving**, so marketing and service teams can act proactively.

---

## 📊 Data Understanding

The dataset represents Telkom customer records with variables such as:

* **CustomerID** — unique customer identifier
* **Tenure** — duration of customer’s subscription
* **Contract Type** — monthly, yearly, or two-year contract
* **InternetService** — DSL, Fiber, or None
* **MonthlyCharges** — monthly bill amount
* **Other service variables** — additional products like security, backup, support

These features are crucial to understanding customer behavior and identifying churn signals.

---

## 🧪 Preprocessing & Feature Engineering

1. **Standard Scaling** for numerical features to stabilize model performance.
2. **One-Hot Encoding** for categorical variables (contract type, internet service, add-on services).
3. **Handling Imbalance** with SMOTEENN (Synthetic Minority Oversampling + Edited Nearest Neighbors) to improve recall on churn cases.
4. **Feature Importance** was evaluated with permutation and SHAP values, revealing key churn drivers:

   * **Tenure** (short contract durations correlate with higher churn)
   * **MonthlyCharges** (higher bills increase churn risk)
   * **Contract Type** (monthly contracts have the highest churn)
   * **InternetService** (fiber optic users have higher churn risk if service quality drops).

---

## 🧠 Modeling Approach

Multiple classification algorithms were tested, including Logistic Regression, KNN, LightGBM, and QDA.

* **Best Model:** Quadratic Discriminant Analysis (QDA) with SMOTEENN
* **Recall:** 0.85
* **ROC AUC:** > 0.84
* **Precision:** 0.49

This combination offered the best balance between catching churners and minimizing false positives.

---

## 📈 Business Impact Simulation

* **Total customers:** 10,000
* **Historical churn:** 25% (2,500 customers)
* **Campaign cost per customer:** $20

| Scenario            | Customers Contacted | Churn Detected | Total Cost | Cost Saved |
| ------------------- | ------------------- | -------------- | ---------- | ---------- |
| Without Model       | 10,000              | 2,500          | $200,000   | $0         |
| With QDA + SMOTEENN | 4,300               | 2,125          | $86,000    | $114,000   |

Using the model, Telkom can **cut campaign costs by more than 50%** while still detecting 85% of churn cases.

---

## 📊 Key Insights

* **Tenure under 12 months** and **monthly contracts** show the highest churn risk.
* **High monthly charges** increase churn probability.
* Customers without bundled services or support features are more likely to leave.
* Fiber optic users represent a large and sensitive segment.

---

## 🧭 Recommendations

* **Contract & Loyalty:** Incentivize customers with monthly contracts to switch to yearly contracts.
* **Product Bundling:** Promote additional services like security and tech support to increase stickiness.
* **Targeted Retention:** Focus early intervention on short-tenure, high-cost customers.
* **Price & Value Alignment:** Offer upgrade packages or discounts to reduce dissatisfaction.
* **Service Quality:** Improve fiber optic reliability and proactive support.

---

## 🧠 Why This Matters for Telkom

By combining predictive analytics with business strategy, Telkom Indonesia can:

* Lower churn rate significantly.
* Reduce unnecessary marketing spend.
* Personalize retention programs for maximum impact.
* Strengthen long-term customer loyalty in a competitive telco market.

