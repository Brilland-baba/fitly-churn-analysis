 # 🏋️ Fit.ly Churn Analysis | DataCamp Data Analyst Certification

[![Python](https://img.shields.io/badge/Python-3.8%2B-blue.svg)](https://python.org)
[![Pandas](https://img.shields.io/badge/Pandas-2.0%2B-green.svg)](https://pandas.pydata.org)
[![DataCamp](https://img.shields.io/badge/DataCamp-Certified-orange.svg)](https://datacamp.com)
[![License](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)

## 📌 Project Overview

This project analyzes customer churn for **Fit.ly Tech**, a subscription-based fitness app experiencing increasing churn rates. The goal is to identify drivers of churn and provide actionable recommendations.

### 🎯 Business Problem
> *"Over the past two quarters, leadership has noticed churn creeping up in our subscriber base. Retaining customers is critical as our cost of acquiring new users is rising."*

---

## 📊 Key Performance Indicators (KPIs)

| Metric | Value |
|--------|-------|
| **Overall Churn Rate** | 28.5% |
| **Total Customers** | 400 |
| **Churned Customers** | 114 |
| **Active Customers** | 286 |

---

## 📈 Churn Rate by Plan

| Plan | Customers | Churn Rate |
|------|-----------|-------------|
| Free | 105 | 🔴 **41.0%** |
| Enterprise | 92 | 🟡 26.1% |
| Basic | 118 | 🟢 23.7% |
| Pro | 85 | 🟢 22.4% |

---

## 🔍 Key Findings

### 1. Plan Type Drives Churn
- **Free plan users churn at 41.0%** - nearly double the rate of paid users
- Pro and Basic plans show the highest loyalty

### 2. Support Tickets = Risk Signal
- Customers with 0-2 tickets: **26.7% churn**
- Customers with 3+ tickets: **31.1% churn** (+4.4 percentage points)

### 3. Engagement is the Strongest Predictor
| Engagement Level | Churn Rate |
|-----------------|-------------|
| 0 events | 🔴 **53.9%** |
| 1-5 events | 🟡 12.6% |
| 6+ events | 🟢 **0%** |

> **Critical Insight:** Users who complete 6+ events NEVER churn in this dataset!

---

## 💡 Recommendations

### Immediate Actions (Next 30 Days)

| Action | Target | Expected Impact |
|--------|--------|-----------------|
| 🎯 "6 Events Challenge" | New users | Reduce early churn 53.9% → <15% |
| 📞 Proactive Support Outreach | 2+ tickets customers | Lower churn 31.1% → <25% |
| 🎁 Free Plan Retention Campaign | Free tier users | Reduce Free churn 41.0% → <30% |

### Medium-term Strategy (Next Quarter)

4. **Redesign Free Plan** - Add engagement hooks (streaks, achievements, social features)
5. **Implement Churn Prediction Model** - Flag high-risk users based on ticket count and event frequency
6. **Launch Customer Loyalty Program** - Reward 12+ month subscribers

---

## 🎯 Target KPIs

| Metric | Current | Target | Status |
|--------|---------|--------|--------|
| Monthly Churn Rate | 28.5% | <20% | 🔴 Critical |
| Free Plan Churn | 41.0% | <30% | 🔴 Critical |
| Users with 6+ events | N/A | +25% | 🟡 To monitor |
| Support Resolution Time | N/A | <24h | 🟡 To monitor |

---

## 📁 Data Sources

| File | Rows | Columns | Description |
|------|------|---------|-------------|
| `da_fitly_account_info.csv` | 400 | 6 | Customer accounts (plan, price, churn) |
| `da_fitly_customer_support.csv` | 918 | 7 | Support tickets (channel, topic, resolution) |
| `da_fitly_user_activity.csv` | 445 | 3 | User activity logs (event type, timestamp) |




## 🛠️ Technical Stack
┌─────────────────────────────────────────────────┐
│ 🐍 Python 3.8+ │
│ ├── pandas (data manipulation) │
│ ├── numpy (numerical operations) │
│ ├── matplotlib (visualizations) │
│ └── seaborn (statistical graphics) │
├─────────────────────────────────────────────────┤
│ 📓 Jupyter Notebook │
│ 📊 PowerPoint (presentation) │
└─────────────────────────────────────────────────┘




## 📂 Project Structure
fitly-churn-analysis/
│
├── README.md # Documentation
├── requirements.txt # Python dependencies
├── notebook.ipynb # Main analysis notebook
│
├── 📊 Data Files/
│ ├── da_fitly_account_info.csv
│ ├── da_fitly_customer_support.csv
│ └── da_fitly_user_activity.csv
│
├── 📈 Visualizations/
│ ├── Customers_plan.png
│ ├── customers_tickets.png
│ ├── hurn Rate_By_Plan_Type.png
│ ├── plots_suppot_tickets.png
│ └── engagement_.png
│
└── 📑 Presentation/
└── Fitly_Retention_Strategy.pptx





---

## 🚀 Quick Start

### Prerequisites
```bash
# Clone the repository
git clone https://github.com/Brilland-baba/fitly-churn-analysis.git
cd fitly-churn-analysis

# Install dependencies
pip install -r requirements.txt






# Launch Jupyter Notebook
jupyter notebook notebook.ipynb