#### CSCE676-DataMiningProject

# Geographic Differences in YouTube Search Results

## Project Overview
This project analyzes whether geographic location influences YouTube search results and how this affects exposure to misinformation. Using a YouTube audit dataset, I compare results from the United States and South Africa to understand differences in content, channel exposure, and misinformation rates. I analyzed search results across countries, queries, filters, and time. I applied data mining techniques to identify patterns in channel repetition, rates of misinformation, and result consistency. The goal is to understand whether YouTube search results behave differently based on the user's location, and how this may impact the information users are being exposed to.

The videos that people see can shape what their beliefs, especially when it comes to controversial topics. If search results differ across geographic locations, users in different countries may be exposed to different perspectives or levels of misinformation. Understanding these differences is important because repeated exposure to the same types of content or sources can shape user beliefs. 

## Main notebook
The main deliverable is here: https://github.com/j-salguero/CSCE676-DataMiningProject/blob/main/main_notebook.ipynb

## Research Question
Does geographic location influence YouTube search results for the same query, and does this affect exposure to misinformation?

## 2-Minute Project Overview
- Youtube: https://youtu.be/SuMNdmeI3cU
- Slides: https://github.com/j-salguero/CSCE676-DataMiningProject/blob/main/937005006_CSCE676_2-MinuteVideoSlides.pdf

## Data
I chose "Algorithmic Behaviors Across Regions: A Geolocation Audit of YouTube Search for COVID-19 Misinformation Between the United States and South Africa"
- Authors: Hayoung Jung, Prerna Juneja, Tanushree Mitra
- https://github.com/social-comp/YouTubeAuditGeolocation-data/tree/main
- Data within this repo: https://github.com/j-salguero/CSCE676-DataMiningProject/blob/main/search-results.zip

After downloading the data, I combined the individual files for each city into one large dataset. To get the data ready for analysis, I grouped the results by country, query, and run. Each group was treated like a set of channels that appeared together in the search results. These steps can be seen in the main_notebook.ipynb preprocessing steps.

## How to Reproduce
This was build using Jupyter Notebook and Google Colab. To build a similar environment, please reference [requirements.txt](https://github.com/j-salguero/CSCE676-DataMiningProject/blob/main/requirements.txt)

Key Dependencies: 
- Python  
- pandas  
- numpy  
- matplotlib  
- prefixspan  

## Repo Structure
CSCE676-DataMiningProject/
│
├── checkpoints/ # Intermediate project work
│ ├── 937005006_CSCE676_ProjectCheckPoint1.ipynb # Project 1 Checkpoint: Dataset Comparison, Selection, and EDA
│ └──  937005006_CSCE676_ProjectCheckPoint1.ipynb # Project Checkpount 2: Research Question Formation
│
├── main_notebook.ipynb # Final curated notebook (main deliverable)
├── search-results.zip # Dataset used for analysis
├── requirements.txt # Python dependencies
│
├── 937005006_CSCE676_2-MinuteVideoSlides.pdf # Slides from 2-minute video about project
└── README.md # Project overview

## Results Summary
The results of this project show that geographic location does influence YouTube search results for the same query. Users in different countries are exposed to different channels, and these differences can lead to different levels of misinformation exposure. While search results are relatively consistent across runs, the specific channels and channel groupings vary by location. Geographic location does play an important role in determining how much misinformation users are being exposed to on YouTube.

