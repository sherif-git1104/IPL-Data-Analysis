# 🏏 IPL Data Analysis — Python & Power BI

> **End-to-end IPL data analytics project using Python and Power BI to uncover team performance, player statistics, match trends, and key insights from IPL match and ball-by-ball data.**

![IPL](https://img.shields.io/badge/Domain-Indian%20Premier%20League-blue)
![Python](https://img.shields.io/badge/Python-Data%20Analysis-yellow?logo=python)
![Pandas](https://img.shields.io/badge/Pandas-Analysis-150458?logo=pandas)
![Power BI](https://img.shields.io/badge/Power%20BI-Dashboard-F2C811?logo=powerbi)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange?logo=jupyter)

---

## 📌 Project Overview

The **IPL Data Analysis** project analyzes Indian Premier League match-level and ball-by-ball delivery data to identify meaningful patterns in:

* 🏆 Team performance
* 👤 Player performance
* 🏏 Batting statistics
* 🎯 Bowling statistics
* 📊 Match outcomes
* 🥇 Player of the Match trends
* 🏟️ Venue performance
* 📅 Season-wise trends
* ⚡ Toss decisions and their impact
* 📈 Team win/loss patterns

The project combines **Python for data cleaning, exploration, and statistical analysis** with **Power BI for interactive visualization and dashboard development**.

---

## 🎯 Business Questions

This analysis aims to answer questions such as:

1. Which teams have performed best across IPL seasons?
2. Which players consistently deliver strong performances?
3. Who are the top run scorers?
4. Who are the leading wicket takers?
5. Which venues host the most matches?
6. Does winning the toss increase the probability of winning the match?
7. Which teams perform better while chasing or defending?
8. Which players have received the most Player of the Match awards?
9. How has team performance changed across seasons?
10. What factors appear to influence IPL match outcomes?

---

# 🛠️ Tech Stack

| Technology          | Purpose                       |
| ------------------- | ----------------------------- |
| 🐍 Python           | Data analysis & preprocessing |
| 🐼 Pandas           | Data manipulation             |
| 🔢 NumPy            | Numerical analysis            |
| 📓 Jupyter Notebook | Exploratory Data Analysis     |
| 📊 Power BI         | Interactive dashboard         |
| 📁 CSV              | Dataset storage               |

---

# 📂 Dataset

The project uses two primary datasets.

### `matches.csv`

Contains match-level information such as:

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

### `deliveries.csv`

Contains ball-by-ball information such as:

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

Using both datasets allows analysis at both **match level** and **delivery level**.

---

# 🔄 Project Workflow

```text
             IPL Raw Data
                  │
                  ▼
        ┌───────────────────┐
        │   Data Loading    │
        │     & Cleaning    │
        └─────────┬─────────┘
                  │
                  ▼
        ┌───────────────────┐
        │ Exploratory Data  │
        │      Analysis     │
        │      (Python)     │
        └─────────┬─────────┘
                  │
                  ▼
        ┌───────────────────┐
        │ Statistical &     │
        │ Performance       │
        │ Analysis          │
        └─────────┬─────────┘
                  │
          ┌───────┴────────┐
          ▼                ▼
      Python EDA        Power BI
          │                │
          │                ▼
          │        Interactive Dashboard
          │                │
          └───────┬────────┘
                  ▼
            Key Insights
```

---

# 📊 Python Analysis

The Jupyter Notebook performs exploratory data analysis using Python.

### Key analysis areas

#### 🏆 Team Analysis

* Matches played
* Matches won
* Win percentage
* Season-wise performance
* Team comparison

#### 🏏 Batting Analysis

* Total runs
* Top run scorers
* Average runs
* Strike rate
* Boundary analysis

#### 🎯 Bowling Analysis

* Total wickets
* Leading wicket takers
* Bowling performance
* Economy-related analysis

#### 🪙 Toss Analysis

* Toss winner vs match winner
* Batting first vs chasing
* Toss decision patterns

#### 🏟️ Venue Analysis

* Matches hosted
* Team performance by venue
* Venue-wise winning patterns

---

# 📈 Power BI Dashboard

The Power BI dashboard transforms the analyzed IPL data into an interactive visual analytics experience.

### Dashboard Highlights

* 📌 KPI cards for major performance metrics
* 🏆 Team performance comparison
* 🏏 Top batsmen
* 🎯 Top bowlers
* 🪙 Toss analysis
* 🏟️ Venue analysis
* 📅 Season-wise performance
* 🔎 Interactive filters and slicers

### Dashboard Preview

> Add your Power BI dashboard screenshot here.

```markdown
![IPL Power BI Dashboard](images/ipl-dashboard.png)
```

---

# 💡 Key Insights

The analysis provides insights into:

* Team dominance and consistency across seasons
* High-performing batsmen and bowlers
* Impact of toss decisions on match outcomes
* Differences between chasing and defending teams
* Venue-specific performance patterns
* Player consistency across matches and seasons

> **Note:** Specific numerical insights should be added here based on the final analysis results from the notebook/dashboard.

---

# 📁 Project Structure

```text
IPL-Data-Analysis/
│
├── 📓 IPL_Analysis.ipynb
│
├── 📊 matches.csv
├── 🏏 deliveries.csv
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

### 1. Clone the repository

```bash
git clone https://github.com/YOUR_USERNAME/YOUR_REPOSITORY.git
```

### 2. Navigate to the project directory

```powershell
cd IPL-Data-Analysis
```

### 3. Create a virtual environment

```powershell
python -m venv .venv
```

### 4. Activate the virtual environment

```powershell
.\.venv\Scripts\Activate.ps1
```

### 5. Install dependencies

```powershell
python -m pip install -r requirements.txt
```

### 6. Open the notebook

Open:

```text
IPL_Analysis.ipynb
```

using **Jupyter Notebook** or **VS Code**.

Run the notebook cells from the project directory so that the CSV files are loaded correctly.

---

# 📦 Requirements

Example dependencies:

```text
pandas
numpy
matplotlib
seaborn
jupyter
```

Install them using:

```bash
pip install -r requirements.txt
```

---

# 🚀 How to Use

### Python Analysis

1. Open `IPL_Analysis.ipynb`
2. Run the notebook cells sequentially.
3. Explore the data cleaning and analysis process.
4. Review the generated charts and statistics.

### Power BI Dashboard

1. Open `IPL DASHBOARD ANALAYSIS.pbix`
2. Refresh the dataset if required.
3. Use the slicers and interactive visuals.
4. Explore team, player, season, and match-level insights.

---

# 📌 Project Objectives

This project demonstrates practical skills in:

* Data Cleaning
* Exploratory Data Analysis
* Data Transformation
* Statistical Analysis
* Data Visualization
* Business Intelligence
* Dashboard Development
* Analytical Storytelling

---

# 🎓 Skills Demonstrated

### Python

```text
Python
 ├── Pandas
 ├── NumPy
 ├── Data Cleaning
 ├── EDA
 └── Data Visualization
```

### Power BI

```text
Power BI
 ├── Data Import
 ├── Data Transformation
 ├── Data Modeling
 ├── DAX
 ├── KPI Development
 ├── Interactive Visualizations
 └── Dashboard Design
```

---

# 🌟 Why This Project?

The IPL generates a large amount of structured sports data. This project demonstrates how raw data can be transformed into meaningful insights using a complete analytics workflow:

**Raw Data → Cleaning → Analysis → Visualization → Insights**

The project is designed as a practical demonstration of **Data Analyst skills using Python and Power BI**.

---

# 🔮 Future Improvements

Potential improvements include:

* [ ] Add advanced DAX measures
* [ ] Add player comparison dashboard
* [ ] Add season-by-season team analysis
* [ ] Add predictive match analysis
* [ ] Add win probability analysis
* [ ] Add advanced batting and bowling metrics
* [ ] Connect Power BI directly to a database
* [ ] Automate data refresh
* [ ] Deploy dashboard for public access

---

# 👨‍💻 Author

**Sherif**

Aspiring Data Analyst | Python | SQL | Power BI | Data Visualization

---

## ⭐ If You Find This Project Useful

If you found this project interesting or useful, consider giving the repository a **⭐ Star**!

Your feedback and suggestions are welcome.
