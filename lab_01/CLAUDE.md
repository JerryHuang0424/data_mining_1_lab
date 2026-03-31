# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a Data Mining lab project focused on customer segmentation analysis. The project contains a Jupyter notebook template for data exploration and preprocessing of customer data to build classification models for customer segmentation.

## Dataset Information

- **File**: `customer.csv` (originally named `Train.csv` in the notebook)
- **Source**: Analytics Vidhya hackathon
- **Target Variable**: `Segmentation` (A, B, C, D segments)
- **Features**:
  - Demographic: ID, Gender, Ever_Married, Age, Graduated, Family_Size
  - Professional: Profession, Work_Experience
  - Behavioral: Spending_Score, Var_1 (anonymized category)

## Notebook Structure

The main notebook `Lab1-Data Exploration.ipynb` follows a structured data analysis workflow:

1. **Data Loading & Initial Inspection** - Load dataset and examine basic structure
2. **Data Cleaning** - Handle missing values, duplicates, and data validity
3. **Feature Engineering** - Create new features like age groups
4. **Preprocessing** - Encoding categorical variables and scaling
5. **Exploratory Analysis** - Univariate, bivariate, and multivariate analysis
6. **Segment Profiling** - Analyze characteristics of each customer segment

## Workflow

1. Before running any Python code, ensure conda environment is used
2. Use `conda run -n neural_network` instead of activating environment
3. All dependencies must be installed in this environment

## Common Development Tasks

### Running the Notebook
- The notebook expects the dataset to be named `Train.csv` in the same directory
- Currently uses `customer.csv` - update the file path in cell 4 to `'customer.csv'`
- Execute cells sequentially to follow the data analysis workflow

### Data Analysis Workflow
1. Start with data loading and initial inspection
2. Handle missing values (some columns like Work_Experience have missing data)
3. Perform exploratory data analysis
4. Generate insights for customer segmentation
5. Answer the business questions in the final section

## Key Files

- `Lab1-Data Exploration.ipynb` - Main analysis notebook
- `customer.csv` - Dataset for customer segmentation
- `customer_description.txt` - Dataset documentation and variable definitions

## Important Notes

- The notebook is designed as a lab template with TODO sections for students to complete
- The analysis focuses on building classification models to predict customer segments
- Business context: Automobile company expanding to new markets using existing segmentation strategy
- Target segments: A, B, C, D (from existing market)