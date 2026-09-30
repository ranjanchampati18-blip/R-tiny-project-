# Student Performance Analysis — R Markdown Tiny Project

## 1. Project title
**Student Performance Analysis**

## 2. Topic selection
This project uses a small student-performance dataset to demonstrate the complete Practical 8–10 R Markdown workflow.

The supplied practical already demonstrates CSV importing, `head()`, `summary()`, `str()`, missing-value checks, descriptive statistics, categorical counts, pie charts, bar plots, and attendance–marks correlation. This Tiny Project reorganizes and expands those elements into a complete reproducible report. The original practical's dataset contains 12 students and the fields Student_ID, Name, Gender, Age, Marks, Attendance, and Result. 

## 3. Dataset
File: `data/student_performance.csv`

Rows: 12

Variables:
- `Student_ID` — student identifier
- `Name` — student name
- `Gender` — categorical gender field
- `Age` — age in years
- `Marks` — marks out of 100
- `Attendance` — attendance percentage
- `Result` — Pass/Fail

## 4. Analysis included
- CSV data importing
- Data inspection and validation
- Missing-value checking
- Duplicate-ID checking
- Text trimming and factor conversion
- Numeric type conversion
- Descriptive statistics
- Gender and result frequency analysis
- Pie charts
- Student marks bar chart
- Attendance bar chart
- Attendance vs. marks scatter plot
- Pearson correlation
- Simple linear regression
- Grouped mean comparisons
- Interpretation, findings, limitations, and conclusion

## 5. Key computed results
- Mean marks: 69.50
- Median marks: 70.00
- Standard deviation of marks: 18.15
- Marks range: 38–95
- Mean attendance: 79.92%
- Pass rate: 83.33%
- Attendance–marks Pearson correlation: 0.992637

## 6. Software requirements
- R 4.0 or later
- RStudio recommended
- `rmarkdown`
- `knitr`

The analysis itself uses base R functions, so no tidyverse or other analysis packages are required.

## 7. How to run
1. Extract the project folder.
2. Open `student_performance.Rmd` in RStudio.
3. Make sure the `data` folder remains beside the Rmd file.
4. Install required packages if necessary:
   `install.packages(c("rmarkdown", "knitr"))`
5. Click **Knit → Knit to HTML**.
6. The rendered report can be saved as `output/student_performance_report.html`.

## 8. Project structure

```text
R_Tiny_Project_Student_Performance/
├── student_performance.Rmd
├── README.md
├── requirements.txt
├── data/
│   └── student_performance.csv
├── source/
│   └── student_performance_analysis.R
├── plots/
│   ├── gender_distribution.png
│   ├── result_distribution.png
│   ├── student_marks.png
│   ├── student_attendance.png
│   └── attendance_vs_marks.png
└── output/
    └── student_performance_report.html
```

## 9. Important interpretation note
The dataset has only 12 observations. Therefore, the results are suitable for a classroom Tiny Project and demonstration of R Markdown methods, but they should not be generalized to a wider student population without a larger and appropriately sampled dataset.

## 10. Source basis
The dataset values and practical operations were taken from the uploaded Practical 8–10 material supplied with this task.
