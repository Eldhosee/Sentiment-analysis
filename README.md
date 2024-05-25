# Sentiment Analysis of User Reviews

## Overview

This document summarizes the approach, challenges faced, and assumptions made during the sentiment analysis of user reviews.

## Approach

1. **Data Loading**: The dataset `user_review.xls` was loaded using `pandas`.
2. **Data Cleaning**: Null values were removed to ensure data integrity.
3. **Text Preprocessing**: 
    - **Accent and Special Character Removal**: Used `unidecode` to convert accented characters to their ASCII equivalents.
    - **Lowercasing**: Converted all text to lowercase for uniformity.
    - **Punctuation Removal**: Used `re.sub` with a regex pattern to remove punctuation.
4. **Sentiment Analysis**: 
    - Implemented using VADER from the NLTK library.
    - Reviews were classified as Positive, Negative, or Neutral based on the compound sentiment score.
5. **Visualization**: Created a bar chart to display the distribution of sentiment categories.
6. **Report Generation**: A summary report was printed to the console and saved to `summary_report.md`.

## Challenges Faced

1. **Text Preprocessing**: Ensuring that all special characters and punctuations were correctly removed required careful regex handling.
2. **Visualization**: Ensuring the bar chart accurately represented the sentiment distribution and was visually appealing.

## Assumptions Made

1. **Data Integrity**: Assumed the input CSV file was clean except for null values.
2. **Language and Context**: Assumed the reviews were primarily in English and that the VADER tool would be appropriate for sentiment analysis.
3. **Sentiment Score Thresholds**: Used standard thresholds (>=0.05 for Positive, <=-0.05 for Negative, and in between for Neutral) based on VADER's recommendations.



      
## Sentiment Analysis

The script uses VADER for sentiment analysis. Reviews are classified as Positive, Negative, or Neutral based on the compound sentiment score.



