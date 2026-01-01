🎓 Students Performance Tracker
Students Performance Tracker is a Power BI analytics project for exploring student performance in math, reading, and writing, along with demographic and contextual factors such as gender, race/ethnicity, parent education, lunch type, and test preparation course participation.

✨ Features
📊 Core Data Model

StudentsPerformance table with cleaned and renamed columns:

Student ID
Gender
Race/Ethnicity
Parent Education
Lunch
Test Preparation Course
Math Score
Reading Score
Writing Score



🧮 Calculated Columns

Score – average of Math, Reading, and Writing scores.
Grade – letter grade (O, A–F) based on the Score using SWITCH logic.

📈 Analytical Measures

No of Students – distinct student count.
Average Score, Avg Math, Avg Reading, Avg Writing.
Gender distribution – percentage of:

Male Students
Female Students


Distribution metrics:

Min Score
Max Score
Median Score
Score Pctile 25
Score Pctile 75
Score IQR and IQR splits
Dynamic Y axis Max



🖼 SVG-Based Visual Measures

Circular progress visuals for Math, Reading, and Writing based on average subject scores.
A progress bar visual for overall average score with color changing by performance band.


📁 Project Contents

Students Performance Tracker.pbix (or .pbit) – main Power BI report file with pages, visuals, and interactions.
Model.bim – semantic model definition (tables, relationships, calculated columns, and DAX measures) used by the report.
data/StudentsPerformance.xlsx – source Excel file with the raw student performance dataset (if included in the repo).
README.md – project overview and usage instructions.


🗂 Data Source

Data is loaded from StudentsPerformance.xlsx, sheet StudentsPerformance, with headers promoted and data types set for each column.
Columns are renamed to analysis-ready names (for example, gender → Gender, math score → Math Score).


🔧 If you clone this project, update the file path in the Power Query M code or configure the data source in Power BI so it points to your local StudentsPerformance.xlsx instead of the original drive path (for example, C:\...).


🚀 How to Use

Open Students Performance Tracker in Power BI Desktop.
Confirm or update the data source to point to your local copy of StudentsPerformance.xlsx.
Refresh the dataset so all measures, calculated columns, and visuals are computed correctly.
Explore the report pages:

Overall KPIs (Average Score, Avg Math/Reading/Writing).
Distribution and grade breakdown using boxplot measures and the Grade Sort table.
Demographic slices by gender, race/ethnicity, parent education, lunch type, and test preparation course.




🔧 Extending the Project

Add new measures (for example, pass rate, subject-wise variance, or year-over-year comparisons).
Introduce new dimensions such as class, school, or region if your dataset supports them.
Customize or add report pages focusing on specific stakeholders (teachers, administrators, or students).
