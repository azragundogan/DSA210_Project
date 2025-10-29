# DSA210_Project
LinkedIn Engagement Analysis – Exploring how hashtags and photos affect post performance.

# DSA210 Project: LinkedIn Engagement Analysis  
Author: Azra Gündoğan  
Term: Fall 2025 – Sabancı University  

## Motivation
LinkedIn is one of the most widely used professional networking platforms where individuals and companies share content to increase visibility and engagement. However, not all posts perform equally well. Some posts go viral while others remain unnoticed.  
This project aims to analyze which factors increase engagement (likes and comments) on LinkedIn posts, focusing especially on the number of hashtags used and whether the post includes a photo.  
Understanding these factors can help professionals and organizations design more effective communication strategies for higher reach and visibility.

## Research Question
What types of LinkedIn posts receive higher engagement, and how do hashtags and photos affect user interaction?

## Hypothesis
LinkedIn posts that include 2–4 hashtags and contain an image receive significantly higher engagement (likes and comments) than posts without images or with fewer or more hashtags.  
This hypothesis will be tested statistically using exploratory data analysis (EDA), correlation analysis, and a two-way ANOVA test to evaluate the individual and combined effects of hashtags and image presence.

## Data Source
The dataset will be obtained from a public LinkedIn Post Analytics dataset on Kaggle, which includes variables such as:  
- post_text (text content of the post)  
- num_hashtags (number of hashtags used)  
- has_image (binary variable: 1 = image, 0 = no image)  
- likes, comments (engagement metrics)  
- post_date (publication date)  

Additionally, a small sample of real LinkedIn posts (approximately 20–30) may be manually collected to capture more recent posting trends.

## Methods and Tools
Stage | Description  
------|-------------  
Data Cleaning | Handle missing values, calculate total engagement (likes + comments).  
EDA | Visualize the relationships between hashtags, photos, and engagement levels.  
Statistical Analysis | Perform two-way ANOVA to test the interaction effects.  
ML (optional) | Use regression models to predict engagement scores.  
Visualization | Create plots with Matplotlib or Seaborn (e.g., boxplots, bar charts).  

Libraries: pandas, numpy, matplotlib, seaborn, statsmodels, scikit-learn  

## Project Timeline
Date | Task  
------|------  
Oct 31 | Submit project proposal (this README.md) on GitHub  
Nov 28 | Collect and clean data, perform exploratory data analysis  
Jan 2 | Apply statistical and machine learning methods  
Jan 9 (23:59) | Submit final report and presentation  

## Expected Findings
- Posts that include images tend to receive higher average engagement.  
- Engagement increases up to a moderate hashtag count (2–4) and then decreases.  
- The combination of an image and an optimal number of hashtags produces the best results.  
- Excessive hashtags or lack of visuals may reduce engagement.  

## Academic Integrity
All data used in this project will be publicly available and properly cited.  
Any use of AI tools (including ChatGPT) for text or code generation will be documented clearly in the final report, in accordance with the academic integrity policy of DSA210.

