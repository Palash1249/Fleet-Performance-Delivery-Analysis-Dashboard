# Fleet Performance & Delivery Efficiency Dashboard

> An interactive Power BI dashboard for exploring fleet trip
> performance, fuel efficiency, on-time delivery rates, and cost per
> kilometre for a logistics use case.

------------------------------------------------------------------------

## Project Overview

This project uses trip-level and vehicle information to examine
logistics operations, including delivery performance, fuel consumption,
vehicle costs, and route efficiency. The Power BI report brings these
measures together in interactive visuals to help explore operational
performance and identify areas that may need attention.

**Project type:** Data Analytics / Business Intelligence\
**Primary tool:** Microsoft Power BI Desktop

------------------------------------------------------------------------

## Dashboard Preview

Add a screenshot of your own customized dashboard to
`assets/dashboard-preview.png`, then use the image reference below:

![Fleet Performance Dashboard](assets/dashboard-preview.png)

For a full-page preview, see `Dashboard.pdf` if that file is included in
this repository.

------------------------------------------------------------------------

## Dataset

**Source file:** `logistics_project_dataset.xlsx`

  ------------------------------------------------------------------------
  Sheet                 Records stated in the source Description
                                              README 
  --------------------- ---------------------------- ---------------------
  `Trip_Data`                               50 trips Trip ID, Vehicle ID,
                                                     Driver ID, Origin,
                                                     Destination, Distance
                                                     (km), Fuel Consumed
                                                     (L), Delivery Status,
                                                     Delivery Date

  `Vehicle_Master`                        7 vehicles Vehicle ID, Vehicle
                                                     Type (Van, Truck,
                                                     Mini-Truck), Capacity
                                                     (kg), Maintenance
                                                     Cost
  ------------------------------------------------------------------------

### Delivery Status Summary

The source README reports the following distribution:

  Status      Count   Share
  --------- ------- -------
  On-Time        30     60%
  Late           20     40%

Please confirm these counts against the dataset if you modify or replace
the source data.

------------------------------------------------------------------------

## Analysis & Dashboard Components

### 1. Data Preparation and Modeling

The original project documentation describes: - Handling missing
fuel-consumption values using mean imputation. - Creating a relationship
between `Trip_Data` and `Vehicle_Master` using `Vehicle_ID`.

Verify these steps in the Power Query Editor and model view of the PBIX
file before treating them as final implementation details.

### 2. Key Measures

The original project documentation lists the following KPI logic:

  Measure              Calculation
  -------------------- -------------------------------------------
  Fuel Efficiency      Distance / Fuel Consumed
  On-Time Delivery %   On-Time Trips / Total Trips
  Cost per km          (Fuel Cost + Maintenance Cost) / Distance

The source README states that fuel cost is assumed to be **₹100 per
litre** as specified in the assignment. Check the actual DAX and cost
calculation in the PBIX before relying on this assumption.

### 3. Visualizations

The original documentation describes these visuals:

  Visual       Analysis
  ------------ ------------------------------------------
  Bar chart    On-Time Delivery % by Destination
  Line chart   Fuel Efficiency trend by Delivery Date
  KPI card     Average Delivery Time
  KPI card     Average Cost per km
  Pie chart    Vehicle Type vs Average Maintenance Cost

### 4. AI-Powered Visuals

The original README lists: - **Q&A visual:** Average Cost per km by
vehicle type. - **Key Influencers:** Delivery Status explained by
Distance, Vehicle Type, and Driver ID. - **Decomposition Tree:** Cost
per km explored by Vehicle Type, Maintenance Cost, and Distance.

Availability and configuration of these visuals may depend on the Power
BI version and sign-in.

------------------------------------------------------------------------

## Repository Contents

  File                                               Description
  -------------------------------------------------- -----------------------------------
  `Fleet_Performance_and_Delivery_Efficiency.pbix`   Power BI report
  `logistics_project_dataset.xlsx`                   Source dataset
  `Dashboard.pdf`                                    Dashboard preview, if included
  `assets/dashboard-preview.png`                     Repository screenshot to be added
  `README.md`                                        Project documentation

File names may differ depending on the contents of the downloaded
repository.

------------------------------------------------------------------------

## How to Use

1.  Clone this repository:

    ``` bash
    git clone https://github.com/Palash1249/Fleet-Performance-PowerBI.git
    ```

2.  Open the project folder.

3.  For a quick visual preview, open `Dashboard.pdf` if it is included.

4.  Open `Fleet_Performance_and_Delivery_Efficiency.pbix` in **Microsoft
    Power BI Desktop**.

5.  If Power BI prompts you to refresh the data, update the source path
    to the local `logistics_project_dataset.xlsx` file.

6.  Explore the report pages, filters, measures, and visuals.

Power BI Desktop is available from [Microsoft Power
BI](https://powerbi.microsoft.com/desktop/).

------------------------------------------------------------------------

## Tools Used

  -----------------------------------------------------------------------
  Tool                                Purpose
  ----------------------------------- -----------------------------------
  Microsoft Power BI Desktop          Dashboard development and
                                      visualization

  Power Query                         Data cleaning and transformation

  DAX                                 Measures and KPI calculations

  Microsoft Excel                     Source dataset

  Power BI AI visuals                 Q&A, Key Influencers, and
                                      Decomposition Tree, where available
  -----------------------------------------------------------------------

------------------------------------------------------------------------

## Learning & Customization Notes

This repository is based on an existing project. I am using it as a
learning reference and documenting any changes I make to the report.

Add your own completed work here before publishing, for example: -
Dashboard layout or theme changes. - New or modified DAX measures. -
Additional report pages or visuals. - Further analysis and observations
from the dataset.

Do not list a customization unless you have actually completed and
checked it.

------------------------------------------------------------------------

## Acknowledgements

Original project source and inspiration:

[Original GitHub repository](https://github.com/bibythayyil/bibythayyil)

Please review the original repository's licence and attribution
requirements before redistributing its files or a modified version.

------------------------------------------------------------------------

## Author

**Palash Halder**

-   GitHub: [Palash1249](https://github.com/Palash1249)
-   LinkedIn: \[Add your LinkedIn profile URL\]
