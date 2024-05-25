# Sentiment Analysis of User Reviews

## Overview

This project performs sentiment analysis on user reviews using the VADER (Valence Aware Dictionary and sEntiment Reasoner) sentiment analysis tool from the NLTK library. The project involves loading a dataset of user reviews, preprocessing the text data, analyzing the sentiment, and visualizing the sentiment distribution.

## Data Preprocessing


The preprocessing steps include:

1. **Removing Accents and Special Characters**:
    
    - Uses `unidecode` to standardize text.
2. **Converting to Lowercase**:
    
    - Ensures uniform text by converting all characters to lowercase.
3. **Removing Punctuation**:
    
    - Uses regular expressions to remove punctuation.
      
## Sentiment Analysis

The script uses VADER for sentiment analysis. Reviews are classified as Positive, Negative, or Neutral based on the compound sentiment score.

## Visualization

A bar chart visualizes the sentiment distribution of user reviews. The chart displays the number of Positive, Negative, and Neutral reviews.

