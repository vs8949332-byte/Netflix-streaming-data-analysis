
## 📌 Project Overview

This project analyses a **synthetic Netflix-style OTT dataset** to understand **user behaviour, content performance, ratings and revenue**.

The data is spread across **5 related tables** and contains deliberate data-quality issues (such as duplicate viewing records), so the project covers the **complete analytics workflow**: cleaning, merging, exploring, visualising and turning numbers into business recommendations.

> ⚠️ **Note:** This is a **synthetic dataset** created for data science practice. It is **not real Netflix internal data**.

---

## 🎯 Project Objectives

- Clean and validate raw multi-table data (duplicates, missing values, data types)
- Merge users, titles, viewership, ratings and payments into an analysis-ready dataset
- Explore user behaviour and content consumption patterns
- Analyse ratings and their relationship with viewership
- Understand payment and revenue trends
- Answer 6 business questions using groupby and correlation analysis
- Build clean, Netflix-themed visualisations
- Generate actionable business recommendations

---

## 🗂️ Dataset Structure

The dataset contains **5 relational tables**:

| Table | Records | Description |
|---|---|---|
| `users.csv` | 8,000 | User information |
| `titles.csv` | 4,500 | Movies and TV shows catalogue |
| `viewership.csv` | 20,150 | Viewing records (includes deliberate duplicates) |
| `ratings.csv` | 9,000 | User ratings and reviews |
| `payments.csv` | 6,000 | Payment records |

### 🔗 Table Relationships

| From | → | To |
|---|---|---|
| `users.user_id` | → | `viewership.user_id` |
| `users.user_id` | → | `ratings.user_id` |
| `users.user_id` | → | `payments.user_id` |
| `titles.title_id` | → | `viewership.title_id` |
| `titles.title_id` | → | `ratings.title_id` |

---

## 🛠️ Tech Stack

| Tool | Purpose |
|---|---|
| 🐍 **Python** | Core programming language |
| 🐼 **Pandas** | Data cleaning, merging, groupby analysis |
| 🔢 **NumPy** | Numerical operations |
| 📊 **Matplotlib** | Custom charts and Netflix-themed styling |
| 🎨 **Seaborn** | Statistical visualisation and correlation heatmaps |
| 📓 **Jupyter Notebook** | Interactive analysis and documentation |

---

## 🔄 Project Workflow

```
Raw Data  →  Cleaning  →  Merging  →  EDA  →  Business Analysis  →  Visualisation  →  Insights
```

### 1️⃣ Data Cleaning
- Inspected each table (shape, data types, nulls)
- Removed duplicate viewing records
- Handled missing and inconsistent values
- Standardised data types

### 2️⃣ Data Merging
- Joined all tables using `user_id` and `title_id`
- Validated record counts after every merge

### 3️⃣ Exploratory Data Analysis
- Distribution of users, content and ratings
- Viewing patterns and trends
- Correlation analysis between key numeric variables

### 4️⃣ Business Analysis
- Answered 6 business questions using **groupby** and **correlation** analysis

### 5️⃣ Visualisation
- Netflix-themed charts built with Matplotlib and Seaborn

### 6️⃣ Conclusion
- Summary of findings and recommendations

---


## 📊 Key Insights

> 👉 Replace the points below with your real findings from the notebook.

- 🔹 The Standard plan is the biggest revenue contributor, followed by Premium..
- 🔹 India leads in user count, followed by the USA and UK.
- 🔹 Romance and Sports are the most available genres on the platform.
- 🔹 Mobile is the most preferred device for streaming.
- 🔹 Average monthly fee varies by country, suggesting some markets are more valuable to the business than others.
---






## 📁 Repository Structure

```
Netflix-streaming-data-analysis/
│
├── Netflix project.ipynb    # Complete analysis notebook
└── README.md                # Project documentation
```

---

## ▶️ How to Run

```bash
# 1. Clone the repository
git clone https://github.com/vs8949332-byte/Netflix-streaming-data-analysis.git

# 2. Install the required libraries
pip install pandas numpy matplotlib seaborn jupyter

# 3. Launch Jupyter and open the notebook
jupyter notebook
```

---

## 🚀 Skills Demonstrated

`Data Cleaning` • `Data Merging` • `Exploratory Data Analysis` • `Groupby & Aggregation` • `Correlation Analysis` • `Data Visualisation` • `Business Storytelling`

---

## 👤 Author

**Vansh**
Aspiring Data Analyst | Excel • Power BI • SQL • Python

🔗 [GitHub Profile](https://github.com/vs8949332-byte)

---

<p align="center">⭐ If you found this project helpful, consider giving it a star! ⭐</p>
