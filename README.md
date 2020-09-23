#  **COVID-19 Outcomes in Washington State:**

Analyzed Covid-19 data from Washington State to understand the relationship between income, poverty, political affiliation, and age with three Covid-19 outcomes: cases, hospitalizations, deaths.

Extracted data from the CDC, Census, and usa.com to assemble a dataset of over 50,000 cases.

Linear regression, Chi-Square, outlier analysis, and visualizations conducted using Python, Pandas, Plotly, and Matplotlib.

The full presentation of the project can be found here: [Covid-19 Presentation](https://github.com/mocchicone/Covid-19-Outcomes-in-Washington-State/blob/master/COVID-19%20Presentation.pptx)

## **Summary:** 

Our team was interested in exploring some lesser studied predictor variables for Covid-19 outcomes.  We decided to focus our research to Washington State to limit the scope of the project.  

## **Hypotheses:**

H1A: Washington counties grouped by political affiliation will show a significant difference in Covid-19 outcomes (cases, hospitalizations, and deaths).

H2A: Mean household income will negatively correlate to Covid-19 outcomes (cases, hospitalizations, and deaths).

H3A: Poverty rate will positively correlate to Covid-19 outcomes (cases, hospitalizations, and deaths).

Additionally, age and Covid-19 outcomes were examined visually.    

## **Initial Visualizations**

After sourcing, cleaning, and merging the data, we reviewed the summary statistics and created several visuals to get a first look at the data.  Some examples are presented below:

**Washington State: Mean Income by County**  
Here we can see how mean household income is spread accross the state, with more urban areas having a higher mean income.  Created using Plotly.   
![Income Heatmap](https://github.com/mocchicone/Covid-19-Outcomes-in-Washington-State/blob/master/Data%20Visualization/Visuals/Household%20Income%20Median.png)    
     
**Washington State: Political Affiliation by County**  
A map displaying majority political affiliation by county, based on the most recent sate senate election.  Created using Plotyly.  
![Political Affiliation Map](https://github.com/mocchicone/Covid-19-Outcomes-in-Washington-State/blob/master/Data%20Visualization/Visuals/politics_map.png)    
    
**Washington State: Age Categories by Covid-19 Outcomes**  
Bar graphs for each of the three Covid-19 outcome variables: cases, hosptalizations and deaths.  We can see here that while younger people make up a higher perecentage of cases, older people make up a higher pecentage of deaths.  Created using Matplotlib.  
![Covid Outcomes by Age Bar](https://github.com/mocchicone/Covid-19-Outcomes-in-Washington-State/blob/master/Data%20Visualization/Visuals/Age%20Bar%20Graphs.PNG)    

## **Analysis and Results**  
In order to compare counties with heterogeneous popuations, we used transformation on our outcome variables, so that we looked at cases, hospitalizations, and deaths per 100 thousand residents.   

**Outlier Analysis**  
We conducted an outlier analysis and found four counties that met our criteria.  The top three were all republican majority counties.  We conducted a simple linear regression with and without the outliers and found that it did greatly impact the strength of the model in that there was a strong positive correlation between income and Covid-19 outcomes when the outliers were removed.  Created using Matplotlib.
![Outlier1](https://github.com/mocchicone/Covid-19-Outcomes-in-Washington-State/blob/master/Data%20Visualization/Visuals/Outlier%20Analysis.PNG)
![Outlier2](https://github.com/mocchicone/Covid-19-Outcomes-in-Washington-State/blob/master/Data%20Visualization/Visuals/Outlier%20Analysis2.PNG)

**Linear Regression: Income, Poverty, and Population Density vs Covid-19 Outcomes**  
For democrat majority counties, we found a strong, positive correlation between mean income and all three Covid-19 outcomes.  There was not a significant correlation for republican majorty counties.  As the direction of the effect was in the opposite direction we investigated one potential confounding predictor varialbe: Population Density and found that it did positively correlate with the outome variable hospitalizations.  Created using Matplotlib.    
![Income vs Outcomes](https://github.com/mocchicone/Covid-19-Outcomes-in-Washington-State/blob/master/Data%20Visualization/Visuals/Income%20vs%20Outcomes.PNG)

**Chi Square: Democrat Majority Counties with Republican Majority Counties**  
We found a significant difference in Covid-19 cases per 100 thousand population when comparing democrat majority counties and republican majority counties.  Created using Matplotlib.
![Chi_Square Pie](https://github.com/mocchicone/Covid-19-Outcomes-in-Washington-State/blob/master/Data%20Visualization/Visuals/Chi-Square.PNG)

## **Conclusions and Insights**  

Revisiting our hypotheses, we conclude that: 

*H1A: Washington counties grouped by political affiliation will show a significant difference in Covid-19 outcomes (cases, hospitalizations, and deaths).*
- A significant difference was found between counties that voted majority republican vs majority democrat, in that republican majority counties has a signficantly higher rate of COVID-19 cases.

*H2A: Mean household income will negatively correlate to Covid-19 outcomes (cases, hospitalizations, and deaths).*
-   For democrat leaning counties income was significantly and positively correllated to all three Covid-19 outcomes.  This was the opposite direction of the effect that we predicted.  We investigated one potential confounding predictor variable, population density, which did show as significant positive correlation with hospitalizations.  

*H3A: Poverty rate will positively correlate to Covid-19 outcomes (cases, hospitalizations, and deaths).*
-  For democrat leaning counties poverty rate was significantly and negatively correllated to hospitalizations only

In conclusion we found evidence that supports our hypothesis that political affiliation may impact Covid-19 outomes at the county level.  We did not find evidence to support our hypotheses that lower income and higher poverty rates is correlated with higher Covid-19 outcomes.  We discovered the effect worked in the opposite direction, and found evidence that population density is a potental confounding predictor variable.

**Project Team Contacts:**   
Mike Occhicone: mpocchicone@gmail.com  
Drew Gilmore:   
Nghia Nguyen:  
James Park:   
Jessie King:   

