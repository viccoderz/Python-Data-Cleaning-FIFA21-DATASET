# Python-Data-Cleaning-FIFA21-DATASET
Introduction
This repository hosts the code and documentation for cleaning and refining the FIFA21 dataset. The project aims to improve the quality and usability of the dataset, which contains valuable information about players featured in the renowned FIFA21 video game.

## Table of Contents
 - [Dataset Source and Overview](#Dataset-Source-and-Overview)
  
 - [Issues found in the data](#Issues-found-in-the-data)
  
 - [Tools Used](#Tools-Used)
  
 - [Data Cleaning Process](#Data-Cleaning-Process)

### Dataset Source and Overview

The FIFA 21 dataset used in this project was obtained from an open-source project, irene-arch.
It consists of player attributes, statistics and other relevant information.

The original FIFA21 dataset contains 18K+ records of player data. Each record represents a unique player and includes
various attributes such as player name, age, nationality, club, overall rating and more.

### Issues found in the data

During the initial exploration and analysis of the FIFA21 dataset, several issues were identified including:

- Missing values - The Hits and Loan Date End columns had missing values which required careful handling and computation.
- Inconsistent formatting - This was observed across different columns making it necessary to standardize the data
  for consistency. The Heights and Weights columns each had values stored in different units.

### Tools Used

For the data cleaning project, the following tools and libraries were used:

1. **Python** for data cleaning tasks.
2. **Pandas** was instrumental in data manipulation, cleaning and handling missing values.
3. **NumPy** was utilized for mathematical operations and array handling during the cleaning process.
4. **Google Collab** provided an interactive environment for code development, exploration and documentation.

### Data Cleaning Process

The data cleaning process involved the following steps:
1. **Data Understanding** - The dataset was thoroughly examined to understand the structure, columns and their meanings.
   The data did not have a data dictionary attached. With the help of online sources I was able to create one that helped me
   gain an understanding of what all the columns represented.
2. **Data Exploration** - Exploratory Data Analysis was performed to gain insights into the data, identify patterns and uncover anomalies.
3. **Handling missing values** - Through the EDA performed, I quickly realised there was a valid reason for the missing values in the Hits and Loan Date End columns.
   The Hits column represented the number of times a player had been searched in the FIFA database. Since some players had never been searched, their records were blank.
   For the Loan Date End column, this represented when the contracts for players who were *On Loan* would end. Since some of the players were free and others
   on contract, their records were left blank.
4. **Standardizing formatting** - Inconsistent formatting issues eg the values in the Heights and Weights columns that were stored with different units were resolved by
   applying transformations, lambda functions and data normalization techniques.
5. **Validation and quality checks** - The cleaned dataset underwent rigorous validation to ensure the quality, accuracy and integrity of the data.
