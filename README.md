# DSA210_Project
Social Media Screen Time Analysis During Exam Weeks  
Author: Azra Gündoğan  
Term: Fall 2025 – Sabancı University  

## Motivation
Social media is an essential part of daily life, but its usage often fluctuates depending on personal and academic stress levels.  
Many students report spending more time on social media during exam periods, either as a form of stress relief or procrastination.  
This project aims to analyze weekly changes in social media screen time and determine whether screen time significantly increases during exam weeks.

## Data Description

The dataset used in this project was collected from third-year Industrial Engineering students.  
The data covers a two-week period during which students were actively taking midterm exams.

All screen time data was self-recorded by the participants screen time app. It includes daily usage durations of communication-based and entertainment-based mobile applications.


## Research Question
Is entertainment-based screen time significantly greater than communication-based screen time on exam days?

## Hypothesis
  The main goal of this project is to determine if students’ phone usage patterns change on exam days.
Rather than looking only at how much time they spend on their phones, the project focuses on how they spend that time — whether they tend to use more entertainment apps (Instagram, TikTok, YouTube) or communication apps (WhatsApp) when they are under exam-related stress.

H₀: On exam days, entertainment-based screen time is <= communication-based screen time.

H₁:On exam days, entertainment-based screen time is > communication-based screen time.


## Data Source
The dataset for this project will be self-collected from weekly smartphone screen time reports using iPhone Screen Time or Android Digital Wellbeing.  
Each week’s total screen time for major social media applications (Instagram, TikTok, YouTube, LinkedIn) will be recorded manually in an Excel file.  
Additionally, each week will be labeled as either an exam day (1) or a non-exam day (0), based on the academic calendar.

The final dataset will include columns such as:
-Participant_ID, Day, WhatsApp_min, Instagram_min, TikTok_min, YouTube_min, Total_Screen_min, Entertainment_min, Communication_min, Exam_day_or_not

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

## Preliminary Results (28 November)

Using daily screen time data from 7 participants, 
I compared entertainment-based apps (Instagram, TikTok, YouTube) and WhatsApp usage 
between exam and non-exam days.

On average, entertainment minutes were higher on exam days 
(277 min) than on non-exam days (187 min), while WhatsApp usage 
was slightly lower on exam days (48 vs. 63 min). 

Two-sample t-tests did not detect statistically significant differences 
at the 5% level (p = 0.32 for entertainment, p = 0.15 for WhatsApp), 
but the direction of the effects is consistent with the hypothesis that 
students shift more of their screen time toward entertainment apps on exam days.

## Machine Learning Analysis (2 January)

In this project, a supervised machine learning approach was applied to examine whether daily screen time patterns can predict whether a day is an exam day.

A Logistic Regression model was used, where the target variable was `Exam_day_or_not` (1 = exam day, 0 = non-exam day). The input features included:
- Entertainment_min  
- Communication_min  
- Total_Screen_min  

The dataset was split into training and testing sets, and the model was evaluated using accuracy, a confusion matrix, and a classification report.

The model achieved an accuracy of approximately 39%, indicating that screen time variables alone have limited predictive power in determining exam days. This suggests that while differences in usage patterns exist, they are not strong enough on their own to reliably classify exam versus non-exam days.

Feature coefficients from the logistic regression model indicate that entertainment-based screen time has a positive association with exam days, while communication-based and total screen time show negative associations. However, these effects are relatively small, highlighting the complexity of behavioral patterns during exam periods.

## Final Notes

All statistical analyses, hypothesis testing, visualizations, and machine learning results are provided in the Jupyter notebook (`analysis.ipynb`).  
The README serves as a high-level overview of the project, while the notebook contains the full analytical workflow and outputs.

This project demonstrates an end-to-end data analysis process, from data collection and exploratory analysis to hypothesis testing, visualization, and basic machine learning modeling.


## Academic Integrity
All data will be collected personally and used solely for educational purposes.  
Any use of AI tools (including ChatGPT) for analysis or text generation will be clearly documented in the final report, in accordance with the academic integrity policy of DSA210.

