# 📊 Dataset for "Unveiling Karachi's Air: A Scientific Foundation for a Clean Air City"
**DOI:** https://doi.org/10.5281/zenodo.15845428

**Cite this dataset as:**
Pakistan Air Quality Initiative (PAQI). (2025). *Air Quality Monitoring Data for Karachi (2016-2024) and Pakistan Environmental Standards* [Data set]. Zenodo. https://doi.org/10.5281/zenodo.15845428

---

### **📄 Description**

This dataset accompanies the policy report "Unveiling Karachi's Air: A Scientific Foundation for a Clean Air City," published by the Pakistan Air Quality Initiative (PAQI). It contains the foundational air quality monitoring data and the summary of environmental standards used in the report's analysis.

The abstract for the main report is as follows:
> Air pollution is a public health crisis in Karachi that shortens the life of an average resident by 2.7 years. On-the-ground monitoring reveals a city trapped in a cycle of hazardous air, with 363 out of 366 days in 2024 failing to meet the WHO's health-based guideline. On 70 of those days, pollution was so severe it also breached the legal limits set by the Sindh Environmental Protection Agency (SEPA). To address this crisis, the Pakistan Air Quality Initiative (PAQI) has developed the first comprehensive, scientific emissions inventory for Karachi. This report diagnoses the primary sources of this pollution, providing the indispensable evidence needed for effective action. The inventory, with a baseline year of 2021, quantifies a substantial pollution load, including 39.11 kilotons of health-damaging fine particulate matter (PM2.5) annually. Key findings pinpoint industrial activities as the largest source of PM2.5 (49%), while the transportation sector is the second-largest contributor (33%) and the overwhelming source of nitrogen oxides (NOx) at 80%. Power generation and port operations are also identified as major polluters. More than a diagnosis, this report is a blueprint for action. It demonstrates that Karachi's air pollution is not an intractable issue but is local, measurable, and solvable. It identifies a suite of priority interventions in industry, transport, and port operations that, if fully implemented, could reduce urban PM2.5 emissions by up to 50%. This research provides the scientific foundation for policymakers, industry, and civil society to collaboratively forge a path toward a healthier, more sustainable Karachi.

**📜 License:** Creative Commons Attribution 4.0 International (CC BY 4.0)

**🔑 Keywords:** Air Quality, Air Pollution, Emissions Inventory, PM2.5, Karachi, Pakistan, Environmental Standards, Public Health Policy, SEPA, PAQI

---

### **File Descriptions and Column Metadata**

This section serves as the data dictionary, explaining the contents of each file.

#### **File: `PAQI_Karachi_Daily_PM2.5_Data_2016-2024.csv`**
* **Description:** Contains the complete daily 24-hour average PM2.5 concentrations from the PAQI monitoring network.
* **Columns:**
    * `date`: The date of the measurement in `YYYY-MM-DD` format. (Data Type: Date)
    * `pm25_concentration_ug_per_m3`: The 24-hour average concentration of PM2.5. (Data Type: Number, Units: µg/m³)

#### **File: `PAQI_Karachi_PM2.5_Monthly_Averages_2016-2024.csv`**
* **Description:** Contains the monthly average PM2.5 concentrations calculated from the daily data.
* **Columns:**
    * `year`: The calendar year. (Data Type: Integer)
    * `month`: The calendar month (1-12). (Data Type: Integer)
    * `pm25_concentration_ug_per_m3`: The monthly average concentration of PM2.5. (Data Type: Number, Units: µg/m³)

#### **File: `PAQI_Karachi_PM2.5_Annual_Averages_2017-2024.csv`**
* **Description:** Contains the annual average PM2.5 concentrations calculated from the daily data.
* **Columns:**
    * `year`: The calendar year. (Data Type: Integer)
    * `pm25_concentration_ug_per_m3`: The annual average concentration of PM2.5. (Data Type: Number, Units: µg/m³)

#### **File: `PAQI_Frequency_of_Days_by_Air_Quality_Category_in_Karachi.csv`**
* **Description:** Summarizes the number of days per year falling into different air quality categories, based on applicable WHO and SEPA 24-hour PM2.5 guidelines.
* **Columns:**
    * `year`: The calendar year. (Data Type: Integer)
    * `days_within_who_guideline`: Number of days where the 24-hour PM2.5 average was within the applicable WHO guideline (≤25 µg/m³ for 2016-2021; ≤15 µg/m³ for 2022-2024). (Data Type: Integer)
    * `days_unhealthy_by_who_legal_by_sepa`: Number of days exceeding the WHO guideline but within the SEQS 24-hour limit of 75 µg/m³. (Data Type: Integer)
    * `days_exceeds_sepa_limit`: Number of days exceeding the SEQS 24-hour limit of 75 µg/m³. (Data Type: Integer)

#### **File: `PAQI_Air_Quality_Standards_Annual_Mean.csv`**
* **Description:** A reference table of annual mean ambient air quality standards.
* **Columns:**
    * `pollutant`: The name of the pollutant. (Data Type: String)
    * `neqs_2010_ug_per_m3` to `who_2021_ug_per_m3`: The standard limit for the respective authority and year. (Data Type: Number, Units: µg/m³)

#### **File: `PAQI_Short_Term_Mean_Ambient_Air_Quality_Standards.csv`**
* **Description:** A reference table of short-term (24h, 8h, 1h) ambient air quality standards.
* **Columns:**
    * `pollutant`: The name of the pollutant. (Data Type: String)
    * `averaging_period`: The time period for the standard (e.g., '24-hour'). (Data Type: String)
    * `unit`: The unit of measurement (e.g., 'µg/m³'). (Data Type: String)
    * `neqs_2010_value` to `who_2021_value`: The standard limit for the respective authority and year. (Data Type: Number)
