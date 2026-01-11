# City-Traffic-Accident-Safety-Analysis-using-Excel
 Trend Analysis:  Monthly/weekly accident counts;  Hotspot Detection:  flag top hotspots. Contributing Factors:  Cross-analyze accident type.  Severity Insights:  Distribution of Minor/Moderate/Severe/Fatal  Interactive Dashboard: Slicers for Location, Accident Type, Weather, Road Condition, Time period. Reporting:  KPIs, charts.
1. Data Prep & Cleaning
Remove duplicates; trim/case-standardize text columns 
Ensure Accident_Date is Date and Accident_Time is Time.
2. Calculated Columns (create a Table tblAccidents)
Convert cleaned data to an Excel Table (Ctrl+T) named tblAccidents, then add:
Functions Used:
DateTime
Month-Year
Year
DayOfWeek
Hour
RushHourFlag (Yes/No)
XLOOKUP()
3. Core KPIs (simple cells or Pivot measures)
COUNTA()
COUNTIFS()
AVERAGE()
Top Location (by count): use a Pivot or INDEX+XMATCH on a location frequency table.
4. Pivot Tables and Slicers
A. Trend Pivot (Accidents over Time)
B. Hotspot Pivot (Locations)
C. Factors Pivot (Cause vs Conditions)
D. Severity Distribution
E. Time-of-Day / Hour Analysis
F. Vehicles vs Severity (optional)
5. Charts & Dashboard (sheet “Dashboard”)
Line: Monthly accidents trend (from Trend Pivot).
Clustered Bar: Top 10 locations (from Hotspot Pivot).
Stacked Column or Heatmap: Accident_Type by Weather_Condition.
Donut/Pie: Severity distribution.
Column: Hour-of-day accident counts.
KPI Cards: Total Accidents, Fatal %, Avg Severity Index, Top Location.
 Data Dictionary sheet describing each column and derived field.
