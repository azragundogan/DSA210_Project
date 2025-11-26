# DSA210_Project
Social Media Screen Time Analysis During Exam Weeks  
Author: Azra Gündoğan  
Term: Fall 2025 – Sabancı University  

## Motivation
Social media is an essential part of daily life, but its usage often fluctuates depending on personal and academic stress levels.  
Many students report spending more time on social media during exam periods, either as a form of stress relief or procrastination.  
This project aims to analyze weekly changes in social media screen time and determine whether screen time significantly increases during exam weeks.

## Research Question
Does social media screen time increase during exam weeks compared to regular weeks?

## Hypothesis
On exam days, the increase in entertainment-based screen time (Instagram, TikTok, YouTube) is larger than the increase in communication-based screen time (WhatsApp).

This hypothesis will be tested using descriptive statistics, exploratory data analysis (EDA), and hypothesis testing (t-test or Wilcoxon test depending on data distribution).

## Data Source
The dataset for this project will be self-collected from weekly smartphone screen time reports using iPhone Screen Time or Android Digital Wellbeing.  
Each week’s total screen time for major social media applications (Instagram, TikTok, YouTube, LinkedIn) will be recorded manually in an Excel file.  
Additionally, each week will be labeled as either an exam week (1) or a non-exam week (0), based on the academic calendar.

The final dataset will include columns such as:
- Participant_ID
-Day
-WhatsApp_min
-Instagram_min
-TikTok_min
-YouTube_min
-Total_Screen_min
-Entertainment_min
-Communication_min
-Exam_day_or_not

Data collection will span approximately 2–4 weeks.

## Methods and Tools
Stage | Description  
------|--------------  
Data Collection | Manually record weekly screen time data and exam week labels.  
Data Cleaning | Handle missing or inconsistent values.  
EDA | Calculate averages and visualize screen time trends.  
Statistical Analysis | Use t-test or Wilcoxon test to determine if exam weeks show higher screen time.  
Visualization | Use bar plots and line charts to show weekly changes.  

Libraries: pandas, numpy, matplotlib, seaborn, scipy  

## Project Timeline
Date | Task  
------|------  
Oct 31 | Submit project proposal (this README.md) on GitHub  
Nov 28 | Collect and clean data, perform exploratory data analysis  
Jan 2 | Conduct hypothesis testing and visualization  
Jan 9 (23:59) | Submit final report and presentation  

## Expected Findings
- Screen time is expected to increase during exam weeks.  
- Entertainment platforms (e.g., TikTok, Instagram) may show greater increases compared to professional ones (e.g., LinkedIn).  
- The findings can provide insights into behavioral patterns and stress-related social media use among students.

## Preliminary Results

Using daily screen time data from 7 participants over 7 days, 
I compared entertainment-based apps (Instagram, TikTok, YouTube) and WhatsApp usage 
between exam and non-exam days. 

Preliminary results show that average entertainment minutes are higher on exam days 
than on non-exam days, while the increase in WhatsApp usage is smaller. 
A two-sample t-test was applied to test this difference.


## Academic Integrity
All data will be collected personally and used solely for educational purposes.  
Any use of AI tools (including ChatGPT) for analysis or text generation will be clearly documented in the final report, in accordance with the academic integrity policy of DSA210.
