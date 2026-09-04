# 🏏 IPL Data Analysis — PostgreSQL, Python & Power BI

> **End-to-end IPL Data Analytics project using PostgreSQL, Python, and Power BI to analyze match and ball-by-ball data, uncover performance trends, and build an interactive business intelligence dashboard.**

![PostgreSQL](https://img.shields.io/badge/PostgreSQL-Database-4169E1?logo=postgresql\&logoColor=white)
![Python](https://img.shields.io/badge/Python-Data%20Analysis-3776AB?logo=python\&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-150458?logo=pandas\&logoColor=white)
![Power BI](https://img.shields.io/badge/Power%20BI-Dashboard-F2C811?logo=powerbi\&logoColor=black)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-F37626?logo=jupyter\&logoColor=white)

---

## 📌 Project Overview

The **IPL Data Analysis** project is an end-to-end data analytics project that uses IPL match-level and ball-by-ball delivery data.

The project follows a complete analytics workflow:

**CSV Data → PostgreSQL → Python → Power BI → Business Insights**

PostgreSQL is used as the **central database** for storing and querying the IPL datasets. Python is used for exploratory data analysis and deeper statistical analysis, while Power BI is used to create an interactive dashboard for data visualization and business insights.

---

# 🎯 Project Objectives

The main objectives of this project are to:

* Analyze IPL match and delivery data
* Store and manage structured IPL data using PostgreSQL
* Perform SQL-based data exploration and analysis
* Clean and transform data using Python
* Perform Exploratory Data Analysis (EDA)
* Analyze team and player performance
* Identify important match and toss trends
* Build an interactive Power BI dashboard
* Convert raw sports data into meaningful insights

---

# 🏗️ End-to-End Data Analytics Workflow

```text
                 IPL Raw CSV Data
                       │
                       ▼
              ┌─────────────────┐
              │   PostgreSQL    │
              │    Database     │
              └────────┬────────┘
                       │
                SQL Queries
                       │
                       ▼
              ┌─────────────────┐
              │     Python      │
              │ Pandas / NumPy  │
              │      EDA        │
              └────────┬────────┘
                       │
                Data Analysis
                       │
                       ▼
              ┌─────────────────┐
              │    Power BI     │
              │   Data Model    │
              │ DAX + Dashboard │
              └────────┬────────┘
                       │
                       ▼
              Business Insights
```

---

# 🛠️ Tech Stack

| Technology              | Purpose                                  |
| ----------------------- | ---------------------------------------- |
| 🐘 **PostgreSQL**       | Data storage, SQL querying & analysis    |
| 🐍 **Python**           | Data cleaning, transformation & analysis |
| 🐼 **Pandas**           | Data manipulation                        |
| 🔢 **NumPy**            | Numerical analysis                       |
| 📓 **Jupyter Notebook** | Exploratory Data Analysis                |
| 📊 **Power BI**         | Dashboard & data visualization           |
| 📁 **CSV**              | Raw source data                          |

---

# 🐘 PostgreSQL Database

PostgreSQL is used to store and analyze the IPL datasets before visualization.

### Database Tables

The project primarily works with:

### `matches`

Contains match-level information including:

* Match ID
* Season
* Date
* Teams
* Venue
* Toss winner
* Toss decision
* Match winner
* Player of the Match
* Match result

### `deliveries`

Contains ball-by-ball information including:

* Match ID
* Inning
* Batting team
* Bowling team
* Batter
* Bowler
* Runs scored
* Extra runs
* Total runs
* Wickets
* Dismissal information

---

## 🔎 SQL Analysis

PostgreSQL is used to answer analytical questions using SQL.

Examples of analysis include:

* Total matches played
* Matches won by each team
* Team win percentage
* Top run scorers
* Top wicket takers
* Most Player of the Match awards
* Toss winner vs match winner
* Batting first vs chasing performance
* Venue-wise match statistics
* Season-wise team performance
* Player performance analysis

Example SQL analysis:

```sql
SELECT 
    winner,
    COUNT(*) AS matches_won
FROM matches
WHERE winner IS NOT NULL
GROUP BY winner
ORDER BY matches_won DESC;
```

---

# 🐍 Python Data Analysis

Python is used after database-level analysis for deeper exploratory analysis and visualization.

### Libraries

```text
Pandas
NumPy
Matplotlib
Seaborn
Jupyter Notebook
```

### Analysis Areas

#### 🏆 Team Analysis

* Matches played
* Matches won
* Win percentage
* Season-wise performance
* Team comparison

#### 🏏 Batting Analysis

* Total runs
* Top run scorers
* Batting averages
* Strike rates
* Boundary analysis

#### 🎯 Bowling Analysis

* Total wickets
* Leading wicket takers
* Bowling performance
* Economy analysis

#### 🪙 Toss Analysis

* Toss winner vs match winner
* Batting first vs chasing
* Toss decision trends

#### 🏟️ Venue Analysis

* Matches hosted
* Team performance by venue
* Venue-wise winning patterns

---

# 📊 Power BI Dashboard

The analyzed IPL data is visualized through an interactive Power BI dashboard.

### Dashboard Features

* 📌 KPI cards
* 🏆 Team performance analysis
* 🏏 Top batsmen
* 🎯 Top bowlers
* 🪙 Toss analysis
* 🏟️ Venue analysis
* 📅 Season-wise analysis
* 🔎 Interactive slicers
* 📈 Performance comparisons

### Data Flow into Power BI

```text
PostgreSQL
     │
     ▼
Power BI
     │
     ├── Data Model
     ├── Relationships
     ├── DAX Measures
     ├── KPIs
     └── Visualizations
             │
             ▼
      Interactive Dashboard
```

### Dashboard Preview

Add your dashboard screenshot inside the repository:

```markdown
![IPL Power BI Dashboard](images/ipl-dashboard.png)
```

---

# 💡 Key Business Questions

The project answers questions such as:

1. Which IPL teams have the highest number of wins?
2. Which teams have the best win percentage?
3. Who are the top run scorers?
4. Who are the leading wicket takers?
5. Which players have received the most Player of the Match awards?
6. Does winning the toss increase the probability of winning the match?
7. Is chasing more successful than batting first?
8. Which venues have hosted the most IPL matches?
9. How does team performance change across seasons?
10. Which players and teams consistently perform well?

---

# 📈 Key Insights

The analysis focuses on identifying:

* Team dominance and consistency
* Player performance trends
* Batting and bowling patterns
* Toss impact on match results
* Chasing vs defending performance
* Venue-specific trends
* Season-wise performance changes

> **Note:** Add your actual numerical findings here after completing the final SQL/Python/Power BI analysis.

---

# 📂 Project Structure

```text
IPL-Data-Analysis/
│
├── 📓 IPL_Analysis.ipynb
│
├── 📊 matches.csv
├── 🏏 deliveries.csv
│
├── 🐘 sql/
│   ├── create_tables.sql
│   ├── data_analysis.sql
│   └── player_analysis.sql
│
├── 📈 IPL DASHBOARD ANALAYSIS.pbix
│
├── 📄 requirements.txt
├── 📄 README.md
│
└── 📁 images/
    └── ipl-dashboard.png
```

---

# ⚙️ Installation & Setup

## 1️⃣ Clone the Repository

```bash
git clone https://github.com/YOUR_USERNAME/YOUR_REPOSITORY.git
```

```powershell
cd IPL-Data-Analysis
```

---

## 2️⃣ PostgreSQL Setup

Install **PostgreSQL** and create a database:

```sql
CREATE DATABASE ipl_analysis;
```

Connect to the database and create the required tables using the SQL scripts provided in the `sql/` directory.

Example:

```sql
CREATE TABLE matches (
    id INT PRIMARY KEY,
    season INT,
    date DATE,
    team1 VARCHAR(100),
    team2 VARCHAR(100),
    toss_winner VARCHAR(100),
    toss_decision VARCHAR(50),
    winner VARCHAR(100)
);
```

Load the IPL CSV data into the appropriate PostgreSQL tables.

> **Important:** Update the database connection details locally. Do not commit passwords or credentials to GitHub.

---

# 🐍 Python Environment Setup

Create a virtual environment:

```powershell
python -m venv .venv
```

Activate it:

```powershell
.\.venv\Scripts\Activate.ps1
```

Install dependencies:

```powershell
python -m pip install -r requirements.txt
```

---

# 📓 Run Python Analysis

Open:

```text
IPL_Analysis.ipynb
```

using **Jupyter Notebook** or **VS Code**.

Run the notebook cells sequentially.

If Python connects directly to PostgreSQL, configure the connection locally using environment variables rather than hardcoding credentials.

Example:

```python
import pandas as pd
from sqlalchemy import create_engine

engine = create_engine(
    "postgresql://username:password@localhost:5432/ipl_analysis"
)

df = pd.read_sql("SELECT * FROM matches", engine)
```

---

# 📊 Open Power BI Dashboard

Open:

```text
IPL DASHBOARD ANALAYSIS.pbix
```

If the dashboard uses PostgreSQL as its data source:

1. Open the `.pbix` file.
2. Verify the PostgreSQL connection.
3. Update the local database/server details if required.
4. Refresh the dataset.
5. Explore the interactive dashboard.

---

# 🔐 Security

Never upload database credentials to GitHub.

❌ Do not commit:

```text
username
password
API keys
connection strings containing passwords
.env files
```

Use environment variables or a `.env` file locally and add it to `.gitignore`.

Example:

```text
.env
.venv/
__pycache__/
*.pyc
```

---

# 📊 Skills Demonstrated

## PostgreSQL

* Database creation
* Table creation
* Data loading
* SQL querying
* Filtering
* Aggregation
* GROUP BY
* JOIN operations
* Subqueries
* Analytical queries

## Python

* Pandas
* NumPy
* Data cleaning
* Data transformation
* Exploratory Data Analysis
* Data visualization

## Power BI

* Data connection
* Data modeling
* Relationships
* DAX measures
* KPI development
* Interactive visualizations
* Dashboard design
* Data storytelling

---

# 🔄 Complete Project Pipeline

```text
       Raw IPL CSV Files
              │
              ▼
       ┌───────────────┐
       │  PostgreSQL   │
       │   Database    │
       └───────┬───────┘
               │
          SQL Analysis
               │
               ▼
       ┌───────────────┐
       │    Python     │
       │     EDA       │
       └───────┬───────┘
               │
        Data Validation
               │
               ▼
       ┌───────────────┐
       │   Power BI    │
       │     DAX       │
       │   Dashboard   │
       └───────┬───────┘
               │
               ▼
       Business Insights
```

---

# 🚀 Future Improvements

* [ ] Add advanced SQL analytics
* [ ] Build a complete star schema
* [ ] Add advanced DAX measures
* [ ] Add player comparison dashboard
* [ ] Add season-by-season analysis
* [ ] Add advanced batting metrics
* [ ] Add advanced bowling metrics
* [ ] Add match win probability
* [ ] Add predictive analysis
* [ ] Automate data refresh
* [ ] Deploy Power BI report
* [ ] Connect Power BI directly to PostgreSQL

---

# 🎓 What This Project Demonstrates

This project demonstrates an end-to-end **Data Analyst workflow**:

> **Data Collection → Database Management → SQL Analysis → Python EDA → Data Modeling → Power BI → Business Insights**

It showcases practical experience with three important tools used in modern data analytics:

**PostgreSQL + Python + Power BI**

---

# 👨‍💻 Author

**Sherif**

Aspiring Data Analyst

**Skills:**
`PostgreSQL` • `SQL` • `Python` • `Pandas` • `Power BI` • `DAX` • `Data Visualization` • `Exploratory Data Analysis`

---

## ⭐ Support

If you found this project useful or interesting, consider giving the repository a **⭐ Star**.

Feedback and suggestions are welcome!
