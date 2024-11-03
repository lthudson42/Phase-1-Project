![commercial-airplane-jetliner-flying-above-600nw-788233372](https://github.com/user-attachments/assets/b9ef7e31-a889-47a8-835f-948118a4e64b)

# Portfolio Diversification Needed:
Commercial Aviation for Polaris Capital
Author: __[Liam Hudson](https://www.linkedin.com/in/liamhud-son)__

## Overview
This project investigates civil aviation accident dataset from the __[National Transportation Safety Board](https://www.ntsb.gov/Pages/home.aspx)__ (NTSB), containing over 90,000 records of accident data between 1962 to 2023. Using data cleaning, analysis, and visualization techniques, the primary goal is to find the safest aircrafts based on a number of variables. These include the number of engines in each aircraft, its type of engine, injury severity, and injury count.

## Business Understanding
My business, Polaris Capital, wants to diversify its reach into new industries. I am tasked with investigating the potential risk of aircrafts and making three business suggestions that will help to make a decision that takes on as little risk as possible. I will base my suggestions on various components of an aircraft that have demonstrated low risk in the overall dataset of aviation accidents. Polaris Capital will use these suggestions to purchase and operate aircrafts for commercial and private enterprises.

## Data Understanding
The National Transportation Safety Board has a comprehensive dataset that records all civil aviation accidents from 1962 all the way to 2023. Each accident has a unique Event ID associated with aircraft components like make, model, and engine type. The data also records external variables like weather conditions, total injuries (i.e., minor, severe, fatal, and/or uninjured), and the phase of the flight.

## Data Preparation
This project uses data cleaning analysis to determine which variables are the most and least relevant to the investigation. Columns that are deemed to be irrelevant are dropped, whereas columns that are relevant are kept and further filtered. Any records containing NaN values in significant columns are also dropped.

## Analysis and Results/Recommendations
The main components that my business should use to purchase and operate the aircrafts with the least amount of risk:

* Boeing

    * Turbo Shaft engine
    * Turbo Prop engine
    * Reciprocating engine
        * At least 4
        
* Airbus

    * Turbo Fan engine
        * At least 2

The variables that these decisions are based on:
* Non-Fatal injury severity
* Frequency of records with given engine type/count
* Injury count of 0 (i.e., Minor, Serious, etc.)

![image](https://github.com/user-attachments/assets/8bff992e-42b0-4bc2-b293-c840d2c8aefd)

This chart shows the significantly large frequency of Reciprocating and Turbo Fan engines in aviation accidents. Thus, these components need to be avoided.

![image](https://github.com/user-attachments/assets/c0384a95-5cae-4b98-8352-e97c428d6100)

Though, this chart demonstrates that aircrafts with 4 Reciprocating engines can be safe due to an incredibly small frequency in the dataset.

![image](https://github.com/user-attachments/assets/02b40b85-5eb0-4a33-a557-2486053a29c9)

This chart demonstrates that there is no recognizable correlation between the count of Turbo Jet engines in Boeing aircrafts. Thus, these cannot be deemed as a safe option.

## Conclusion

This analysis has led to three primary recommendations for Polaris Capital to consider when looking for aircrafts to puchase and operate:

1. **Airbus and Boeing aircrafts are the best option for commercial use.**  Not only do these two manufacturers produce very popular commercial jets, but their planes are reliable and contain components that greatly minimize risk in the case of an unlikely accident.

2. **Turbo shaft and Turbo prop are consistently reliable.** Within the Boeing models that I have recommended, many have a turbo engine. But, upon deep analysis, it can be deduced that only the Shaft and Prop variations are reliable. <br>On the other hand, all the Airbus models I have recommended have only 2 Turbo Fan engines, but still perform significantly better with them than the Boeing models do.

3. **In the unlikely case of an aviation accident, it is important to select planes with an injury count of 0.** It is impossible to lower aviation accident rates to 0%. As a result, when selecting an aircraft to invest in, having an injury count of 0 speaks volumes to the plane's safety mechanisms and overall structure. All of the models I have recommended have had an injury count of 0 when in an accident.

## Next Steps

Further analyses could expose more insight to potentially better alternatives:

* Better predictions of accidents' causes. Many variables that were not detailed in this dataset could play a significant role in the cause of an accident.

* Detailed research into "Probable Cause" accident reports. The National Transportation Safety Board explores "Probable Cause" in this __[documentation](https://www.faa.gov/sites/faa.gov/files/2022-11/Boeing%20review%20of%20NTSB%20probable%20cause.pdf)__, meaning that there is a comprehensive report on exactly what caused each particular accident. When deciding on an aircraft to purchase and operate, it could be important to look at the specifics of what caused its crash.

* Looking at outliers in the data. My task was to identify the main components of an aircraft that are the least likely to cause an accident. However, there were some records that had outlier data, like the planes with "Electric," "LR," "Hybrid Rocket," and "Geared Turbofan" engine types. I chose not to investigate those records as they composed a small percentage of the data and would not result in a conducive analysis.

## For More Information
See the full breakdown of this dataset in this __[Jupyter Notebook](https://github.com/lthudson42/Phase-1-Project/blob/ad28e77735295df3193c8d381ed05543b50f42f2/polaris_capital_aircraft_analysis.ipynb)__ or viewing this __[presentation]()__. Additional visualizations are also available to view on this interactive __[Tableau Dashboard](https://public.tableau.com/views/BoeingandAirbusModelsDashboard/BoeingandAirbusModelsDashboard?:language=en-US&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link)__.

## Repo Structure

```
├── Data
├── .gitignore
├── Polaris_Capital_Analysis_Presentation.pdf
├── README.md
└── polaris_capital_aircraft_analysis.ipynb
```
