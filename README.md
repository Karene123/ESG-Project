# ESG-Project for Regression (STAT 615)

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
6. [Challenges](#Challenges)
7. [Summary of Results and Methods Used](#Summary-of-Results-and-Methods-Used)
8. [Contributions](#Contributions)
9. [Acknowledgments](#Acknowledgments)
10. [Graphs](#Graphs)


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

* [Car](https://cran.r-project.org/web/packages/car/index.html)
* [GGally](https://cran.r-project.org/web/packages/GGally/index.html)
* [Broom Mixed](https://cran.r-project.org/web/packages/broom.mixed/index.html)
* [Nlme](https://svn.r-project.org/R-packages/trunk/nlme/R/nlme.R)
* [Broom](https://broom.tidymodels.org/)
* [Stringr](https://stringr.tidyverse.org/)
* [Tidyverse](https://dplyr.tidyverse.org/)

### Installation

* Car
  ```sh
  install.packages("car")
  ```
* GGally
  ```sh
  install.packages("ggally")
  ```
* Broom Mixed
  ```sh
  install.packages("broom.mixed")
  ```
* Nlme
  ```sh
  install.packages("nlme")
  ```
* Broom
  ```sh
  install.packages("broom")
  ```
* Stringr
  ```sh
  install.packages("stringr")
  ```
* Tidyverse
  ```sh
  install.packages("tidyverse")
  ```
  
  <p align="right">(<a href="#readme-top">back to top</a>)</p>

  ## Challenges
  The initial assumption of the independence model is violated due to correlations among data points within each country over time. To address this issue, we applied a linear mixed-effects model, considering the correlation within countries. After conducting residual analysis and implementing required log transformations, we assessed and satisfied the assumptions of constant variance and linearity for both the response and predictor variables.

  ## Summary of Results

We wished to examine different variables that are not traditionally associated with life expectancy or social determinants of health. 
As part of this project, the following statistical methods were utilized:
- Overall F-test
- Transformations involving the use of log
- Simple Linear Regression

We were able to provide a model including 14 variables out of the original 17.
- Fossil Fuels
- log(C02)
- log(Fertility)
- GDP
- log(Population Density)
- School Enrollment
- log(Women’s Labor Participation Rate)
- log(Internet Usage)
- log(Hospital Beds)
- Government Effectiveness
- log(Women's Participation in Parliament)
- Political Stability
- Rule of Law
- Voice and Accountability
  
The following is the model used for our Multiple Linear Regression model: 
log(Predicted life expectancy) = 3.89 - .00009* Fossil Fuels - .00007* log(CO2) + .005* Overweight - .0059* log(Fertility) - .000038* GDP + .024* log(Population Density) + .028* School Enrollment - .00075* log(Women’s Labor Participation Rate) + .0035* log(Internet Usage) + .0019* log(Hospital Beds) + .0013* Government Effectiveness + .000053* log(Women’s Participation in Parliament) + .00075* Political Stability + .0027* Rule of Law - .00038* Voice and Accountability.


<p align="right">(<a href="#README-top">back to top</a>)</p>

<!-- ACKNOWLEDGMENTS -->
## Acknowledgments

I worked closely with my classmates (Lindsay, Elizabeth, and Micheala) to bring this project to fruition, fostering a collaborative environment where each team member's unique strengths contributed to the project's success. Through open communication and shared dedication, we overcame challenges and celebrated our collective achievements, solidifying the importance of teamwork in delivering outstanding results.

- [ESG image](https://www.kiplinger.com/investing/esg/what-is-esg)

The presentation is under: ESG Regression Final
<p align="right">(<a href="#readme-top">back to top</a>)</p>

## Graphs

![ESG pic1](https://github.com/Karene123/ESG-Project/assets/70621033/22c91fc9-dfbb-4c54-b480-b0da86948984)
![ESG pic2](https://github.com/Karene123/ESG-Project/assets/70621033/04ac5925-08be-44c3-bfd2-5a604fa162f7)

