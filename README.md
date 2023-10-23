# IT-Service-Desk-Dashboard

### Introduction

The IT Service Desk Dashboard provides a comprehensive view of KPIs and insights for monitoring and managing IT service operations. It is designed to help managers and stakeholders gain a quick and clear understanding of the service desk's performance and requestor satisfaction.

### Data Preparation

<img width="900" alt="image" src="https://github.com/rcfrazier127/IT-Service-Desk-Dashboard/assets/63532077/69dc432e-ff20-4e7c-a728-da421d7bedf8">

This dataset was checked for blank/empty fields, errors and other discrepancies. Column headers were standardized, irrelevant columns were removed, and the satisfaction and severity columns were split to remove numeric values specifying tiers/score levels. The data only contains ticket creation dates between March and October of 2020. 

### Data Model

<img width="1180" alt="image" src="https://github.com/rcfrazier127/IT-Service-Desk-Dashboard/assets/63532077/c9159583-f670-484b-915a-caa8a52ff3ed">

The data was modeled into 6 dimension pages, each linked to a central fact table. An additional table was created that contains custom columns for the buckets used to display tickets by open days. This column was made in Power Query using the M language and a sort order column was also created to allow for the buckets to be sorted properly in the bar graph visual.

### Dashboard Page

<img width="1575" alt="image" src="https://github.com/rcfrazier127/IT-Service-Desk-Dashboard/assets/63532077/6033614b-9a9a-45ff-b03e-090e6cb5a6c0">

The dashboard page features visuals that are intended to provide an at-a-glance of the service desk's operation performance and allows users to delve deeply into factors surrounding ticket status and requestor satisfaction ratings. The visuals within this dashboard provide an analysis of ticket volumes by ticket severity, issue category, ticket type, and the number of days tickets remain open. Users can utilize these insights to identify bottlenecks along the ticket resolution pipeline and understand this ultimately impacts requestor satisfaction. The distribution of these satisfaction scores is also visualized for further analysis. The most unique feature of this dashboard is the time series analysis of ticket volumes which has slicers that only filter the data within this specific visual. A slicer reset button is included in the top corner of the page.

### Future Works

An additional dashboard page that allows for the filtering of the IT service desk operations as of the latest day within the dataset, which would simulate viewing the data as of the current day.
