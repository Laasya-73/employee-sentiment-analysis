# 📘 Employee Sentiment Analysis – Project Summary

This project focuses on analyzing internal employee messages to understand sentiment trends, rank employees by positivity, identify those who may be disengaged, and build a predictive model to anticipate sentiment scores.

I worked on this end-to-end — from labeling sentiment in raw email texts to analyzing trends, ranking behavior, detecting flight risks, and finally building a model to forecast future sentiment. Everything was implemented using Python, with pandas, seaborn, scikit-learn, and TextBlob for analysis and modeling.

---

## ✅ Top 3 Positive and Negative Employees (January 2010)

After scoring each employee's monthly sentiment using a +1/0/–1 system, I ranked them based on total sentiment scores per month. Here's a quick look at the first month of data to give an idea:

- **Top 3 Positive Employees:**
  - Kayne Coulter (Score: 9)
  - Don Baughman (Score: 5)
  - Eric Bass (Score: 5)

- **Top 3 Negative Employees:**
  - Rhonda Denton (Score: 0)
  - Bobette Riner (Score: 2)
  - Johnny Palmer (Score: 2)

This ranking logic was applied across every month in the dataset, helping identify consistent patterns in employee tone and communication.

---

## ⚠️ Employees Flagged as Flight Risks

Using a rolling 30-day window, I flagged employees who sent **4 or more negative emails** in that span. These employees showed short-term bursts of negativity, which could be early signs of disengagement or dissatisfaction.

**Flagged Flight Risks:**
- bobette.riner  
- don.baughman  
- eric.bass  
- john.arnold  
- johnny.palmer  
- kayne.coulter  
- lydia.delgado  
- patti.thompson  
- rhonda.denton  
- sally.beck

This wasn’t based on judgment — just data-driven criteria. It highlights employees HR might want to check in with proactively.

---

## 🔍 Key Insights & Recommendations

### 📊 Insights:
- **Positive sentiment dominated**, but there were still over 250 negative emails — which shouldn't be ignored.
- Employees with **high message volume** also had a larger impact on sentiment trends.
- Some employees were both highly active and highly negative in specific time windows, which stood out more clearly once scoring and risk analysis were applied.

### 💡 Recommendations:
- Use monthly sentiment scoring as part of performance and wellness dashboards.
- Track changes in employee rankings over time — sudden drops could indicate issues worth exploring.
- Don’t rely solely on message count. Sentiment tone provides deeper insights.
- Use flight risk logic regularly to monitor short-term shifts in employee morale.

---

## 📂 Project Files

- `labeled_test.csv` – Sentiment-labeled email data
- `employee_monthly_sentiment_scores.csv` – Monthly sentiment scores
- `top_3_positive_employees_by_month.csv`
- `top_3_negative_employees_by_month.csv`
- `flight_risk_employees.csv`
- `visualization/` – Charts for distribution, trends, rankings, and regression
- `README.md` – You’re reading it!

---

📌 Project by: **Laasya Priya Vemuri**



```python

```
