# Opioid Utilization Rates and Substance Use Disorder Trends
### Team:
* Kameron Thao
* Mary Vang
* Sandra Braun 

## Introduction
According to the CDC, substance use disorders (SUDs) are treatable chronic conditions marked by an unhealthy pattern of substance use, resulting in health impairments, social dysfunction, and lack of control over substance use. This cluster of physical, behavioral, and cognitive manifestations indicates a person's continuous use of the substance in spite of harmful effects. The presence of symptoms due to substance use (drugs or alcohol) can assist providers in diagnosing a person with an SUD. The range of SUDs can range from mild to extreme, and it can affect anyone regardless of race, gender, income level, or social class.<sup>1</sup>

Opioids are a class of drugs that bind to opioid receptors on nerve cells in the body and brain, resulting in decreased pain signals and sensations. This category of drugs consists of the illicit drug heroin; synthetics such as fentanyl, which often are manufactured and obtained illegally; and legally-obtained prescriptions like oxycodone, hydrocodone, codeine, and morphine.<sup>2</sup>

According to the CDC, in 2020 there were 40.3 million Americans aged 12 or above who had a SUD in the past year. This equates to one in seven individuals reporting the presence of a SUD.1 The CDC also reported that 2.7 million of those individuals suffered from an opioid use disorder specifically in the last year.<sup>2</sup>

It is important to note that SUDs can include alcohol, cannabis, hallucinogens, inhalants, opioids, sedatives, hypnotics, anxiolytics, stimulants, nicotine, and any other substance. These afflictions can lead to substantial obstacles in all aspects of an individual's life, including employment, education, and home life. To ensure positive results, coordinated care is paramount in treating anyone with a SUD and any simultaneous disorders, such as mental health conditions.<sup>1</sup>

## Analysis Objective: 
The purpose of this analysis is to identify if there are any relationship or trends between opioid utilization and substance use disorders in the U.S. (2020)

* Is there an association between population and prescription count? 
* What are the top 5 states with the highest numbers of prescriptions? 

* What are the top 5 states with the highest rates in substance usage, risk, and disorder? 
* Is there any association between substance usage, risk, and disorder?

* Is there an association between usage, risk, and disorder rates to prescription counts? 
* Is there an association between opioid prescribing rates and substance use disorder? 

### Data:
**CMS State Drug Utilization Data**
* https://www.medicaid.gov/medicaid/prescription-drugs/state-drug-utilization-data/index.html
* Data covered outpatient drugs paid for by state Medicaid agencies 

**2019-2020 National Survey on Drug Use and Health: Model-Based Prevalence Estimate (50 States and the District of Columbia)** 
* https://www.samhsa.gov/data/report/2019-2020-nsduh-state-prevalence-estimates
* Nation survey on drug use and health 
* Model-Based prevalence estimates for 50 U.S. States

**American Community Survey - Demographic and Housing Estimates**
* https://data.census.gov/table?q=DP05
* Census on the 50 U.S States 

### Method/Techniques: 
* Python
* Pandas
* Numpy 
* Matplotlib 
* Scipy 

## Findings 
### Relationship between Population and Prescription

![Population vs Prescription](Images/1/Population%20vs%20Prescription.png)

* R-squared: 0.76
* Correlation Coefficient: 0.87
* pvalue: 6.47
* The analysis between Population and Prescription Count indicates a weak positive relationship between the two variables. This means that as the population increases, the number of prescriptions count also increases. However, with a pvalue of 6.47, we do not have sufficient information to conclude if there is a significant relationship between the two variables.  

### Relationship between Substance Usage, Risk, and Disorder Rates

![Usage vs Risk](Images/2/Usage%20vs%20Risk.png)

* R-squared: 0.04
* Correlation Coefficient: -0.21
* pvalue: 0.15
* The analysis between Substance Usage Rates and Risk Rates indicates a negative relationship between the two variables. This means that as the usage rates increase, the risk rates decrease. However, with a low R-squared value and a negative correlation coefficient, it is important to consider other factors that may affect the relationship between the two variables. 

![Usage vs Disorder](Images/2/Usage%20vs%20Disorder.png)

* R-squared: 0.19
* Correlation Coefficient: 0.43
* pvalue: 0.001
* The analysis between Substance Usage Rates and Disorder Rates indicates a positive relationship between the two variables. The R-squared value and correlation coefficient provide valuable insights into the relationship between the two variables, while the pvalue indicates the strength of the relationship. 

![Risk vs Disorder](Images/2/Risk%20vs%20Disorder.png)

* R-squared: 0.37
* Correlation Coefficient: -0.61
* pvalue: 1.87
* The analysis between Substance Risk Rates and Disorder Rates indicates a weak positive relationship between the two variables. However, with a pvalue of 1.87, we do not have sufficient information to conclude if there is a significant relationship between the two variables. 

### Relationship between Prescription and Substance Usage, Risk, and Disorder

![Prescription vs Usage](Images/3/Rx%20vs%20Usage.png)

* R-squared: 0.09
* Correlation Coefficient: -0.31
* pvalue: 0.03
* The analysis between Prescription Count and Substance Usage Rates indicates a negative relationship between the two variables. This insight can be used to address reduction in prescription count and improve patient's health. 

![Prescription vs Risk](Images/3/Rx%20vs%20Risk.png)

* R-squared: 0.00
* Correlation Coefficient: 0.017
* pvalue: 0.91
* The analysis between Prescription Count and Substance Risk Rates indicates a weak positive relationship between the two variables. However, with a pvalue of 0.91, we do not have sufficient information to conclude if there is a significant relationship between the two variables. 

![Prescription vs Disorder](Images/3/Rx%20vs%20Disorder.png)

* R-squared: 0.03
* Correlation Coefficient: -0.16
* pvalue: 0.26
* The analysis between Prescription Count and Substance Disorder Rates indicates a weak positive relationship between the two variables. However, with a pvalue of 0.26, we do not have sufficient information to conclude a significant relationship between the two variables. 

## Summary
Based on the findings, there is a weak positive relationship between prescription count and substance usage, risk, and disorder rates. Further analysis is needed to determine if there is any relationship that can draw insights in making decisions pertaining to substance use disorders. Overall, the findings suggest that reducing prescription count and improving substance use and risk management can contribute to improving patient health and reducing the risk of substance abuse and disorders. 

### Citations

1.	“Substance Use Disorders (SUDS).” Centers for Disease Control and Prevention, Centers for Disease Control and Prevention, 5 Oct. 2022, https://www.cdc.gov/dotw/substance-use-disorders/index.html. 
2.	“Opioid Use Disorders (SUDS).” Centers for Disease Control and Prevention, Centers for Disease Control and Prevention, 5 Oct. 2022, https://www.cdc.gov/dotw/opioid-use-disorder/index.html. 
3.	“State Drug Utilization Data.” Center for Medicare and Medicaid Services, Health and Human Services, https://www.medicaid.gov/medicaid/prescription-drugs/state-drug-utilization-data/index.html.
4.	“2019-2020 National Survey on Drug Use and Health: Model-Based Prevalence Estimates (50 States and the District of Columbia).” Substance Abuse and Mental Health Services Administration, U.S. Department of Health &amp; Human Services, 29 Dec. 2021, https://www.samhsa.gov/data/report/2019-2020-nsduh-state-prevalence-estimates.
5.	“2020 Demographic and Housing Five Year Estimates.” American Community Survey, U.S. Census Bureau, https://data.census.gov/table?q=DP05.
6.	“NDC MME TABLE.” Opioid Drug Listing, New York State Department of Health, 4 Jan. 2021, https://health.ny.gov/professionals/narcotic/docs/opioid_drug_listing.pdf.