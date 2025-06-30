# Aircraft Risk Assessment

This is a data analysis of aviation accident data to evaluate the safety of different aircraft types, engine types, engine count and

make to guide the company in making investment decisions as it seeks to expand into the aviation industry.


## Overview

The aviation industry is a high risk sector where safety and risk mitigation are critical. There is need to understand which factors

contribute most to fatal accidents essential for making informed decisions as the company seeks to expand into the aviation industry.

The analysis of aviation accident data aims to uncover patterns in aircraft related fatalities and injuries. By exploring the

relationships between aircraft characteristics such as engine type, number of engines, manufacturer, damage level and the severity of

accidents, the analysis provides insights that can help a company:

1.Avoid investing in high risk aircraft.

2.Recognize which engine types and count are safer.

3.Understand the distribution of injuries across aircraft types.

An interactive Tableau dashboard shows the insights. This is after thorough  data cleaning and exploratory analysis. Final deliverables

include presentation slides, a Jupyter notebook and a GitHub repository.



## Business Understanding

The company is exploring the possibility of diversifying its business operations into the aviation industry. Due to the high risks

associated with aviation there is the need  to understand the factors that influence aircraft safety and operational risk.

The company wants to answer critical safety questions using data driven insights by leveraging historical accident data to assess how

different aircraft types, engine types and Make relate to the severity of accidents.

###  Goals

1. Minimize risk by avoiding historically dangerous aircraft.

2. Identify safer aircraft types and manufacturers.

3. Use data insights to influence investment decisions.

###  Business Questions

1. Which aircraft makes  are most frequently involved in fatal accidents?

2. Does the number of engines or engine type affect accident severity?

3. How does the level of aircraft damage relate to injury and fatality outcomes?

4. Are amateur-built aircraft riskier than those built by certified manufacturers?



## Data Understanding and Analysis

This aviation accident data is sourced from the Federal Aviation Administration. It has aviation incidents and accidents reported in the United States. 

### Key Features in the Dataset

| Column Name            | Description                                                                 |
|------------------------|-----------------------------------------------------------------------------|
| `Make`                 | Manufacturer of the aircraft (e.g., Cessna, Piper, Beech)                   |
| `Model`                | Model of the aircraft                                                       |
| `Engine.Type`          | Type of engine (e.g., Reciprocating, Turbo Fan, Turbo Prop)                |
| `Number.of.Engines`    | Number of engines on the aircraft                                           |
| `Amateur.Built`        | Indicates whether the aircraft was amateur-built or certified               |
| `Aircraft.Damage`      | Type of damage sustained (Minor, Substantial, Destroyed)                    |
| `Injury.Severity`      | Overall injury outcome of the incident                                      |
| `Total.Fatal.Injuries` | Number of people who died in the accident                                   |
| `Total.Uninjured`      | Number of people involved who were uninjured                                |

###  Data Cleaning

The cleaning steps included:

1. Handling null  values in columns.

2. Correcting inconsistenticies such as different spellings of `UNK`, or `Unknown`.

3. Dropping irrelevant columns.


Exploratory Data Analysis was performed using Matplotlib and Seaborn.

Tableau was used for visualizations.

## Visualizations

The Tableau dashboard includes the following visualizations to support data driven decision making:

1. Fatalities by Engine:  
   Highlights which engine types are most associated with fatalities.

2. Fatalities by Aircraft Damage:  
   Shows how damage levels like “Destroyed” or “Substantial” correlate with fatal injuries.

3. Fatalities by Top 10 Aircraft Makes:  
   Identifies the manufacturers most commonly involved in fatal incidents.

 All visuals use bar plots for simplicity and interpretability. The link to the visualizations https://public.tableau.com/views/Phase1_Dashboard/Dashboard1?:language=en-GB&publish=yes&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link



##  Conclusion

The analysis revealed patterns in how aircraft characteristics relate to injury severity and fatality outcomes. 

### Key Insights:

1. Engine Count and Type Matter: 
   Aircraft with reciprocating engines and single engines are most frequently associated with fatal accidents.

2. Aircraft Damage Level has a strong correlation with Injury Severity: 
   Most accidents resulting in fatalities have "Destroyed" aircrafts.

3. Clearly seen manufacturing patterns:  
   Cessna, Piper and Beech make up the majority of fatal cases due to their market dominance.

4. Amateur Built Aircraft have higher associated risks:  
   Fewer in number but have a higher fatality rate per incident.

### Recommendations

1. Avoid engines with high risks such as reciprocating and single-engine aircraft.

2. Prioritize aircraft with lower fatalities and injuries based on make and engine type. 

3. Choose aircraft with high survivability rating in past crash reports.
