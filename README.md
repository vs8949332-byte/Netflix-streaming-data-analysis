This project analyses a synthetic Netflix-style dataset created for data science practice. It is not real Netflix internal data.

The goal is to clean messy multi-table data, explore user behaviour, and answer real business questions about viewership, ratings and revenue.

🗂️ Dataset
Table	Records	Description
users.csv:	8,000	User profiles
titles.csv:	4,500	Movies and TV shows
viewership.csv:	20,150	Viewing records (includes deliberate duplicates)
ratings.csv:	9,000	Ratings and reviews
payments.csv:	6,000	Payment records



🔗 Table Relationships
users.user_id   ──► viewership.user_id
users.user_id   ──► ratings.user_id
users.user_id   ──► payments.user_id
titles.title_id ──► viewership.title_id
titles.title_id ──► ratings.title_id


🛠️ Tools & Libraries
Python
Pandas, NumPy – data cleaning and manipulation
Matplotlib, Seaborn – visualisation
Jupyter Notebook – analysis environment



🔄 Project Workflow
Data Cleaning:  removed duplicates, handled missing values, fixed data types
Data Merging:  joined the 5 tables using the keys above
Exploratory Data Analysis:  distributions, trends, correlations
Business Analysis:  answered 6 business questions using groupby and correlation analysis
Visualisation:  Netflix-themed charts
Conclusion:  key insights and recommendations


📊 Key Insights:
- The Standard plan is the biggest revenue contributor, followed by Premium.
- India leads in user count, followed by the USA and UK.
- Around 84% of users are active, showing healthy retention.
- Romance and Sports are the most available genres on the platform.


🔹 Most-watched genre / content type: ...
🔹 Subscription plan generating the highest revenue: ...
🔹 Relationship between ratings and viewing time: ...
📁 Repository Structure
Netflix-streaming-data-analysis/
│
├── Netflix project.ipynb   # Main analysis notebook
└── README.md               # Project documentation
▶️ How to Run
bash
# 1. Clone the repository
git clone https://github.com/vs8949332-byte/Netflix-streaming-data-analysis.git

# 2. Install dependencies
pip install pandas numpy matplotlib seaborn jupyter

# 3. Open the notebook
jupyter notebook


👤 Author

Vansh Aspiring Data Analyst | Excel • Power BI • SQL • Python

🔗 GitHub

⭐ If you found this project useful, consider giving it a star!
