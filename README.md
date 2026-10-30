# Student Academic Performance Analysis

An interactive **Power BI** dashboard analyzing how gender, race/ethnicity and parental education relate to students' exam scores.

## Dashboard Preview

![Dashboard](screenshots/dashboard.png)

> Add your dashboard screenshot as `screenshots/dashboard.png`.

## Project Goal

Understand which factors are linked to student performance in **math, reading and writing**, and turn the findings into clear recommendations.

## Dataset

- **File:** `data/study_performance.csv`
- **Rows:** 1,000 students (no missing values)

| Column | Description |
|---|---|
| `gender` | Student gender |
| `race_ethnicity` | Group A to E |
| `parental_level_of_education` | Highest education level of parents |
| `lunch` | Standard or free/reduced |
| `test_preparation_course` | Completed or none |
| `math_score` | Math score (0-100) |
| `reading_score` | Reading score (0-100) |
| `writing_score` | Writing score (0-100) |

**Calculated column:** `Overall Score = (math + reading + writing) / 3`

## Dashboard Visuals

| Visual | Chart type | Purpose |
|---|---|---|
| Test Preparation Course | Bar chart | Overall performance of students who completed the prep course vs those who did not |
| Average of Overall Score by Gender | Pie chart | Performance split between male and female students |
| Performance Gap by Race/Ethnicity | Donut chart | Gap between groups A to E |
| Impact of Parental Education on Scores | Bar chart | Effect of parents' education on scores |

## Key Insights

- Average overall score is **67.77** out of 100.
- Students who completed the test preparation course average **73**, compared with **65** for those who did not.
- Female students lead overall (**69.57** vs **65.84**) and in reading and writing; male students lead in math (**68.73** vs **63.63**).
- Scores rise from **Group A (62.99)** to **Group E (72.75)**, a gap of about 9.8 points.
- Students whose parents hold a Master's degree average **73.60**, compared with **63.10** for high school, a gap of 10.5 points.

## Recommendations

1. Strengthen math support for girls.
2. Boost reading and writing support for boys.
3. Target the lowest-scoring groups (A and B) with tutoring and resources.
4. Support students whose parents have less education with follow-up and homework help.

## Repository Structure

```
.
├── dashboard/
│   └── study_performance.pbix
├── data/
│   └── study_performance.csv
├── docs/
│   ├── insights.html
│   └── conclusion_recommendations.html
├── screenshots/
│   └── dashboard.png
├── .gitignore
└── README.md
```

## How to Open

1. Install [Power BI Desktop](https://powerbi.microsoft.com/desktop/) (free, Windows).
2. Download `dashboard/study_performance.pbix`.
3. Open it in Power BI Desktop. If the data source path breaks, go to **Transform data → Data source settings → Change Source** and point it to `data/study_performance.csv`.

## Tools

Power BI Desktop, DAX, Power Query

## Author

**Mohamed Salem**: [LinkedIn](https://www.linkedin.com/in/mohamed-salem-b67689446) | [GitHub](https://github.com/mohamedsalem26)

*Route Academy, Power BI Assignment 2*
