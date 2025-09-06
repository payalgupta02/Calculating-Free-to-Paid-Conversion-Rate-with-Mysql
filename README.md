## Calculating-Free-to-Paid-Conversion-Rate-with-Mysql
### Project Overview
This project analyzes the student funnel of an edtech platform using SQL. The funnel tracks three stages per student:  
1. **Registration** – when a student signs up.  
2. **First Engagement** – when a student watches their first lecture.  
3. **First Purchase** – when a student subscribes for the first time.  

The aim is to understand student behavior, measure engagement, and calculate the free-to-paid conversion rate. ***Please refer to the attached/uploaded .sql text file with name 'db_course_conversions_Solved' to go through the complete schema structure & analysis**

### Objective
- Measure the **free-to-paid conversion rate** among engaged students.  
- Calculate the **average duration** between registration and first engagement.  
- Calculate the **average duration** between first engagement and first purchase.  
- Identify insights that can inform engagement and monetization strategies.

### Dataset
The project uses three tables from the `db_course_conversions` database:  
- **student_info** – contains registration information of students.  
- **student_engagement** – logs of lectures watched by students.  
- **student_purchases** – details of students’ subscription purchases.  

### Approach / Methodology
1. Explore each table to understand the structure and data quality.  
2. Identify students who have registered but never engaged, and those who engaged but never purchased.  
3. Create a **master table** joining all three tables using LEFT JOINs to capture all students.  
4. Create a **subset table** of engaged students to calculate metrics.  
5. Compute key metrics:  
   - Free-to-paid conversion rate among engaged students.  
   - Average days between registration and first engagement.  
   - Average days between first engagement and first purchase.
<img width="462" height="718" alt="image" src="https://github.com/user-attachments/assets/b2b4fd1d-1d38-4117-b9d1-99812ae59539" />

### Key Metrics & Results
- **Total registered students:** 40,979  
- **Engaged students (watched at least one lecture):** 20,255  
- **Unique purchasers:** 3,138  
- **Free-to-paid conversion rate among engaged students:** 11.29%  
- **Average duration between registration and first engagement:** 3.42 days  
- **Average duration between first engagement and first purchase:** 26.25 days  

### Interpretation & Insights
- Only **half of the registered students** engage with the platform initially.  
- Among engaged students, **~11% convert to paid subscriptions**, highlighting potential for growth.  
- Students typically watch their first lecture within **3-4 days** of registration.  
- The delay between first engagement and purchase suggests that **upselling or targeted reminders** could accelerate conversions.  
