# Risk Assessment: Analysis for best Aicraft Acquisition.
![image alt](https://github.com/user-attachments/assets/fc908a47-0645-47b0-a479-97a3ca0fba72)
## Introduction
For this analysis, we will use the dataset  **"Aviation Accident Database & Synopses, up to 2023"** from Kaggle, provided by the National Transportation Safety Board (NTSB). This dataset contains comprehensive information about aviation incidents.

Our goal is to analyze accident patterns, aircraft reliability, evolution of accident frequency in aviation incidents. We will generate data-driven insights that will help the new aviation division in identifying the safest aircrafts for purchase and determining the best strategies for fleet management.

## Dataset overview
- Aircraft Makes and Models: Information about the specific make and model of the aircraft involved in each incident.
- Event date : the specific date each incident happened.
- location : The location where the aviation accident took place.
- injury severity: the Gravity and the amount of injuries.
- Aircraft Damage : the state of Aircrafts after accident.
- weather conditions

the dataset also contains other information, that are less relevant to the analysis.
##### N.B: the dataset is not up to date. Any analysis conducted will only be representative of the approximate year range from 1982 to 2023.
## Exploratory Data Analysis (EDA)
Exploratory Data Analysis (EDA) is the foundation for data-driven decision-making. It involves examining, cleaning, and visualizing data to uncover patterns, trends, and insights.

For the purpose of this analysis we will take the following steps:
- Data cleaning
- Data Understanding
- Data Analysis
- Recommendations
- Summary

### **Data Cleaning: Ensuring Accurate and Reliable Analysis**  
In this section, we focus on refining the dataset to maintain precision and consistency:  
- **DataFrame Duplication** – Creating a structured copy for controlled modifications.All modifications will be done in the copy not in the original DataFrame.  
- **Column Filtering** – Removing irrelevant fields to streamline analysis.  
- **Data Type Optimization** – ensures consistency in how information is stored, improving efficiency in processing and analysis. By standardizing data formats, we reduce errors and streamline operations, making insights more reliable.
- **Handling Missing Values** – Filling incomplete records to preserve dataset integrity.  

These steps ensure a **clean, well-structured dataset**, allowing for accurate aviation risk assessment and meaningful insights.
## Data Understanding:
This section ensures that the data is properly structured and prepared for analysis, laying a solid foundation for meaningful insights. It sets the framework for the upcoming exploration.
Below are key questions that the new aviation division may seek to answer. They will be addressed in the notebook.
- Which aircraft makes have suffered the fewest and the most accidents?
- How has accident frequency evolved over the years for the country with the highest number of accidents?
- For which flight purposes have accidents been most frequent?
- For which flight phases have accidents been most frequent?
- For which Weather conditions have accidents been most frequent?
- How resistant are certain aircraft to accidents for Top Manufacturers ?
- How well are passengers protected in the event of an aircraft crash For top Aircraft Manufacturers?

## Data Analysis
In this section, we apply data-driven methodologies to support informed business decisions:  
- **Data Visualization** – Clear graphical representations to highlight key trends.  
- **Correlational Analysis** – Identifying relationships between critical aviation factors.  
- **Pattern Recognition** – Detecting recurring themes to enhance risk mitigation strategies.  
- **Trend Identification** – Assessing historical data to forecast future outcomes.  
- **Actionable Insights** – Extracting meaningful findings to optimize operational efficiency.  
- **Risk Assessment** – Evaluating aviation safety metrics to minimize potential liabilities.  
### Which aircraft makes have suffered the fewest and the most accidents?
To address this question a bar chart of the top 5 Aircraft Makes that have suffered the most accidents and the 5 that have suffered the fewest will be provided.
![image alt](https://github.com/Haender-Michael/Phase-1-Project/blob/63e87f67892f84f2a77bcebb9b12aadfa7f5ab19/images/image1.png)
#### Analysis :
Now, we might mistakenly believe that the least recurrent aircraft are the safest, but that's not necessarily true. The fact that these aircraft have fewer recorded accidents could simply mean that they have operated fewer flights, reducing their chances of incidents rather than proving their reliability.

For example, if the aircraft make Cessna has the most accidents, it might simply indicate that it has operated the most flights. However, when analyzing accident rates, it could actually be among the most reliable aircraft in terms of avoiding accidents.
### How has accident frequency evolved over the years for the country with the highest number of accidents?
The new aviation division would want this information to :
- Evaluate safety trends --> Assess whether accident rates have decreased due to improved regulations and technology.

- Improve fleet management --> Make informed decisions about aircraft acquisition based on reliability across regions.

- Support policy decisions --> Use data-driven insights to enhance aviation safety measures and operational guidelines.

- Identify high-risk regions 
#### The top 4 countries with the most aviation accidents will be represented in the plot below.
![image alt](https://github.com/Haender-Michael/Phase-1-Project/blob/7ce2a5f003b24d7c300af9d93cf7fc301e4dea5a/images/image2.png)
### Analysis:
The head of the new aviation division may need to reconsider or conduct further research before initiating airplane operations in countries such as Canada and Brazil due to the increase in aviation accident frequency observed between 2020 and 2022.

However, since the dataset is not up to date,it's not safe to assume that it is still the case for years after 2022.


Additional analysis should be done, as significant changes in aviation trends may occur in the years after 2022.
![image alt](https://github.com/Haender-Michael/Phase-1-Project/blob/716c41e68c071d4c26e72214e3741ec74fe0e1bf/images/image3.png)

Only by comparing accident rates  instead of frequency can we determine which aircraft make could be considered the most reliable.
###For which flight purposes have accidents been most frequent?
#### Analysis:
N.B: This graph does not show which purpose of flight is most likely to cause an accident. It only presents accident frequency by purpose, not accident rates.

For example, personal flights may have the highest accident count simply because they account for more aircraft operations overall.

The frequency of Aircraft accident for personal purpose of flight may prompt the head of the new aviation division to take specific measures of safety regarding the personal or other very recurrent flight purposes, but it should not be assumed that higher frequency directly correlates with a higher accident rate.
### For which flight phases have accidents been most frequent?
![image alt](https://github.com/Haender-Michael/Phase-1-Project/blob/347e465630da0f06d9dd6c47ad1fcfe455520fd2/images/image4.png)
Result: there has been the most accident during the landing phase.
### For which weather condition have accidents been most frequent?
![image alt](https://github.com/Haender-Michael/Phase-1-Project/blob/626dff4e3dcbecb4af65eee2ea88233d3cc6311e/images/image5.png)

Visual Meteorological Conditions(*VMC*):Weather conditions that allow pilots to fly using visual references rather than relying on instruments.
Instrument Meteorological Conditions(*IMC):This usually indicates that the weather condition was not recorded or is uncertain in aviation reports.

Analysis: 
Most accidents happen during favorable weather conditions.
Regardless, Measures should be taken to avoid accidents that are related to bad weather condition as they account for around 8 percent.
### How resistant are certain aircrafts to accidents for Top Manufacrtures ?

Top Aircraft Manufacturers:

With a market valuation of over \$114.97 billion as of 2024, Airbus dominates the aircraft manufacturing industry, closely followed by Boeing at \$113.82 billion. Other notable players include Lockheed Martin (\$110.98 billion), Hindustan Aeronautics (\$42.80 billion), Textron (\$16.35 billion), Dassault Aviation (\$14.18 billion), Bombardier (\$6.26 billion), Embraer (\$4.82 billion), Joby Aviation (\$3.51 billion), and Korea Aerospace Industries (\$3.45 billion). These organizations produce both military and commercial aircraft and provide necessary services, including component manufacturing, maintenance, and repairs. (source:https://straitsresearch.com/statistic/largest-aircraft-manufacturers-globally)


> ### Why are we using the top aircraft manufacturers for this analysis?

 >The top aircraft manufacturers are highly recognized and trusted in the aviation industry. Their market valuation serves as proof of their reliability and effectiveness. For instance, Airbus and Boeing are widely regarded as industry leaders in safety and innovation.

![image alt](https://github.com/Haender-Michael/Phase-1-Project/blob/2926a6da1d279872da0597eb30535779f8466650/images/image6.png)
### How well are passengers protected in the event of an aircraft crash For top Aircraft Manufacturers?
![image](https://github.com/Haender-Michael/Phase-1-Project/blob/d0562f935c431ed6e5351691ec2a245dadc86ad0/images/image7.png)
#### Result:
airbus a330-243 and boeing 737-800 have the lowest amount of injuries.
## 
Summary

> For this analysis, we used a dataset from Kaggle: **"Aviation Accident Database & Synopses, up to 2023."**  
After cleaning, we aimed to address key questions that the head of the aviation division is likely to have.  
> For each analysis, we found the following information:  
> - The aircraft that has sustained the fewest accidents is not necessarily the safest.  
> - Accident frequency increased from 2020 to 2022 in both Brazil and Canada.  
> - there have been far more accidents for personal flight purposes than for the others, but we shouldn't assume that this correlates directly with accident rates. Instead, the head of the aviation division should implement specific safety measures to ensure smooth operations for these flights.
> - There have been far more accidents for landing than the other phase of flight.
> - Most accident happen during favorable weather conditions. Regardless, Measures should be taken to avoid accidents that are related to bad weather condition as they account for around 8 percent.
> - Airbus a330-243 and boeing 737-800 have the lowest destroyed rate.
> -  Airbus a330-243 and boeing 737-800 also the lowest amount of injuries, making them among the safest among the top aircrafts.
## Recommendations 

The head of the new aviation division may need to reconsider or conduct further research before initiating airplane operations in countries such as Canada and Brazil due to the increase in aviation accident frequency observed between 2020 and 2022.

The frequency of Aircraft accident for personal purpose of flight may prompt the head of the new aviation division to take specific measures of safety regarding the personal or other very recurrent flight purposes in the Aviation accident dataset, but it should not be assumed that higher frequency directly correlates with a higher accident rate.

Our DataFrame account most accidents for landing. Specific Measures towards assuring proper landing will have to be taken by the head of the new aviation division. Also the head of the new aviation division should take approximate amount of measures for other most recurrent phase of flight in the Aiation accident dataset.

Most accidents happen during favorable weather conditions. Regardless, the head of aviation division will need to take Measures to avoid accidents that are related to bad weather conditions as they account for around 8 percent.

Finally Airbus a330-243 and boeing 737-800 are strongly recommended as they are from top manufacturerers. Additionally, among the Aircraft made by top manufacturers, they  have the lowest destroyed rate,and the lowest amount of injuries, making them  very reliable Aircrafts.

NB :The dataset is not up to date. Analysis of recent years is recommended. For this purpose and more, contact information of the Analyst who worked on this porject is provided.
### Interactive dashbord 
An interactive dashboard is a decision-making tool that provides stakeholders with clear, actionable insights through dynamic visualizations. It allows  users to filter, explore, and compare key metrics, the dashboard simplifies complex data into an accessible format, enabling informed strategic discussions. 
link to this project dashbord: 
#  **
## Contact Information
- First Name: Haender Michael

- Last Name: Jean Louis

- Email: michaelhaenderjeanlouis@gmail.com

- Phone Number: +509 41 75 0264

- LinkedIn: https://www.linkedin.com/in/michael-haender-jean-louis-4b7320316?utm_source=share&utm_campaign=share_via&utm_content=profile&utm_medium=ios_app

For further inquiries, feedback, or collaboration on this analysis, feel free to reach out. I welcome discussions and any contract to work with the head of the new Aviation division



