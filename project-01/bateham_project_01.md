# Fuel Consumption Analysis Project

## Project Overview

This project analyzes fuel consumption data to identify trends, compare vehicle characteristics, and visualize key findings related to fuel efficiency. The primary dataset used is `fuel.csv`.

## Project Structure

The project is organized as follows:


dataviz_mini-project_01/
|- fuel_analysis.Rproj  # RStudio Project file
|- data/
|  |- fuel_analysis.csv               # The raw dataset used for analysis
|- report/
|  |- fuel_analysis.Rmd      # R Markdown file containing the analysis code and narrative
|  |- fuel_analysis.html     # HTML report generated from the R Markdown file
|- README.md                # This file: provides an overview of the project


## How to Reproduce the Analysis

1.  **Prerequisites:**
    * R (version 4.0 or later recommended)
    * RStudio (recommended IDE)
    * The following R packages:
        * `tidyverse` (for data manipulation and visualization)
        * `lubridate` (for date/time manipulation, if applicable)
        * `knitr` (for generating the report from R Markdown)

    You can install these packages in R using:
    ```R
    install.packages(c("tidyverse", "lubridate", "knitr"))
    ```

2.  **Setup:**
    * Clone or download this project repository.
    * Ensure the `fuel.csv` dataset is placed in the `data/` subfolder. If you have a different dataset, update the file path in `report/fuel_analysis.Rmd`.

3.  **Running the Analysis:**
    * Open the `your-project-name.Rproj` file in RStudio. This will set the working directory correctly.
    * Open the `report/fuel_analysis.Rmd` file.
    * Click the "Knit" button in RStudio (or run `rmarkdown::render("report/fuel_analysis.Rmd")` in the R console). This will execute the R code within the Rmd file and generate an HTML report (`fuel_analysis.html`) in the `report/` folder.

## Key Files

* **`data/fuel.csv`**: The input dataset. *You should briefly describe your dataset here: what it contains, its source (if known), and any important characteristics.*
* **`report/fuel_analysis.Rmd`**: The core of the analysis. This R Markdown document includes all R code for data loading, cleaning, summarization, visualization, and the narrative explaining the process and findings.
* **`report/fuel_analysis.html`**: The final, human-readable report generated from the `.Rmd` file. This is the primary output to share.

## Findings Summary

The analysis of the `fuel.csv` dataset revealed several key trends in vehicle fuel consumption. Notably, there was a **drastic increase in average combined MPG for vehicles manufactured after 2010**, suggesting significant improvements in automotive technology and efficiency standards around that time. The study also confirmed that **engine displacement generally has an inverse relationship with fuel efficiency**, meaning larger engines tend to result in lower MPG. Among the different vehicle classes analyzed, **"Small Station Wagons" demonstrated the highest average combined MPG**, indicating this category may offer a good balance of utility and fuel economy. These findings highlight an evolving automotive landscape with increasing emphasis on fuel efficiency.


