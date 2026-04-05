# san-antonio-police-calls-analysis
End-to-end GIS analysis of 5.2 million police service calls using Python and QGIS
# San Antonio Public Safety: Spatial Analysis of 5.2M Service Calls

## Project Overview
An MIS-focused analysis exploring the distribution of police service calls across San Antonio. This project bridges the gap between massive raw datasets and actionable geographic insights.

## Key Technologies
* **Python (Pandas, NumPy):** Data engineering and cleaning of 5.2 million records.
* **QGIS:** Spatial joins, zip-code aggregation, and cartographic design.
* **Data Source:** [San Antonio Open Data Portal](https://data.sanantonio.gov/)

## Methodology
1. **Cleaning:** Handled null values and categorized 911 codes into 6 priority groups.
2. **Feature Engineering:** Extracted timestamps to compare Day vs. Night trends.
3. **Visualization:** Developed 5-class manual legends to ensure accurate comparisons of high-volume medical calls vs. lower-volume fire hazards.

## Results

## Analysis by Service Area

### 1. Day vs. Night Call Volume (Service Area)
![Day vs Night Service Area](SATX_Area_Call_DayVsNight.png)
**Analytical Insight:** The temporal analysis reveals a massive surge in service demand during daylight hours. Specifically, the urban core and western service areas reach **Peak Volume (420K - 500K calls)** during the day. In contrast, night-shift activity shows a significant reduction in total volume, with the highest-activity zones peaking at only **340K - 420K calls**. This **20-25%** drop in peak volume suggests a high dependency on daytime traffic safety and public order incidents, providing critical data for staggered shift-scheduling and resource deployment.

---

### 2. Crime Category Comparison
![Crime Comparison](SATX_Area_Call_ViolentVsProperty.png)
**Analytical Insight:** A comparative breakdown of Violent vs. Property crime reveals a distinct inverse relationship in the northern jurisdictions. While Violent crime remains concentrated in the urban center, the **North** and **Prue** service areas experience a disproportionate volume of Property-related incidents—exceeding Violent crime counts by over **100,000 calls**. This divergence indicates that while personal safety risks are clustered centrally, asset-related risks are significantly more distributed into the residential and commercial corridors of the North.

---

### 3. Health & Fire Hazard Distribution
![Crime Comparison](SATX_Area_Call_HealthVsFire.png)
**Analytical Insight:** The volume disparity between Health and Fire service calls is stark, with Medical Assistance receiving approximately **28x more volume** than Fire/Environmental hazards. Despite the scale difference, spatial patterns remain consistent: the **South** service area is categorized as 'Peak Volume' for both incident types, marking it as a critical zone for emergency medical infrastructure. Conversely, the **Central** and **Downtown** districts show relatively low volumes for both categories, suggesting that daytime density in the core is driven more by administrative and traffic-related calls than by medical or environmental emergencies.

## Analysis by ZIP code

### 1. Day vs. Night Call Volume (Zip Code)
![Day vs Night Service Area](SATX_Zip_Call_DayVsNight.png)
**Analytical Insight:** Transitioning from Service Areas to Zip Codes reveals that daytime volume is heavily concentrated in the **78207 (West Side)** and **78201 (Central)** corridors, both exceeding **110K calls**. Interestingly, while night-time volume drops city-wide, these specific zip codes maintain a disproportionately high "High" or "Very High" status, suggesting that these areas require constant, 24/7 patrol saturation regardless of the temporal shift.

---

### 2. Crime Category Comparison
![Crime Comparison](SATX_Zip_Call_ViolentVsProperty.png)
**Analytical Insight:** While Property Crime is widely distributed across the northern and western suburbs, Violent Crime is tightly clustered in the **central and eastern zip codes**. The data shows a significant "volume gap" in the **78216 (North Central)** area, where Property Crime calls are nearly 3x more frequent than Violent Crime calls, likely due to the high density of retail and commercial assets in that sector.

---

### 3. Health & Fire Hazard Distribution
![Crime Comparison](SATX_Zip_Call_HealthVsFire.png)
**Analytical Insight:** While Medical Assistance calls outnumber Fire/Environmental calls by a nearly **28:1 margin**, the spatial distribution of these incidents is remarkably similar. Both categories show a heavy concentration in the **western and southern residential corridors**, specifically within the **78201** and **78228** zip codes, which fall into the **'Very High' volume tier**. The true **'Peak Volume'** hotspots are limited to the high-density urban core, indicating that while emergencies are city-wide, the most consistent demand for integrated medical and fire response infrastructure is centered in these established residential sectors(78207).
