# ESG-Project for Regression (STAT 415-615)

<!-- PROJECT LOGO -->
<br />
  <a href="https://github.com/Karene123/ESG-Project">
    <img src="https://github.com/Karene123/ESG-Project/assets/70621033/26b3a4fd-b7a9-4385-b2d9-49475c08ce96" alt="Logo" width="1500" height="500">
  </a>
  
<!-- TABLE OF CONTENTS -->
### Table of Contents

1. [Project Overview](#Project-Overview)
2. [Getting Started](#Getting-Started)
3. [Prerequisites](#Prerequisites)
4. [Utilized Python Libraries](#Utilized-Python-Libraries)
5. [Installation](#Installation)
6. [Project Motivation](#Project-Motivation)
7. [Summary of Results](#Summary-of-Results)
9. [Contributions](#Contributions)
10. [Acknowledgments](#Acknowledgments)
11. [File Description](#File-Description)


# Environment, Social, and Government Data (ESG) from the World Bank Data Bank

<!-- Project Overview -->
## About The Project

Since 2019, the World Bank has introduced the Sovereign ESG Data Framework focusing on Environmental, Social, and Governance pillars aligned with their 17 sustainable development goals. This framework aims to assist potential investors and illuminate a country's sustainability performance. Our study delves into exploring associations among variables within these themes. Specifically, we focus on anticipated lifespan as the response variable in our multiple regression model. Our interest lies in understanding how these variables influence life expectancy across various groups, including gender, development status, income, and regions such as Latin America, European Union, Central Asia, East Asia, and the Pacific, spanning a 5-year timeframe.

The variables we were interested in analyzing to study their association to life expectancy include: 
- (1)  CO2 emissions (metric tons per capita)
- (2) prevalence of overweight (% of adults)
- (3) hospital beds (per 1000 people)
- (4) fertility rate (births per women)
- (5) government effectiveness (estimate)
- (6) portion of seats held by women in national parliaments (%)
- (7) political stability and absence of violence/terrorism (estimate)
- (8) GDP (annual growth %)
- (9) school enrollment primary and secondary and gender parity index (gross)
- (10) ratio of female to male labor force participation rate (%)
- (11) voice and accountability (estimate)
- (12) population density (people per sq. km of land area)
- (13) fossil fuel (% of total)
- (14) Rule of Law
- (15) Internet Usage

We choose these variables to explore different interests across group members and to explore possible associations among different categories of indicators (i.e. the impact of climate change on life expectancy). The sample size is 1,081. 

<!-- GETTING STARTED -->
## Getting Started

All the predictors were carefully picked and downloaded from [The World Bank DataBank](https://databank.worldbank.org/source/environment-social-and-governance-(esg)-data) 
This link leads directly to the website.

### Prerequisites

[R-4.3.2](https://cran.r-project.org/bin/windows/base/)

Install and Import those libraries in order to access the project.

### Utilized Python Libraries:

* [NumPy](http://www.numpy.org/)
* [Pandas](http://pandas.pydata.org/)
* [Scikit-learn](http://scikit-learn.org/stable/)
* [Matplotlib](http://matplotlib.org/)
* [Seaborn](https://seaborn.pydata.org/)
* [Folium](https://pypi.org/project/folium/)
* [SciPy](https://www.scipy.org/)
* [lightgbm](https://lightgbm.readthedocs.io/en/v3.3.2/)

We wished to examine different variables that are not traditionally associated with life expectancy or social determinants of health. 

As part of this project, the following statistical methods were utilized:
- Overall F-test
- Transformations involving the use of log
- Simple Linear Regression

We were able to provide a model including 5 variables out of the original 15. 

The presentation is under: ESG Regression Final

![ESG pic1](https://github.com/Karene123/ESG-Project/assets/70621033/22c91fc9-dfbb-4c54-b480-b0da86948984)
![ESG pic2](https://github.com/Karene123/ESG-Project/assets/70621033/04ac5925-08be-44c3-bfd2-5a604fa162f7)

