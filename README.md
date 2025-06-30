# Aviation Low-Risk Aircraft Analysis

For this project, we will use data cleaning, imputation, analysis, and visualization to generate insights for a business stakeholder,and whose company is expanding in to new industries to diversify its portfolio.

## Overview

The company is diversifying into aviation without any prior industry experience and needs data-driven guidance to minimize risk in this high-stakes, multi-million dollar investment where safety directly impacts lives, reputation, and financial success. The challenge is translating 61 years of complex aviation accident data into clear, actionable recommendations for aircraft selection that will enable safe market entry while avoiding costly mistakes. This project tackles the knowledge gap by systematically analyzing NTSB accident data across multiple risk dimensions (manufacturer safety records, engine configurations, operational purposes, and weather conditions) to identify the safest aircraft options and the highest-risk combinations to avoid. The analysis transforms raw accident statistics into concrete business recommendations that prioritize safety as a competitive advantage, providing the aviation division head with evidence-based criteria for aircraft selection.

## Business Understanding

### Stakeholders
- **Primary Stakeholder**: The Head of Aviation Division (the presentation audience) who will make strategic decisions about aircraft acquisition and fleet configuration based on this risk analysis.
- **Secondary Stakeholders**: The company's executive leadership and shareholders who will benefit from reduced operational risk, lower insurance costs, and safer market entry into the aviation sector.
### Key Business Questions
1. Objective: Identify the lowest-risk aircraft for our company's entry into commercial and private aviation markets
2. Goal: Three concrete business recommendations backed by 60+ years of safety data
3 Impact: Strategic guidance for initial aircraft purchases to minimize operational risk


## Data Understanding and Analysis

### Source of Data
- Source: National Transportation Safety Board (NTSB)-Kaggle
- Timeframe: from 1962 to 2023 (61 years of data)
- Scope: Civil aviation accidents and incidents in the US and international waters
- Scale: 70106  total records and 25 fields


### Description of Data
Provide details about your dataset:
- Target Variable: make, model, with low risk of accident, type of engine, purpose of flight.
- Key Features: injury severity, aircraft damage, purpose of flight, weather condition, make, model, type of engine, number of engines, event date, fatal ,sever,e and minor injury columns,
- Data Quality: i kept most of the placeholders to avoid biasness, and also assigned some       missing values to unkown where appropriate to ensure consistency in my data.
### Key Visualizations

#### Visualization 1: Aircraft Safety Overview
![Visualization 1](images/aviation_dashboard.png)
*Top recognized aircraft makes and the number of counts of accidents in 62 years. It clearly shows that Cessna would be the least to consider choosing as it has the highest count of accidents and fatality rate, too as well as could be high*

#### Visualization 2: Aircraft damage by amateur build
![Visualization 2](images/aviation_dashboard.png)
*This vusialization shows how the kind of amatuer build, engine count, and engine type maters when it comes to recommending or choosing a low risk aircraft for private or commercial purposes. Amateur builds seem to have less number of  accidents that damage aircraft, but that should be reconsidered. The more the number of engines, the fewer the number of accidents and fatal injuries, and as seen from the visual, the best type of engine is the one with the lowest count of accidents*

#### Visualization 3: Aircraft Assessment by Purpose
![Visualization 3](images/aviation_dashboard.png)
*Private purpose seems to have the highest count of accidents accopmpanied by injuries, cutting accross fatal, serious, and minor ones. on the other hand, commercial purpose seem to be moderately affected. Regardless, there has been improvements over the years, as seen for all the models, and the number of accidents reduced greatly for all the purposes. Also, some make seem to be working well with both business and personal reasons, they should be prioritized when choosing the lower risk aircraft*

## Methodology

Brief overview of analytical approach
- Data Cleaning: checking for duplicates, null values, dealing with missing data by dropping columns and rows, filling others with Unkown where appropriate, keeping placeholders all that was to ensure I got the right result without bias.
- Exploratory Analysis: using some built-in functions and methods to know what the data entails such include, .info(),.columns,.index, accessing rows and columns by .loc[] and .iloc[], unstacking(), and many others.

## Conclusion

### Summary of Findings

1. Cessna Aircraft Demonstrates Highest Risk Profile:
Cessna leads in total accidents: 23,630 incidents (highest among all manufacturers)
Fatality rate: 7,058 fatal injuries - significantly higher than other manufacturers
Injury severity: 23,630 total injuries, with 12,909 serious injuries

2. Amateur Build Status, Engine Count, and Engine Type Are Critical Risk Factors: ·	Single engine (1)- Highest accident concentration ( Approximately 61,000 plus accidents based on the peak).
	Twin engine (2)- Significantly lower (Approximately 15,000 accidents). Multi-engine (3+)- Much lower accident rates (under 1,000 each). We can see a clear pattern- More engines = better safety profile.
	Amateur-built aircraft: Only 415 total accidents. Professionally-built aircraft: 45,325+ accidents. Key insight: Professional aircraft have 110x more accidents than amateur-built.
And upon selecting any type or number of engines, you get to see the extent of damage to the aircraft.

3. Aircraft Purpose and Manufacturer Trends Reveal Operational Risk Patterns: Aerial Application - 4,228 accidents. Business flights - 3,513 accidents. All other purposes can be seen in the visual.
970s-1980s: Peak accident periods, 700 plus accidents per year. Steady decline: Clear downward trend from the 1980s onward.Modern era (2000s+): Significantly lower accident rates under 200 per year


### Recommendations

Based on the analysis, here are the recommended actions:
- Focus on Business-Configured Aircraft from Manufacturers with Consistent Safety Records like  Mooney. Avoid Cessna at all costs.
- The Triple Safety Filter: Avoid Single-Engine Reciprocating Aircraft, Consider Professional Multi-Engine Turbine Aircraft
- Consider manufacturers with lower incident rates (Boeing, Bell, and Mooney show much better safety profiles)


### Next Steps

- Id have developed a metrix to be more specific on giving a recommendation and for other companies to use as a standard metrix.
- Number of flights per make or model, the cost of the flight, 
- Given enough data losses incurred can be calculated.

## Repository Structure

```
Aviation-Risk-Analysis/
├── .gitignore                   <- .ipynb_checkpoints
├── README.md                    <- This file
├── data/                        <- Data files and analysis
│   ├── aviation_dataset/        <- Original aviation data
│   ├── images/                  <- Visualizations
│   ├── clean_data.csv          <- Final processed data
│   ├── cleaned_data.csv        <- Cleaned dataset
│   └── DSF-FT13 Hy-Phase-1-Project.ipynb  <- Jupyter notebook
└── notebook/                  <- PDF Presentation
```

## Files in This Repository

### Key Visualizations

#### Aviation Risk Analysis Dashboard
![Aviation Risk Analysis Dashboard](images/aviation_dashboard.png)
*Comprehensive dashboard showing aviation safety trends, accident analysis by aircraft type, and key risk factors. This analysis provides stakeholders with actionable insights for improving aviation safety protocols.*
## Tools Used

- anaconda(Python 3.x)
- Pandas for data manipulation
- Numpy 
- Matplotlib/Seaborn for visualization
- Tableau 

Canvas Link(PDF): https://www.canva.com/design/DAGrpKLZRxw/fdxC91xCWOvBhKG2iWX79w/edit?utm_content=DAGrpKLZRxw&utm_campaign=designshare&utm_medium=link2&utm_source=sharebutton

Tableau Link: https://public.tableau.com/app/profile/rosemary.wanjiru/viz/AircraftSafetyOverview
Project Link: https://github.com/r0sh1ddy/Aviation-Risk-Analysis
