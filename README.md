# Objectives
This project analyzes MTA subway ridership and service data using API-driven datasets to uncover trends, delays, and incidents. The goal is to provide insights into how disruptions affect commuters and identify opportunities for service improvements.

# Data Source
https://new.mta.info/open-data

# Data Structure
## delay.csv: 
Containing detailed information regarding delays, including time, division, line, day_type (weekends/ weekdays), category (reasons for delays), subcategory (specific reasons), numbers of delays.
## ridership.csv:
Containing estimated riderships before and after pandemic from 3/2020 to 11/2022.
## incident_pre.csv:
Containing the number of delays before pandemic from 1/1/2015 - 9/1/2016.
## incident_post.csv:
Containing the number of delays after pandemic from 9/1/2022 - 10/1/2024.

# Data Cleaning
## Reformat "Date" columns 
### <img width="874" alt="Screenshot 2024-12-14 at 11 49 40 AM" src="https://github.com/user-attachments/assets/8228be67-3f38-48a4-a957-948857963af2" />
### <img width="893" alt="Screenshot 2024-12-14 at 11 50 27 AM" src="https://github.com/user-attachments/assets/98c482bd-566d-4e9a-ba0e-c83d6caf1ac6" />
### <img width="902" alt="Screenshot 2024-12-14 at 11 50 36 AM" src="https://github.com/user-attachments/assets/557afe1d-924e-4b6b-a905-bd93b3ef8023" />
### <img width="964" alt="Screenshot 2024-12-14 at 11 51 16 AM" src="https://github.com/user-attachments/assets/57cb6395-cc45-4a5a-b668-39ea30a5f06f" />

By reformatting date columns, tables can be standardized, making it easier to merge or join them in Tableau for more complex visualizations.

## Dropping Unnessary Columns
Removing irrelevant columns ensures the dataset is clean and contains only the essential information needed to support business metrics.

## Deleting NULL Values
This ensures the dataset contains only valid entries, enhancing the accuracy of the analyses.

## Adding the Total Pre-pandemic Ridership Column
This calculated column provides an overall view of ridership trends.

## Standarizing Reporting Categories 
This helps keep the record consistent and accurate throughout the analysis process.

# Data Analysis & Visualizations
## Reason for Delays
### <img width="576" alt="Screenshot 2024-12-14 at 12 06 21 PM" src="https://github.com/user-attachments/assets/433dfc01-b9bf-4f5b-a0cb-cae976e6f7a5" />

## Common Major Incidents Between Pre and Post-Pandemic
### <img width="528" alt="Screenshot 2024-12-14 at 12 06 28 PM" src="https://github.com/user-attachments/assets/3b788854-6cf3-4b93-b5e0-a6ffb2baf7ef" />

## Comparison between Weekdays and Weekends
### <img width="573" alt="Screenshot 2024-12-14 at 12 06 36 PM" src="https://github.com/user-attachments/assets/7753521d-e3e8-42da-a7e5-bf12642b9107" />

## Comparison in Divisions and Lines
### <img width="584" alt="Screenshot 2024-12-14 at 12 06 43 PM" src="https://github.com/user-attachments/assets/5c2668f6-f3c9-4283-86de-09ff00f2569d" />

## Monthly Analysis
### <img width="615" alt="Screenshot 2024-12-14 at 12 06 51 PM" src="https://github.com/user-attachments/assets/d9360275-2d53-4ee1-8cfe-12255882c9ca" />

# Insights and Recommendations
## Insights
### B Division experiences more delays than A Division.
### Delays due to signals and track issues have been declined after the pandemic but still remained significantly.
### The highest contributor for delays shifted to Persons on Trackbed/ Police/ Medical.
### Line N, 6, and 2 face persistent delays due to infratructure strain. (Line 6: high delays due to passenger behavior and crime incidents + Line N, 2: heavily impacted by operational inefficients).
### Seasonal Trend:
#### Pre-Pandemic: peaks occurred in summer and reached low in November and December.
#### Post-Pandemic: peaks moved to September and October -> trends became less predictable.
## Recommendations
### Evaluate schedules and capacity planning for B Division.
### Prioritize investments in modernizing train infrastructure + implement IoT sensors to predict maintenance beforehand.
### Conduct maintenance in low traffic months.
### Address crimes with more security camera and workforce on line 6. 

# References
### https://www.who.int/news/item/02-03-2022-covid-19-pandemic-triggers-25-increase-in-prevalence-of-anxiety-and-depression-worldwide
### https://www.thecity.nyc/2020/11/22/subway-people-on-tracks-rising-new-york-city/
### https://www.bloomberg.com/news/articles/2023-10-04/mta-details-plan-to-fix-aging-system-fight-storms-through-2044
### https://nypost.com/2021/07/14/nyc-morning-rush-still-plagued-by-mtas-archaic-faulty-signal-system/
### https://www.amny.com/nyc-transit/mta-upgrades-disrepair-cbc-report/?utm_source=chatgpt.com
### https://www.nbcnewyork.com/news/local/new-details-emerge-on-nyc-subway-safety-plan-these-6-lines-will-be-targeted-first/3566126/



