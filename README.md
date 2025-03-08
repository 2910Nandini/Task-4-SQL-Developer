# Task-4-SQL-Developer
# Window Functions
# Objective: Utilize SQL window functions to rank students and perform cumulative analysis.
# Project Steps
1. Dataset Setup
● Create and Populate Table:
Define a table Students with fields like:
○ StudentID (Primary Key)
○ Name
○ MathScore
○ TotalScore
● Populate with sample data for the analysis.
2. Tasks to Perform
Task 1: Rank Students Based on Total Scores
● Query Objective: Use the RANK() function to assign ranks to students based on their
TotalScore.
● Query Explanation:
○ Use RANK() OVER (ORDER BY TotalScore DESC) to rank students in
descending order of their total scores.
○ If two students have the same score, they receive the same rank, and the next
rank is skipped.
Task 2: Calculate Running Totals for Math Scores
● Query Objective: Use the SUM() function with OVER() to calculate running totals of
MathScore ordered by StudentID.
● Query Explanation:
○ Use SUM(MathScore) OVER (ORDER BY StudentID) to compute a
cumulative total.
○ This provides the total Math score up to each student in the order specified
