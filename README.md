---
editor_options: 
  markdown: 
    wrap: 72
---

**Author(s):** Ross, Connor & Wells, Katie

**Instructor:** Handel, Andreas PhD

**Course:** EPID 8060

**Semester:** Spring 2023

**Title:** *Potential Drivers of COVID-19 Vaccine Administration Differences in the US*

**Manuscript:** Manuscript.docx (Manuscript.docx -> products ->
connor-katie-MADA-project)

## Code Run Order/Reproducibility:

-   Code files can be found in the 'code' folder of the project. See
    below for specific file locations.

-   In order to ensure that this project is reproducible and all files
    generate as intended. Please run in the following order from first
    to last

    1.  wrangling.qmd (wrangling.qmd -> processing_code -> code ->
        connor-katie-MADA-project)

    2.  exploration.qmd (exploration.qmd -> processing_code -> code
        connor-katie-MADA-project)

    3.  fitting.qmd (fitting.qmd -> analysis_code -> code ->
        connor-katie-MADA-project)
        
    4.  analysis.qmd (analysis.qmd -> analysis_code -> code -> 
        connor-katie-MADA-project)

    5.  Manuscript.qmd (Manuscript.qmd -> manuscript -> products ->
        connor-katie-MADA-project)

## Data/Data Files Information:

-   raw_data:
    COVID-19_Vaccinations_in_the_United_States_Jurisdiction.csv ->
    raw_data -> data -> connor-katie-MADA-project (OR raw_data.rds -
    same location)

    -   From: Centers for Disease Control and Prevention. Data.CDC.gov.
        COVID-19 Vaccinated in the United States, Jurisdiction.
        <https://data.cdc.gov/Vaccinations/COVID-19-Vaccinations-in-the-United-States-Jurisdi/unsk-b7fc>

-   processed_data: SubData.csv -> processed_data -> data ->
    connor-katie-MADA-project ( OR SubData.rds - same location)

    -   Added Region based on state as well as filtered for years of
        interest 21 - 22.

## Code Files Information:

-   Wrangling/Preparing the Data (wrangling.qmd -> processing_code ->
    code -> connor-katie-MADA-project)

    -   Imports raw dataset. Formats date

    -   Creates SubData which add US Region based on state information.
        Filters for years of interest 21 - 22

    -   Lays framework for the graphs used in exploration of the data
        (found in exploration.qmd).

-   Exploration/Exploring and Visualizing the Data (exploration.qmd ->
    processing_code -> code -> connor-katie-MADA-project)

    -   Run to see the following visualizations:

        -   Vacccine Distribution Overtime by Manufac. US Wide

        -   Vaccine Administration Overtime by Manufac. US Wide

        -   Vaccines Administered in Southeast Region

        -   Vaccines Administered in Northeast Region

        -   Vaccines Administered in MidWest Region

        -   Vaccines Administered in SouthWest Region

        -   Vaccines Administered in West Region

## Fitting Models

-   Fitting Models (fitting.qmd -> analysis_code -> code ->
    connor-katie-MADA-project)

    -   lm1:

        -   Outcome: Overall vaccine count

        -   Predictor: Region

    -   lm2 - lm6:

        -   Outcome: \<Vaccine Manufac.> Administered

        -   Predictor: Region

    -   lm7:

        -   Outcome: Administered (total)

        -   Predictor: Region & Distributed (total)

    -   lm8:

        -   Outcome: Administered (total)

        -   Predictor: Region

    -   lm9:

        -   Outcome: Administered (total)

        -   Predictor: Distributed (total)

    -   NOTE: Some include 'model checks'




