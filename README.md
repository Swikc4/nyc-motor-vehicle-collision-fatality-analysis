<a id="readme-top"></a>

<br />
<div align="center">
  <h3 align="center">NYC Motor Vehicle Collision Fatality Analysis</h3>
  <p align="center">
    Binary logistic regression on NYC collision records to test whether Ford vehicle involvement is associated with fatal crashes, a CIS 3920 team project at Baruch College
    <br />
    <a href="https://github.com/Swikc4/nyc-motor-vehicle-collision-fatality-analysis"><strong>Explore the repo »</strong></a>
  </p>
</div>

<details>
  <summary>Table of Contents</summary>
  <ol>
    <li><a href="#about-the-project">About The Project</a>
      <ul><li><a href="#built-with">Built With</a></li></ul>
    </li>
    <li><a href="#materials">Materials</a></li>
    <li><a href="#dataset">Dataset</a></li>
    <li><a href="#key-findings">Key Findings</a></li>
    <li><a href="#usage">Usage</a></li>
    <li><a href="#team-context">Team Context</a></li>
    <li><a href="#acknowledgments">Acknowledgments</a></li>
  </ol>
</details>

## About The Project

Academic team analysis completed for CIS 3920 Data Mining for Business Analytics at Baruch College in Spring 2026.

The analysis examined whether Ford vehicle involvement was independently associated with fatal crash outcomes after accounting for driver, vehicle, and time related factors in NYC motor vehicle collision data.

I worked as part of a four person team with Shazrim Farin, Ethan Ma, and Geovanni Ramos.

<p align="right">(<a href="#readme-top">back to top</a>)</p>

### Built With

* ![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
* ![pandas](https://img.shields.io/badge/pandas-150458?style=for-the-badge&logo=pandas&logoColor=white)
* ![statsmodels](https://img.shields.io/badge/statsmodels-4B8BBE?style=for-the-badge)

<p align="right">(<a href="#readme-top">back to top</a>)</p>

## Materials

* [`team_project_details.md`](team_project_details.md) documents the final research question, dataset, model, findings, and team attribution.
* [`results/model_output.txt`](results/model_output.txt) contains the statsmodels binary logistic regression output from the analysis, including descriptive statistics, the unadjusted and adjusted models, and the male-only and female-only models.

<p align="right">(<a href="#readme-top">back to top</a>)</p>

## Dataset

The dataset was provided by the professor: 89,102 collision records across 27 columns, sourced from NYPD crash records. After cleaning and preparing the modeling data, the final dataset contained 70,272 observations.

Fatal crashes were very rare in the final dataset, with 39 fatal crashes, or about 0.055 percent of observations.

Note: the CSV in `data/` is currently an empty placeholder file. A rename through the GitHub website emptied the upload, so the raw data itself is not available in this repository right now.

<p align="right">(<a href="#readme-top">back to top</a>)</p>

## Key Findings

Ford involvement was not statistically significant at the 0.05 level after controlling for the other variables in the model (coefficient 0.7343, p = 0.070).

Large vehicle involvement was positively associated with fatal crash risk (coefficient 0.6626, p = 0.049), while rush hour crashes were negatively associated with fatal outcomes in the fitted model (coefficient -1.0723, p = 0.038).

The adjusted model was statistically significant overall (LLR p = 0.003674), but with 39 fatal crashes out of 70,272 records, the results describe associations in this dataset, not causes.

<p align="right">(<a href="#readme-top">back to top</a>)</p>

## Usage

This repository documents the analysis and its results; there is no runnable code here. Start with `team_project_details.md` for the research question, dataset, and findings, then see `results/model_output.txt` for the full statsmodels binary logistic regression output, including descriptive statistics and model coefficients.

<p align="right">(<a href="#readme-top">back to top</a>)</p>

## Team Context

The course was conceptual, and the Python code was provided by the professor. This repository contains the project write-ups and model output, not the original Python code.

This was completed by a four person academic team. The repository documents the analysis without presenting the full team work as my individual contribution.

<p align="right">(<a href="#readme-top">back to top</a>)</p>

## Acknowledgments

* CIS 3920 Data Mining for Business Analytics, Baruch College (Zicklin School of Business)
* NYC Open Data: [Motor Vehicle Collisions](https://data.cityofnewyork.us/Public-Safety/Motor-Vehicle-Collisions-Crashes/h9gi-nx95)
