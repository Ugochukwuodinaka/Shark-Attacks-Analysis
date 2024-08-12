# Shark Attacks Analysis (1900-2017)
![](images/Sharks_Attacks_image.jpg)
<br />

## Table of Contents
- [Project Overview](#project-overview)
- [Dataset Overview](#dataset-overview)
- [Tools Used](#tools-used)
- [Visualization in Power BI](#visualization-in-power-bi)
- [Project Analysis](#project-analysis)
- [Visuals in Power BI Report](#visuals-in-power-bi-report)
- [Recommendations On Mitigating Shark Attack Risks](#recommendations-on-mitigating-shark-attack-risks)
<br />

## Project Overview

### Introduction:
The __Shark Attacks Analysis (1900-2017)__ project aims to investigate and analyze global shark attack data to gain insights into the patterns, trends, and factors associated with shark attacks. Through the examining of this data, geographical locations, species involved, environmental conditions, and human activities, the project seeks to provide an understanding of shark attacks, their frequency, and potential risk factors. Sharks Atacks Analysis contains Shark attacks reported over the past 100 years, including location, activity, victim info (name, gender, age), shark species, etc. The project aims to explore and analyze sharks attacks all around the world.


### Objectives:
### Introduction:
The __Shark Attacks Analysis (1900-2017)__ project aims to investigate and analyze global shark attack data to gain insights into the patterns, trends, and factors associated with shark attacks. Through the examining of this data, geographical locations, species involved, environmental conditions, and human activities, the project seeks to provide an understanding of shark attacks, their frequency, and potential risk factors. Sharks Atacks Analysis contains Shark attacks reported over the past 100 years, including location, activity, victim info (name, gender, age), shark species, etc. The project aims to explore and analyze sharks attacks all around the world.


### Objectives:
- Analyze the data on shark attacks annually since 1900, and identify trends and patterns in shark attack occurrences over time.
- Identify the countries with the highest reported incidences of shark attacks and determine the specific areas and locations within those countries that exhibit higher levels of risk, providing insights into geographic hotspots for shark-human interactions.
- Practice data cleaning skills by preparing the raw dataset for analysis, ensuring consistency, accuracy, and suitability for further investigation.
- Perform text analysis on the "Injury" column to determine the body parts most frequently injured in shark attacks, providing valuable insights into the severity and nature of shark-related injuries.
- Transform the "Time" data to analyze the timing of shark attacks and ascertain whether certain parts of the day are associated with increased occurrence of shark-human interactions.
- Clean and analyze the data related to shark species involved in attacks to identify the species most frequently implicated in shark attacks, despite potential data inconsistencies and inaccuracies.


### Expected Outcomes:
- A comprehensive visualization illustrating the trends and patterns of shark attacks annually since 1900, facilitating a deeper understanding of the temporal evolution of shark-human interactions.
- Identification of countries with the highest incidence rates of shark attacks and pinpointing specific regions within these countries where shark encounters are most prevalent, aiding in the development of targeted safety measures and risk mitigation strategies.
- Cleaned and prepared dataset ready for analysis, ensuring reliable and accurate insights into various aspects of shark attacks.
- Insights into the body parts most commonly injured in shark attacks, informing medical and safety protocols for individuals at risk of shark encounters.
- Determination of whether certain times of day are associated with higher rates of shark attacks, potentially informing beach safety guidelines and public awareness campaigns.
- Identification of the shark species most frequently involved in attacks, despite data cleaning challenges, contributing to our understanding of species-specific behaviors and informing conservation efforts and management strategies aimed at reducing human-shark conflicts.
<br />
<br />

### Dataset Overview
The dataset used in this analysis is the "Attacks.csv" and was provided by [Quantum Analytics](https://www.quantumanalyticsco.org/). The "Attacks.csv" dataset contains information on shark attacks documented over some time. The dataset provides insights into various aspects of shark-human interactions, including the location, date, time, severity of injuries, shark species involved, and other relevant details about each recorded shark attack incident. You can access the dataset [here](attacks.csv).

This dataset has a single data table with 16 columns and 6,091 rows of data. Below is a description of the columns in this dataset for a better understanding of this analysis:
| Table                              | Field                    | Description                            |            
|:-----------------------------------|:------------------------ |:-------------------------------------- |
|attacks.csv                         | Case Number              | A unique identifier for each shark attack incident.   |
|                                    | Date                     | The date when the shark attack occurred.     |
|                                    | Year                     | The year in which the shark attack took place.        |
|                                    | Type                     | Describes the type of attack (e.g., provoked, unprovoked, invalid, etc.).       |
|                                    | Country                  | The country where the shark attack occurred.        |
|                                    | Area                     | The specific area or region within the country where the shark attack occurred.        |
|                                    | Location                 | Provides details about the location of the shark attack (e.g., beach name, geographical coordinates, etc.).      |
|                                    | Activity                 | Describes the activity being performed by the victim at the time of the shark attack.       |
|                                    | Name                     | Name of the individual involved in the shark attack incident.         |
|                                    | Sex                      | Gender of the individual involved in the shark attack.         |
|                                    | Age                      | Age of the individual involved in the shark attack.      |
|                                    | Injury                   | Specifies the type and severity of injuries sustained during the shark attack.        |
|                                    | Fatal (Y/N)              | Indicates whether the shark attack resulted in a fatality (Y for yes, N for no).       |
|                                    | Time                     | The time of day when the shark attack occurred.    |
|                                    | Species                  | Specifies the shark species involved in the attack, if known.        |
|                                    | Investigator or Source   | Provides information about the source of the data or the investigator who documented the shark attack incident.     |
<br />

### Skills Utilized
1. Data Cleaning
2. Data Visualiziation
3. Descriptive Analytics
4. Critical Thinking and Problem Solving
5. Communication and Reporting
<br />

### Tools Used
1. Power Query Editor
    - Was used to:
        1. Clean
        2. Transform the dataset for this analysis.
           
2. Power BI (Was used to create reports and dashboard for this analysis)
    - The following Power BI Features were incorporated:
        1. DAX
        2. Quick Measures
        3. Page Navigation
        4. Filters
        5. Tooltips
        6. Button
<br />

### Data Cleaning, Transformation and Loading using the Excel and Power Query Editor:
1. Removed a few data rows with outdated, irregular, unreadable, duplicate, empty, or wrong information in the __"Case Number"__ column and other columns from the table.
2. Created and added a new column - __"Age_Band"__ using the "If Statement" in the power query editor to display the age range of shark attack victims.
3. Created and added a new column - __"Time_Period"__ using the "If Statement" in the power query editor to display the period (morning - night) that shark attacks on victims happened.
4. Corrected the __"Time"__ column using the right time data format and corrected all column rows.
5. Used __"N/A"__ to fill-up the __"Sex"__ column rows without information.
6. Used __"N/A"__ to fill-up the __"Fatal (Y/N)"__ column rows without information.
7. Used __"Unknown"__ to fill-up the __"Age Band"__ column rows without information.
8. Re-ordered the columns in the table properly in the Power Query Editor.
9. Made sure that all the table columns returned __"100%"__ valid using the column quality feature of the Power Query Editor. 
10. The total number of data rows before data cleaning was __"6,091"__ rows and was reduced to __"5,940"__ rows after cleaning.
<br />

**Raw Data**
- Below a screenshot of a part of the raw data in .csv file format. You can access the dataset [here](attacks.csv).

![](images/Raw_File_Screenshot.png)
<br />

**Final Power Query Editor screenshot**
- Below is a screenshot of a part of the cleaned data in power query editor:
![](images/Power_Query_File_Screenshot.png)
<br />
<br />

## Data Modelling
No data modeling was required since a single table was utilized in this analysis.
<br />
<br />

## Visualization in Power BI:
#### Report View 1
![](images/Shark_Attacks_Analysis_Dashboard1.jpg)

#### Report View 2
![](images/Shark_Attacks_Analysis_Dashboard2.jpg)
<br />
<br />

### Project Analysis:
From the analysis, i made the below Key findings:
- The Total Number of Shark Attack Cases is __5,956.__
- The Total Number of Survivors are __4,341.__
- The Total Number of Fatalities are __1,515.__
<br />
<br />

- <img src="images/Top10_Cases_By_Activity.jpg" width="300">

- **Casualty Cases By Activity:**
My analysis of the top 10 shark attack cases by activity provides insightful views into the activities that correspond to shark-human interaction. Here are some key observations and insights:
- __Surfing Tops:__ Surfing tops the list of activities with the highest number of shark attacks, at 934 incidents. This can be understood by the fact that surfers on the surfboards appear to sharks as prey due to their silhouette and motion, for sharks are known to mistake from below the profile of surfers for resembling potential prey species.
- __Swimming Vulnerability:__ There are recorded 861 cases of shark attack for swimming. Swimmers normally stay in the water for a longer period, which may increase their likelihood of encountering sharks. Shark attraction can also be facilitated by the splashing and disturbing in the water by swimmers.
- __Fishing and Spear Fishing mph__. With fishing, cases of shark attacks in the activities of fishing and spearfishing are astronomically high, at 419 and 328, respectively. Bait and blood chumming form a significant part of activities associated with these two foregoing activities. Chumming tends to attract sharks to an area, considerably improving the chances of encounters.
Other activities such as bathing, wading, and standing have also been involved in shark attack cases, although to much smaller degrees compared with surfing and swimming. Whereas these two activities may be considered a bit more passive compared to active activities like surfing and swimming, it still shows that people engaged in these activities are not exempt from shark encounters due to the nature of their behavior.
- __Diving and Snorkeling:__ Shark attacks in diving and snorkeling have been much fewer compared to other activities because it is simply underwater sightseeing. However, the activity still has a degree of risk associated with locations that are known to have sharks or feeding behaviors of these creatures.
- We have several rows of data in our results where case activity was not provided. We have classified this activity as "Not Provided" - 511 cases. These cases demonstrate a possible underestimate of the risks associated with water-based activities and underline the need for improved completeness in reporting.
<br />
<br />

- <img src="images/No_of_Cases_By_Time_of_Day.jpg" width="300">

- **Number of Cases By Time of Day:**
The Time-of-day analysis for the cases of shark attacks gives insights into how the attacks are distributed across the different periods of the day. Some key observations and insights are as follows:
- __Unprovided Cases Prevalence:__ A total of 3,146 instances fall under the category of unprovided cases, which is far higher in all categories of time. It thus means that a good percentage of the dataset has no information on the exact time of day when shark attacks occurred. Such prevalence of the unprovided cases reiterates that complete and accurate data collection is extremely critical when doing elaborate analysis and trying to understand temporal patterns associated with shark attacks.
- __Afternoon Activity__: Afternoon is the second most frequent period, accounting for 1,101 cases of shark attacks. Afternoons usually form the peak times for recreation at the beach or coastal areas, entailing swimming, surfing, and diving, and hence invite more human presence in the water to interact with sharks.
- __Morning and Evening Incidents:__ Other important cases of shark attacks are during morning and evening hours, Cook:942 and 606 respectively. These hours may prove to be times when people go out in the water though not as much as during the afternoon. Factors such as changing environmental conditions, prey, and human behavior could impact shark activity and interactions with humans at these times of the day.
- __Nighttime Vulnerability__: According to the dataset, there have been 161 cases of shark attacks at night. Generally, activities on the coast are lesser compared with daylight hours because of reduced visibility and safety concerns; fewer shark-human interaction opportunities are present. However, for those who engage in night fishing or other activities at such hours, there can still be chances of encountering sharks.
<br />
<br />

- <img src="images/No_of_Cases_By_Sex.jpg" width="300">

- **Number of Cases By Sex:**
The data regarding the cases of shark attacks by sex provides a look at the mix of the genders of the individuals involved in the attacks. The key observations and insights are marked below.
- __Male Majority:__ The data set shows that males have a high incidence rate in shark attacks, with 4,820 recorded incidences. This will clearly prove that males engage in activities or situations predisposed to higher potential exposure with sharks, for example, surfing, swimming, and diving, which have generally been the traditional male recreational activities along coastal areas.
- __Female Representation:__ Significantly fewer cases are, at 591, where females have been attacked. This might be a function of different participation rates between the sexes in activities, with females participating in water-based activities less frequently or under different circumstances than men. Other socioeconomic factors or cultural expectations, too, could lead to sex-based differences in behaviors and risk abandonment in aquatic activities.
- __No Sex Information Given:__ Much of the data includes cases where no information was given regarding the sex of the side concerned, and this counts up to 537, labeled N/A. This means that there was no information provided about the sex of the side concerned., therefore, gives room for better ways of data collection to ensure the information reported and data analyzed concerning shark attacks is accurate.
<br />
<br />

- <img src="images/Number_of_Cases_By_Survivors_vs_Fatalities.jpg" width="300">

- **Number of Cases By Survivors or Fatalities:**
Analysis of this data will give the manifestations of the results of shark attacks about the number that survived compared to those who succumbed to various injuries. Listed below are observations and insights derived from the information provided:
- __Survival Rate:__ Most of the general cases of shark attacks have survived the trauma, with cases amounting to 4,341 recorded as survivors. This is approximately 72.93 percent of all reported cases, indicating most shark encounters end in non-fatal outcomes.
- __Fatalities:__ While it has a relatively high survival rate, a large number of the cases of shark attacks ended in fatalities. There are 1,515 reported death cases. Fatalities account for approximately 25.45% of all reported cases of shark attacks, so it means they can be very serious and fatal.
- __Unknown Outcomes:__ Ninety-six cases of shark attacks exist where the main outcome regarding survivor or fatality is unknown, which makes for about 1.61 percent of the cases. That there is no information available about the result in these few instances obviously drives home the need for a better system of data collection and reporting to ensure that incidents of shark attacks are suitably assessed and analyzed.
<br />
<br />

- <img src="images/Top10_Countries_With_Most_No_of__Cases_By_Casualties_%26_Fatalities.jpg" width="250">

- **Top 10 Countries With Most Number of Cases By Survivors and Fatalities:**
The analysis below describes the top-10 countries by number of cases of shark attacks, delineated between survivors and fatalities. The main observations and insights are hereby presented:
- __United States of America Tops:__ The USA has been reported to have the most incidents of shark attacks, totaling 2,140 cases. Of the total cases, nearly all people who were involved in shark attacks within the USA survived, amounting to 1,868. However, some of the incidents still caused death, with a recorded 248. Coastal areas in the USA, more so in Florida, California, and Hawaii, had a medium volume of shark activities that always attracted many tourists and locals involved in various water activities.
- __Australia and South Africa:__ Next in line to the USA in terms of shark attack cases are Australia and South Africa. In Australia, there are 1,287 cases, with a disproportionately high number of fatalities, 334, vis-a-vis survivors, at 928. In South Africa, 560 cases were reported with 425 survivors and 130 fatalities. These countries are known for their huge marine biodiversity and are destinations for a great number of water sports, thus increasing the level of contact between sharks and humans.
- __Varied Survivor-Fatality Ratios:__ Varied survivor-fatality ratios are also found, evidenced by data from different countries. For example, Papua New Guinea had 129 cases, of which 73 survivors were recorded against 54 fatalities, a quite high fatality rate in comparison to other countries. In contrast to this are countries that had a lower fatality record, such as the Bahamas and New Zealand, where more survivors are recorded compared to fatalities.
- __Factors Influencing Survivorship:__ Several factors would lead to a difference in survivorship rates, including prompt medical attention, availability of emergency services, and public awareness about the risks of shark attacks. These may explain the higher survivorship rates in countries with a well-developed emergency reaction system and public safety campaigns, like the USA or Australia.
<br />
<br />

- <img src="images/Shark_Attacks_Trend_By_Year_Since_1900.jpg" width="450">

- **Shark Attack Trend By Year Since 1900:**
In this analysis, I made a revelation of the time course evolution of shark-human interactions and results. The key observations and insights for this analysis are as follows:
- __General Trend:__ The total number of shark attack cases reported has been variable over the years, while different trends seem to prevail in shorter stretches. There is no net linear trend; however, periods of increase and decrease in number related to reported shark attacks can be realized from the data, suggesting temporal variability in shark activity and human exposure to shark encounters.
- __Fatalities and Survivors:__ However, information must also brings out is regarding fatalities; that is, deaths and survivors from shark attacks. The number of fatalities ranges from year to year, as some years have many fatalities compared to others. So, too, variation takes place regarding the number of survivors over time, showing differences in the severity of shark attacks, the effectiveness of emergency response measures, and people's resilience in surmounting injuries from shark attacks.
- __Peaks and Troughs:__ Certain years stick out as notable peaks or troughs in shark attack activity. For example, the early 1900s showed rather low numbers of reported shark attacks, with a fairly higher increase in the early 1920s. Peaks of shark attack activity are again observed in the late 1930s, the early 1940s, the late 1950s, and the late 1990s. Such fluctuations may be caused by various drivers, including changing environmental conditions, growing human population and coastal development, shifting shark populations, and improved data collection and reporting practices.
- __Recent Trends:__ A general increase in the number of reported shark attacks can be shown in the data for the more recent years, with peaks occurring at the beginning of the 2000s and mid-2010s. Although part of the increase can be attributed to improved data collection and reporting, shifts in human behavior, coastal recreational activities, and environmental factors possibly play important roles in shaping the recent trends of shark attack activity.
<br />
<br />

- <img src="images/Number_of_Cases_By_Age_Band.jpg" width="250">

- **Number of Cases By Age Band:**
The findings of this analysis provide insight into the demographic distribution of shark-human interactions and the risk factors associated with different age groups. Key insights and observations:
- __Adult Predominance:__ The list of shark attack cases is topped by adults, totaling 2,360, which accounts for almost 70.53 percent of the total cases. Again, this would be perfectly explainable as adults are more likely to take up sports like surfing, swimming, and diving, which would put them at greater risk of becoming victims of shark attacks. The high percentage rate of adult victims shows clearly the need for a focus on and campaign of beach safety measures and public awareness campaigns targeting this demographic group.
- __Vulnerability of Teenagers:__ 701 cases of shark attacks on teenagers have been reported, which is nearly 20.95 percent of the total cases. Since adolescence is the time for thrill-seeking behavior, they might get involved in some kind of risk-taking activity or get involved in water-based activities without knowing the risks involved in it, hence making themselves vulnerable to shark attacks. Making teenagers aware of the risks of shark attacks and responsible behavior, with education on safety measures, will help in reducing their vulnerability to shark attacks.
- __Children and Elderly:__ While children and the elderly, compared with adults and teenagers, have fewer cases of shark attacks, they still comprise a reasonable percentage of the victims. There are 203 cases regarding children, which forms 6.07% of the total cases while that regarding the elderly is 82, making up 2.45% of the total cases. Children are smaller and, therefore, more easily mistaken for their preferred food; furthermore, they are unable to distinguish potential dangers in aquatic environments. On the other hand, elderly people have reduced mobility or sensory capabilities, which places them at a disadvantage concerning the ability to evade shark encounters. Setting up some safety rules and systems of supervision according to age categories will help to reduce some of the risks for these groups.
- __Unknown Age Category:__ As many as 2,609 cases of shark attacks are labeled "Unknown", which thereby reduces any age information available for such incidents. This lack of age information portrays the requirement for improved data collection and handling practices for the correct assessment and analysis of the incidents of shark attacks.
<br />
<br />

- <img src="images/Top10_Locations_By_No_of_Cases.jpg" width="300">

- **Top 10 Location By Number of Cases:**
Valuable insights provided in the analysis were concerning the geographic distribution and prevalence of shark-human interactions across different coastal areas. The following are the key observations and trends in the analysis:
- __New Smyrna Beach:__ New Smyrna Beach, Volusia County, Florida, is in the foreground as the leading area concerning shark attacks, having had the most reported incidents at 163. So, what may cause this site to be labeled as the "shark attack capital of the world"? First, it is a favorite spot for surfers. Moreover, its channel inlets attract sharks, and it contains ample sea life that acts as food for sharks. The high number of incidents is a pointer to why increased awareness and caution become relevant for every beachgoer.
- __Regional Concentration__: Volusia County is a county with several beaches that feature highly in the rankings of shark-attack locations. In addition to New Smyrna Beach, both Daytona Beach and Ponce Inlet have tall counts of 31 and 18 incidents, respectively. Such concentration would point to more localized factors in raising shark–human interactions ascribable to socio-economic, physical, and behavioral patterns of sharks and humans.
- __International Presence:__ It comprises those countries that host some of the world's most famous shark attack points, including Boa Viagem in Recife, Brazil, and Durban in South Africa. Warm waters and rich marine life attract tourists and water sport enthusiasts worldwide, but at the same time, they bring enhanced risks of shark encounters. Therefore, effective management strategies become a necessity not only for ensuring public safety but also for the preservation of marine biodiversity.
<br />
<br />

- <img src="images/Top10_Cases_By_Injury_Type.jpg" width="400">

- **Top 10 Cases By Injury Type:**
This analysis provides insights into the types of injuries suffered by shark attack victims. Some of the key observations or trends obtained from the analysis include:
- __Limb Injuries Are Preponderant__: By far, the greatest number of injuries reported from shark attacks includes bites to limbs: feet, legs, hands, arms—all appendages. This serves as a notice of the vulnerability of extremities during encounters with the sharks since these body extremities usually are open to and in the reach of a shark's jaws during swimming, surfing, or other water-based activities.
- __Lower Extremities:__ Injuries to the feet, legs, and thighs are very predominant in the top cases, with "Foot Bitten," "Leg Bitten," and variations like "Left Foot Bitten" and "Right Foot Bitten" very well represented. The lower limbs become preferred targets in shark attacks, probably because the splashing of a human's lower body could resemble the movement of some of their natural prey or trigger additional hunting-related instincts.
– __Variation in Severity:__ Even though limb injuries formed the bulk of cases, the severity of shark attack-related injuries varies greatly, based on a host of specific factors: "size and species of shark, depth and location of the bite, and promptness of medical treatment." In some, one finds serious injuries, such as in traumatic amputations or large-area tissue damage. This attests to the potentially life-threatening nature of shark attacks.
- __Importance of Hand and Arm Protection__: Though not as common as limb injuries, bites to the hands and arms still make up a fair percentage of all reported cases. Protecting the upper extremities by providing appropriate gear, such as wetsuits or gloves, can reduce the potential for harm and offer some protection against shark bites during water sports or activities.
<br />
<br />

## Visuals in Power BI Report:
You can view and interact with this dashboard report on Shark Attacks (1900-2017) Analysis [here](https://app.powerbi.com/view?r=eyJrIjoiNzkwNjNhNTktZDUzZi00NzhhLThlYWQtY2IxOGYwMzliMDQyIiwidCI6IjdlYzI5NjU5LTNjZjItNGYzZi1hYmIzLWE3MjJlZGY3ZmYyZCJ9).
<br />
<br />
<br />

## Recommendations On Mitigating Shark Attack Risks:
- __Public Education:__ Conduct information campaigns on shark behavior and hazards, with guidelines for avoiding high-risk behaviors near shorelines.
- __Beach Safety:__ More lifeguards and installation of warning signs; technology to be deployed in real-time shark detection and alerts.
- __Tech and Innovation:__ Development of shark repellent technologies and wearable safety devices for water enthusiasts.
- __Fisheries Management:__ Implement sustainable fishing to maintain healthy shark populations; also, collaborate with fishing communities in order to reduce incidental catches.
- __Community Engagement__: There needs to be one stakeholder engagement for overarching strategies, while there must be enhanced citizen science initiatives and beach cleanups that encourage community involvement.
<br />
<br />

## Thank You For Following Through!
![](images/Thank_You_1.jpg)
