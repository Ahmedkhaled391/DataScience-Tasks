# DataScience Tasks Documentation

## Overview
This project contains multiple data science tasks focusing on data analysis, cleaning, visualization, and web scraping techniques.

---

## Team members:
Ahmed Khaled          42310090 (TL)
Ziyad Ashraf          42310062
Youssef Ayman         42310376
Ebrahim Ragab         42310461
Abdullah Abdelnaby    42310085
Youssef Ahmed         42310281


## Task 1: Student Performance Factors Analysis

### Objective
Analyze factors affecting student exam performance using a dataset of 6,642 students across both public and private schools.

### Dataset
- **Source:** Kaggle - Student Performance Factors
- **Records:** 6,642 students
- **Features:** 20 variables including study habits, attendance, sleep hours, family income, parental involvement, and school type

### Key Tasks
1. **Data Understanding & Exploration** - Initial data inspection and descriptive statistics
2. **Data Cleaning** - Handle missing values, outliers, and data inconsistencies
3. **Data Analysis** - Answer 15 analytical questions about student performance
4. **Visualization** - Create insightful charts to represent findings

### Research Questions
1. Average Exam Score per Motivation Level
2. Gender differences in average Exam Score
3. Impact of Internet Access on scores
4. Average study hours per Family Income category
5. Learning disabilities prevalence and average scores
6. Public vs private school distribution and performance
7. Exam marks distribution
8. Correlation analysis (Study hours, Attendance, Sleep hours vs Exam Score)
9. Tutoring sessions impact on performance
10. School type and parental income effects
11. Can high effort overcome socioeconomic barriers?
12. Relationship between study time and scores
13. Top 10% vs bottom 10% student comparison
14. High attendance student routines
15. Most common motivation level among top scorers (>85)

### Files
- `Dirty_StudentPerformanceFactors.csv` - Raw data with potential issues
- `Cleaned_StudentPerformanceFactors.csv` - Cleaned dataset ready for analysis
- `StudentPerformanceFactors.csv` - Original dataset
- `task1.ipynb` - Jupyter notebook with analysis

### Technologies Used
- **Python Libraries:** pandas, numpy, matplotlib, seaborn, datasist
- **Techniques:** Data cleaning, exploratory data analysis (EDA), statistical analysis, data visualization

---

## Task 2: Web Scraping and Sports Data Analysis - YallaKora

### Objective
Scrape football match data from YallaKora website and perform comprehensive analysis on match results, teams, and championships.

### Dataset
- **Source:** https://www.yallakora.com/
- **Data Collection Period:** 2024 onwards
- **Target:** Minimum 1,000+ rows of match results
- **Data Points:** Championship, Team A, Team B, Score A, Score B, Time, and Date

### Project Methodology

#### Phase 1: Web Scraping
- Use **BeautifulSoup** and **requests** library to scrape match data from YallaKora
- Extract championship information, teams, scores, match time, and dates
- Handle HTML parsing and data extraction from dynamic content
- Implement error handling for failed requests and incomplete data

#### Phase 2: Data Preprocessing
1. **Handle Missing Values** - Remove empty rows and invalid data
2. **Data Type Conversion** - Convert scores from strings to integers
3. **Data Cleaning** - Remove duplicates and fix inconsistencies
4. **Friendly Match Filtering** - Cap scores for friendly matches (max 4 goals)
5. **Feature Engineering** - Create derived columns:
   - `Result` - Match outcome (Home Win, Away Win, Draw)
   - `Total_Goals` - Total goals scored in a match

#### Phase 3: Data Analysis and Visualization
Answer 5 key analytical questions through visualizations:

1. **Top 10 Championships by Match Count** (Bar Chart)
   - Describes data diversity across championships
   - Identifies most covered leagues/tournaments

2. **Match Results Distribution** (Pie Chart)
   - Analyzes match competitiveness
   - Shows Home Win vs Away Win vs Draw ratios

3. **Total Goals Distribution** (Histogram with KDE)
   - Identifies scoring patterns
   - Detects seasonal variations in goal frequency

4. **Top 10 Most Frequent Home Teams** (Horizontal Bar Chart)
   - Identifies dominant teams in the dataset
   - Shows team representation in collected data

5. **Average Goals for Top 5 Championships** (Bar Chart)
   - Compares goal-scoring intensity across major leagues
   - Identifies high-scoring vs low-scoring competitions

### Files
- `task2.ipynb` - Jupyter notebook with web scraping code and analysis
- `yallakora_data_cleaned.csv` - Output file with cleaned match data

### Technologies Used
- **Web Scraping:** requests, BeautifulSoup4
- **Data Processing:** pandas, numpy
- **Visualization:** matplotlib, seaborn

### Dependencies
All required libraries are listed in `requirements.txt`:
- requests (for HTTP requests)
- beautifulsoup4 (for HTML parsing)
- pandas (for data manipulation)
- numpy (for numerical operations)
- matplotlib (for static visualizations)
- seaborn (for statistical visualizations)
- jupyterlab (for notebook environment)
- datasist (for data science utilities)

---

## Project Structure
```
DataScience-Tasks/
├── requirements.txt           # Project dependencies
├── DOCUMENTATION.md           # This file
├── Task1/
│   ├── task1.ipynb
│   ├── Dirty_StudentPerformanceFactors.csv
│   ├── Cleaned_StudentPerformanceFactors.csv
│   └── StudentPerformanceFactors.csv
└── Task2/
    └── task2.ipynb
```

---

## Setup Instructions

### 1. Install Dependencies
```bash
pip install -r requirements.txt
```

### 2. Running the Notebooks
```bash
jupyter lab Task1/task1.ipynb
jupyter lab Task2/task2.ipynb
```

---

## Key Technologies & Concepts

### Data Science Libraries
- **pandas:** Data manipulation and analysis
- **numpy:** Numerical computations
- **matplotlib & seaborn:** Data visualization

### Web Scraping
- **requests:** HTTP library for web requests
- **BeautifulSoup4:** HTML/XML parsing

### Data Preprocessing Techniques
- Handling missing values
- Data type conversion
- Duplicate removal
- Outlier handling
- Feature engineering

### Analysis Methods
- Exploratory Data Analysis (EDA)
- Descriptive statistics
- Correlation analysis
- Comparative analysis
- Distribution analysis

---

## Notes for Developers

- Task 1 focuses on structured data analysis with clean datasets
- Task 2 demonstrates real-world web scraping challenges and data quality issues
- Both tasks emphasize proper data cleaning before analysis
- Visualizations are created to answer specific business questions
- Code includes error handling for robust execution

---

**Last Updated:** May 2, 2026
