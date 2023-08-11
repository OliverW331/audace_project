# Audace Project - Script Directory

This directory contains scripts related to the processing, classification, and visualization of articles from various sources.

## 1. **proquest_corpus_documentation.ipynb**
- **Purpose**: Splits and cleans modern English articles downloaded from the Canadian Newstream database of [ProQuest](https://www.proquest.com/canadiannews/news/fromDatabasesLayer?accountid=12339).
- **Output**: Cleaned articles in `cleaned_corpus/english_modern` directory.
- **Improvements Needed**:
  - Optimize the `remove_duplicates` function.
  - Adjust for the change in the modern period to 1995-2015.
  - Handle new search words and folder naming.

## 2. **eureka_corpus_documentation.ipynb**
- **Purpose**: Splits and cleans modern French articles downloaded from Eureka.
- **Output**: Cleaned articles in `cleaned_corpus/french_modern` directory.
- **Improvements Needed**:
  - Develop a function to remove duplicates.
  - Adjust for the change in the modern period.
  - Ensure file separation works with varying regular expression patterns.

## 3. **random_50.ipynb**
- **Purpose**: Assigns transcription tasks to team members to check the OCR error rate.

## 4. **english_classification_LDA.ipynb**
- **Purpose**: Conducts unsupervised classification on the English modern corpus.
- **Sections**:
  - Data Cleaning
  - Selecting Number of Topics
  - Training
  - Classification
- **Improvements Needed**: Examine labeling accuracy.

## 5. **classification_LDA_include_subject.ipynb**
- **Purpose**: Similar to `english_classification_LDA.ipynb` but includes subject words from the database.

## 6. **french_classification_LDA.ipynb**
- **Purpose**: Conducts unsupervised classification on the French modern corpus.
- **Improvements Needed**:
  - Enhance data cleaning.
  - Complete the classification of the French corpus.

## 7. **classificationi_nomic.ipynb**
- **Purpose**: Imports data from the English modern corpus and visualizes clustering using the NOMIC API.

## 8. **classification_BERT.ipynb**
- **Purpose**: Performs supervised classification based on the LDA model's results.
- **Sections**: Pytorch and Tensorflow
- **Improvements Needed**:
  - Examine label accuracy.
  - Analyze data frame metrics.
  - Tune models for better accuracy.
  - Visualize the attention matrix.
