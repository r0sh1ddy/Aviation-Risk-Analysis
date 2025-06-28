# Project Title

Brief description of your project in 1-2 sentences.

## Overview

Provide a clear, concise overview of your project. What problem does it solve? What is the main goal? This should be 2-3 paragraphs that give readers a quick understanding of what your project is about.

## Business Understanding

### Stakeholders
- **Primary Stakeholder**: [Who is the main beneficiary of this analysis?]
- **Secondary Stakeholders**: [Who else would benefit from these insights?]

### Key Business Questions
1. Objective: Identify lowest-risk aircraft for our company's entry into commercial and private aviation markets
2. Goal: Three concrete business recommendations backed by 60+ years of safety data
3 Impact: Strategic guidance for initial aircraft purchases to minimize operational risk


## Data Understanding and Analysis

### Source of Data
- Source: National Transportation Safety Board (NTSB)
- Timeframe: 1962-2023 (61 years of data)
- Scope: Civil aviation accidents and incidents in US and international waters
- Scale: 70106  total records 25 fields


### Description of Data
Provide details about your dataset:
- Target Variable: make,model with low risk of accident, type of engine, purpose of flight.
- Key Features: injury severity, aircraft damage, purpose of flight, weather condition,make, model, type of engine, number of engines, event date,fatal,severe and minor injury columns,
- Data Quality: i kept most of the placeholders to avoid biasness, and also assigned some       missing values to unkown where appropriate to ensure consistency in my data.
### Key Visualizations

#### Visualization 1: Aircraft Safety Overview
Visualization 1- (images/aviation_dashboard.png)
*Top recognized aircraft makes and the number of counts of accident in 62 years. It clearly shows that Cessna would be the least to consider choosing as it has the highest count of accidents and fatality rate too as well could be high*

#### Visualization 2: Aircraft damage by amature build
Visualization 2- (images/aviation_dashboard.png)
*This vusialization shows how the kind of amatuer build, engine count and engine type maters when it comes to recommending or choosing a low risk aircraft for private or commercial purposes. Amature build seem to have less number of  accidents that damaging aircraft but that should be reconsidered, the more the number of engines the less the number of accidents and fatal injuries and as seen from the visuals the best type of egine is the one with low count of accidents*

#### Visualization 3: Aircraft Assessment by Purpose
![Visualization 3](images/aviation_dashboard.png)
*Private purpose seem to have the highest count of accidents accopmpanied by injuries cutting accross fatal, serious, and minor ones. on the other hand commercial purpose seem to be moderately affected. Regardless there has been improvements over the years as seen for all the models and the number of accidents reduced greatly for all the purposes. Also some make seem to be working well with both business and personal reasons they should be prioritized when choosing the lower risk aircraft*

## Methodology

Brief overview of analytical approach
- Data Cleaning: checking for duplicates, null values, dealing with missing data by dropping columns and rows, filling others with Unkown where appropriate, keeping placeholders all that was to ensure i got the right result without bias.
- Exploratory Analysis: using some built in functiond and methods to know what the data entails such include, .info(),.columns,.index, accessing rows and columns by .loc[] and .iloc[], unstacking() and many others.

## Conclusion

### Summary of Findings

1. Cessna Aircraft Demonstrate Highest Risk Profile:
	Cessna leads in total accidents: 23,630 incidents (highest among all manufacturers)
	Fatality rate: 7,058 fatal injuries - significantly higher than other manufacturers
	Injury severity: 23,630 total injuries, with 12,909 serious injuries

2. Amateur Build Status, Engine Count, and Engine Type Are Critical Risk Factors: ·	Single engine (1)- Highest accident concentration ( Approximately 61,000 plus accidents based on the peak).
	Twin engine (2)- Significantly lower (Approximately 15,000 accidents). Multi-engine (3+)- Much lower accident rates (under 1,000 each). We can see a clear pattern- More engines = better safety profile.
	Amateur-built aircraft: Only 415 total accidents. Professionally-built aircraft: 45,325+ accidents. Key insight: Professional aircraft have 110x more accidents than amateur-built.
and upon selecting any type or number of engine you get to see the extent of damage to the aircraft.

3. Aircraft Purpose and Manufacturer Trends Reveal Operational Risk Patterns: Aerial Application - 4,228 accidents. Business flights - 3,513 accidents. All other purposes can be seen in the visual.
970s-1980s: Peak accident periods 700 plus accidents per year. Steady decline: Clear downward trend from 1980s onward	Modern era (2000s+): Significantly lower accident rates under 200 per year


### Recommendations

Based on the analysis, here are the recommended actions:
- Focus on Business-Configured Aircraft from Manufacturers with Consistent Safety Records like  Mooney. Avoid Cessna at all cost.
- The Triple Safety Filter: Avoid Single-Engine Reciprocating Aircraft, Consider Professional Multi-Engine Turbine Aircraft

- Consider manufacturers with lower incident rates (Boeing, Bell, Mooney show much better safety profiles)


### Next Steps

- Id have developed a metrix to be more specific on giving a recommendation and for other companies to use as a standard metrix.
- Number of flights per make or model, the cost of flight, 
- Given enough data losses incured can be calculated.

## Repository Structure

```
├── README.md                    <- This file
├── data/                        <- Data files and analysis
│   ├── aviation_dataset/        <- Original aviation data
│   ├── images/                  <- Visualizations and plots
│   ├── clean_data.csv          <- Final processed data
│   ├── cleaned_data.csv        <- Cleaned dataset
│   └── DSF-FT13 Hy-Phase-1-Project.ipynb  <- Jupyter notebook
└── notebooks/                   <- PDF Presentation
```

## Files in This Repository

### Key Visualizations

#### Aviation Risk Analysis Dashboard
Aviation Risk Analysis Dashboard- (images/aviation_dashboard.png)
*Comprehensive dashboard showing aviation safety trends, accident analysis by aircraft type, and key risk factors. This analysis provides stakeholders with actionable insights for improving aviation safety protocols.*
## Tools Used

- anaconda(Python 3.x)
- Pandas for data manipulation
- Numpy 
- Matplotlib/Seaborn for visualization
- Skitlearn
- Tableau 

Canvas Link(PDF): https://www.canva.com/design/DAGrpKLZRxw/fdxC91xCWOvBhKG2iWX79w/edit?utm_content=DAGrpKLZRxw&utm_campaign=designshare&utm_medium=link2&utm_source=sharebutton

Tableau Link: https://public.tableau.com/app/profile/rosemary.wanjiru/viz/AircraftSafetyOverview
Project Link: https://github.com/r0sh1ddy/Aviation-Risk-Analysis
