## Calculating-Free-to-Paid-Conversion-Rate-with-Mysql
### Project Overview
This project analyzes the student funnel of an edtech platform using SQL. It tracks three stages per student:
**Registration** – All students who signed up.
**First Engagement** – Students who watched their first lecture.
**First Purchase** – Students who purchased their first paid subscription.

The goal is to understand the conversion from free to paid users, and the average duration students take between registration, engagement, and purchase.

Objectives

Calculate the Free-to-Paid Conversion Rate among engaged students.

Determine the average time between registration and first engagement.

Determine the average time between first engagement and first purchase.

Provide insights to help the platform improve user engagement and monetization.

Dataset

The project uses three tables:

Table	Description
student_info	Contains all registered students and their registration dates.
student_engagement	Logs all engagement events (lecture watched) by students.
student_purchases	Logs all purchase events (subscriptions) by students.
Approach / Methodology

Explore the tables and understand the funnel.

Identify students who registered but never engaged, engaged but never purchased, and purchased without engagement.

Create a master table combining all three tables using LEFT JOIN to retain all students.

Create a subset of engaged students for calculating the free-to-paid conversion.

Calculate key metrics:

Free-to-paid conversion rate.

Average duration from registration to first engagement.

Average duration from first engagement to first purchase.
