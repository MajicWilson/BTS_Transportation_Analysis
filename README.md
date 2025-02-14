# Problem Statement
Transportation systems are critical to modern economies, ensuring the smooth movement of people, goods, and services. However, as these networks expand, they face increasing challenges such as congestion, safety issues, infrastructure strain, and environmental concerns. The Bureau of Transportation Statistics (BTS) collects vast amounts of data related to transportation, covering various modes such as road, rail, air, and water. Despite the availability of this data, inefficiencies persist in transportation systems, leading to economic disruptions and environmental impacts. The challenge is to analyze BTS data effectively to uncover actionable insights that can improve transportation efficiency, enhance safety, and support sustainable development. This project aims to utilize data analytics to extract meaningful patterns, identify inefficiencies, and recommend strategic improvements to BTS stakeholders.
# Objectives
The main objective of this project is to analyze the transportation data provided by the Bureau of Transportation Statistics (BTS) to uncover insights related to the efficiency, safety, and environmental impacts of freight transportation across various modes (road, rail, air, and water). Other key objectives are to;

Analyze freight movement across transportation modes: Study trends in the volume, routing, and modes used for transporting goods across regions and time periods.

Identify inefficiencies in transportation systems: Find areas of congestion, delays, or underused infrastructure and suggest ways to improve resource use and throughput.

Assess environmental impact: Examine emissions, fuel use, and sustainability metrics across transportation modes, and recommend ways to reduce the sector's carbon footprint.

Evaluate transportation safety: Investigate safety incidents related to freight, understand their causes, and propose improvements to safety protocols.

Examine the impact of economic disruptions: Analyze how factors like trade changes, policy shifts, or global events affect freight movements and transportation efficiency.
# Project Phases Using the Cross-Industry Standard Process for Data Mining (CRISP-DM) Methodology
##  Business Understanding
The goal was to explore the challenges faced by transborder freight systems and understand how factors like congestion and inefficiency impact the movement of goods between the U.S., Canada, and Mexico. With rising trade volumes and strained infrastructure, optimizing these systems is critical for economic growth.
## Data Understanding
The dataset spans freight border data from 2020 to 2024, coming in zipped files with monthly folders containing CSV files (dot1, dot2, dot3, and YTD). The data had various complexities such as duplicates, missing values in specific columns, and varying file structures. I created three main dataframes by concatenating all dot1, dot2, and dot3 files across months and years to maintain consistency.
## Data Preparation
Data Cleaning: Duplicate records were removed, and missing values were handled carefully. Missing values in columns like MEXSTATE and CANPROV were small (7%), so they were dropped. Missing DF column values were filled using the mode based on USASTATE grouping.

Outlier Handling: Outliers in numerical variables (SHIPWEIGHT, FREIGHT CHARGES, and VALUE) were identified using boxplots and addressed through log transformation to ensure more accurate analysis.

Data Type Adjustment: Data types were modified as needed to ensure compatibility for analysis.
## Modeling
Exploratory Data Analysis (EDA) was conducted in several steps:

Univariate Analysis: Examined the distribution of numerical and categorical variables.

Multivariate Analysis: Investigated relationships between variables to identify patterns and correlations, especially between freight charges, weight, and value, which showed a positive correlation.

Hypothesis Testing: Based on data insights, hypotheses were formed regarding the impact of congestion, delays, and economic disruptions on freight systems, which were tested through statistical methods.
## Evaluation
Insights from the EDA and hypothesis testing helped identify key inefficiencies and areas needing attention, such as underutilized infrastructure and high-congestion points. Recommendations were made to improve the system's throughput, reduce environmental impact, and enhance safety protocols based on the analysis.
## Deployment
The final insights and recommendations were aimed at informing strategies to optimize transborder freight systems. These included improving infrastructure, streamlining customs processes, reducing emissions, and enhancing safety measures to ensure smoother trade flow between the U.S.A, Canada, and Mexico.
