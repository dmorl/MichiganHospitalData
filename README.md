## Michigan Hospital Overview Tracking

-------------------------------------------

Author: Daria Orlowska <br />
Contact: daria.orlowska@wmich.edu <br />
Last Updated: 2020-06-30 11:40 <br />

-------------------------------------------

Source: Data is found under the Cumulative Data link of Michigan's Coronavirus webpage, under the link "Data About Places", under the url https://www.michigan.gov/coronavirus/0,9753,7-406-98159-523641--,00.html <br />
Description: Tabular data of Statewide Available PPE and Bed Tracking <br />
Date range: 2020-04-02 through 2020-06-29 <br />
Missing dates: 2020-04-07, 2020-05-04, 2020-05-09, 2020-05-16, 2020-05-17, 2020-05-25  <br />
**NOTE: As of 2020-05-18, data on the website will now be updated Monday - Friday due to furloughs**

Author notes: Tables were released without variable descriptions. If Author felt confident about a new variable being a name change, tracking remained in same column and is noted in the "Note" field. When Author was uncertain if newly introduced variables were a name change or just a new way of tracking, a new column was added in the spreadsheet.

---

### REGIONS

Description: Data is aggregated using the Healthcare Coalition Regions: https://www.michigan.gov/mdhhs/0,5885,7-339-71548_54783_54826_56171-237197--,00.html#hcc <br />
Author notes: Counties provided below. The City of Detroit is contained within Wayne county. Region #4 does not exist.

1 – Clinton, Eaton, Gratiot, Hillsdale, Ingham, Jackson, Lenawee, Livingston, Shiawassee <br />
2S – Monroe, Washtenaw, Wayne <br />
2N - Macomb, Oakland, St Clair <br />
3 - Saginaw, Alcona, Iosco, Ogemaw, Arenac, Gladwin, Midland, Bay, Genesee, Tuscola, Lapeer, Sanilac, Huron <br />
5 - Allegan, Barry, Calhoun, Branch, St. Joseph, Cass, Berrien, Van Buren, Kalamazoo <br />
6 - Clare, Ionia, Isabella, Kent, Lake, Mason, Mecosta, Montcalm, Muskegon, Newaygo, Oceana, Osceola, Ottawa <br />
7 - Manistee, Wexford, Missaukee, Roscommon, Benzie, Leelanau, Grand Traverse, Kalkaska, Crawford, Oscoda, Antrim, Otsego, Montmorency, Alpena, Presque Ilse, Cheboygan, Emmet, Charlevoix <br />
8 - Chippewa, Mackinac, Luce, Schoolcraft, Delta, Alger, Marquette, Dickinson, Menominee, Baraga, Iron, Gogebic, Ontonagon, Houghton, Keweenaw <br />

---

### VARIABLES

Date
* Column: A
* Description: Date of report in format YYYY-MM-DD, contained within the first table title, Statewide Available Bed Tracking for COVID-19
* Values: Date
* Missing values reason: This value should never be missing

Region
* Column: B
* Description: Michigan Healthcare Coalition Regions
* Values: String
* Missing values reason: This value should never be missing <br />
Unique values: 1, 2S, 2N, 3, 5, 6, 7, 8 <br />
Note: See REGIONS section above for what counties are classified into each region

Bed_TOT
* Column: C
* Description: Data from the Statewide Available Bed Tracking for COVID-19 table, variable "Total Number of Hospital Beds" (see Note)
* Values: Integer
* DateRange: 2020-04-02 through xxxx-xx-xx
* Missing values reason: This value may be missing if it is not provided in the report <br />
Note: Appears as "Total Beds" between 2020-04-02 through 2020-04-15 ("Total Bed Capicity" on 2020-04-05), "Total Number of Hospital Beds" on 2020-04-16 onward

CriticalCare
* Column: D
* Description: Data from the Statewide Available Bed Tracking for COVID-19 table, variable "Critical Care"
* Values: Integer
* DateRange: 2020-04-02 through 2020-04-03
* Missing values reason: This value may be missing if it is not provided in the report <br />
Note: Possibly reorganized into the COVID-19 Metrics table as "# In Critical Care" (see variable Inpatients_Crit)

ED
* Column: E
* Description: Data from the Statewide Available Bed Tracking for COVID-19 table, variable "Hospital Inpatient Beds" (see Note)
* Values: Integer
* DateRange: 2020-04-02 through xxxx-xx-xx
* Missing values reason: This value may be missing if it is not provided in the report <br />
Note: Appears as "Emergency Dept." on 2020-04-02 and 2020-04-03, then as "Emergency Department" on 2020-04-04 until 2020-04-15, and then as "Hospital Inpatient Beds" from 2020-04-16 onward

ED_Used
* Column: F
* Description: Data from the Statewide Available Bed Tracking for COVID-19 table, variable "Hospital Inpatient Beds Occupancy"
* Values: Integer
* DateRange: 2020-04-16 through xxxx-xx-xx
* Missing values reason: This value may be missing if it is not provided in the report

ICU
* Column: G
* Description: Data from the Statewide Available Bed Tracking for COVID-19 table, variable "ICU Beds" (see Note)
* Values: Integer
* DateRange: 2020-04-02 through xxxx-xx-xx
* Missing values reason: This value may be missing if it is not provided in the report <br />
Note: Appears as "Adult ICU" on 2020-04-02 until 2020-04-15, and then as "ICU Beds" from 2020-04-16 onward

ICU_Used
* Column: H
* Description: Data from the Statewide Available Bed Tracking for COVID-19 table, variable "ICU Bed Occupancy"
* Values: Integer
* DateRange: 2020-04-16 through xxxx-xx-xx
* Missing values reason: This value may be missing if it is not provided in the report

BurnCare
* Column: I
* Description: Data from the Statewide Available Bed Tracking for COVID-19 table, variable "Available Burn Care" (see Note)
* Values: Integer
* DateRange: 2020-04-02 through xxxx-xx-xx
* Missing values reason: This value may be missing if it is not provided in the report <br />
Note: Appears as "Burn Care" on 2020-04-02 through 2020-04-15, and then as "Available Burn Care" from 2020-04-16 onward

MedSurg
* Column: J
* Description: Data from the Statewide Available Bed Tracking for COVID-19 table, variable "Available Adult MedSurg" (see Note)
* Values: Integer
* DateRange: 2020-04-02 through xxxx-xx-xx
* Missing values reason: This value may be missing if it is not provided in the report <br />
Note: Appears as "Adult Medical/Surgical Unit" on 2020-04-02 and 2020-04-03, then as "Adult Med Surg"/"Adult MedSurg" on 2020-04-04 until 2020-04-15, and then as "Available Adult MedSurg" from 2020-04-16 onward

Obstetric
* Column: K
* Description: Data from the Statewide Available Bed Tracking for COVID-19 table, variable "Obstetric"
* Values: Integer
* DateRange: 2020-04-02 through 2020-04-15
* Missing values reason: This value may be missing if it is not provided in the report

OR
* Column: L
* Description: Data from the Statewide Available Bed Tracking for COVID-19 table, variable "Available Operating Room" (see Note)
* Values: Integer
* DateRange: 2020-04-02 through xxxx-xx-xx
* Missing values reason: This value may be missing if it is not provided in the report <br />
Note: Appears as "Operating Room" on 2020-04-02 through 2020-04-15, and then as "Available Operating Room" from 2020-04-16 onward

Pediatric
* Column: M
* Description: Data from the Statewide Available Bed Tracking for COVID-19 table, variable "Available Pediatric" (see Note)
* Values: Integer
* DateRange: 2020-04-02 through xxxx-xx-xx
* Missing values reason: This value may be missing if it is not provided in the report <br />
Note: Appears as "Pediatric" on 2020-04-02 through 2020-04-15, and then as "Available Pediatric" from 2020-04-16 onward

PediatricICU
* Column: N
* Description: Data from the Statewide Available Bed Tracking for COVID-19 table, variable "Pediatric ICU"
* Values: Integer
* DateRange: 2020-04-02 through 2020-04-15
* Missing values reason: This value may be missing if it is not provided in the report

Psychiatric
* Column: O
* Description: Data from the Statewide Available Bed Tracking for COVID-19 table, variable "Available Psychiatric" (see Note)
* Values: Integer
* DateRange: 2020-04-02 through xxxx-xx-xx
* Missing values reason: This value may be missing if it is not provided in the report <br />
Note: Appears as "Psychiatric" on 2020-04-02 through 2020-04-15, and then as "Available Psychiatric" from 2020-04-16 onward

Morgue_Avail
* Column: P
* Description: Data from the Statewide Available Bed Tracking for COVID-19 table, variable "Morgue Availability" (see Note)
* Values: Integer
* DateRange: 2020-04-02 through xxxx-xx-xx
* Missing values reason: This value may be missing if it is not provided in the report

Morgue_TOT
* Column: Q
* Description: Data from the Statewide Available Bed Tracking for COVID-19 table, variable "Total Morgue Capacity"
* Values: Integer
* DateRange: 2020-04-16 through xxxx-xx-xx
* Missing values reason: This value may be missing if it is not provided in the report

NegPress_Avail
* Column: R
* Description: Data from the Statewide Available Bed Tracking for COVID-19 table, variable "Negative Pressure Isolation Available"
* Values: Integer
* DateRange: 2020-04-02 through xxxx-xx-xx
* Missing values reason: This value may be missing if it is not provided in the report

NegPress_TOT
* Column: S
* Description: Data from the Statewide Available Bed Tracking for COVID-19 table, variable "Negative Pressure Isolation Total" (see Note)
* Values: Integer
* DateRange: 2020-04-02 through xxxx-xx-xx
* Missing values reason: This value may be missing if it is not provided in the report <br />
Note: Appears as "Bed Capacity: Neg Pressure Isolation" on 2020-04-02 through 2020-04-14, and as "Negative Pressure Isolation Total" 2020-04-15 onward

MechVent_Used
* Column: T
* Description: Data from the Statewide Available Bed Tracking for COVID-19 table, variable "Mechanical Ventilators in Use"
* Values: Integer
* DateRange: 2020-04-16 through 2020-04-18
* Missing values reason: This value may be missing if it is not provided in the report

MechVent
* Column: U
* Description: Data from the Statewide Available Bed Tracking for COVID-19 table, variable "Mechanical Ventilators"
* Values: Integer
* DateRange: 2020-04-16 through xxxx-xx-xx
* Missing values reason: This value may be missing if it is not provided in the report <br />
Note: Possibly a replacement for Statewide Available Bed Tracking for COVID-19 table, variable "Total Ventilators" (see variable Vent_TOT), because MechVent is only reported when Vent_TOT stops being reported

Vent_Avail
* Column: V
* Description: Data from the Statewide Available Bed Tracking for COVID-19 table, variable "Available Ventilators" (see Note)
* Values: Integer
* DateRange: 2020-04-02 through xxxx-xx-xx
* Missing values reason: This value may be missing if it is not provided in the report <br />
Note: Appears as "Ventilators Not in Use" from 2020-04-02 to 2020-04-10, then as "Available Ventilators" on 2020-04-11 onwards

Vent_TOT
* Column: W
* Description: Data from the Statewide Available Bed Tracking for COVID-19 table, variable "Total Ventilators"
* Values: Integer
* DateRange: 2020-04-04 through xxxx-xx-xx
* Missing values reason: This value may be missing if it is not provided in the report

Inpatients
* Column: X
* Description: Data from the COVID-19 Metrics table, variable "# of Inpatients" (see Note)
* Values: Integer
* DateRange: 2020-04-08 through xxxx-xx-xx
* Missing values reason: This value may be missing if it is not provided in the report <br />
Note: Appears as "COVID Inpatients" in the COVID-19 Capacity Metrics table on 2020-04-08, then as "# of Inpatients" in the COVID-19 Metrics table on 2020-04-09 onwards

Inpatients_Crit
* Column: Y
* Description: Data from the COVID-19 Metrics table, variable "# in Critical Care" (see Note)
* Values: Integer
* DateRange: 2020-04-08 through xxxx-xx-xx
* Missing values reason: This value may be missing if it is not provided in the report <br />
Note: Appears as "COVID Inpatients in Critical Care" in the COVID-19 Capacity Metrics table on 2020-04-08, then as "# in Critical Care" in the COVID-19 Metrics table on 2020-04-09 onwards

Inpatients_Vent
* Column: Z
* Description: Data from the COVID-19 Metrics table, variable "# on Ventilators" (see Note)
* Values: Integer
* DateRange: 2020-04-08 through xxxx-xx-xx
* Missing values reason: This value may be missing if it is not provided in the report <br />
Note: Appears as "COVID Inpatients on Ventilators" in the COVID-19 Capacity Metrics table on 2020-04-08, then as "# on Ventilators" in the COVID-19 Metrics table on 2020-04-09 onwards

Inpatients_Dis
* Column: AA
* Description: Data from the COVID-19 Metrics table, variable "# of ED Discharges" (see Note)
* Values: Integer
* DateRange: 2020-04-08 through xxxx-xx-xx
* Missing values reason: This value may be missing if it is not provided in the report <br />
Note: Appears as "COVID ED Discharges" in the COVID-19 Capacity Metrics table on 2020-04-08, then as "# of ED Discharges" in the COVID-19 Metrics table on 2020-04-09 onwards

Elasto_Filters
* Column: AB
* Description: Data from the Statewide Available PPE Tracking for COVID-19 table, variable "Elastomeric Respirator Filters"
* Values: Integer
* DateRange: 2020-04-11 through xxxx-xx-xx
* Missing values reason: This value may be missing if it is not provided in the report

Elasto_Resp
* Column: AC
* Description: Data from the Statewide Available PPE Tracking for COVID-19 table, variable "Elastomeric Respirator"
* Values: Integer
* DateRange: 2020-04-11 through xxxx-xx-xx
* Missing values reason: This value may be missing if it is not provided in the report

PAPR_Batteries
* Column: AD
* Description: Data from the Statewide Available PPE Tracking for COVID-19 table, variable "PAPR Batteries"
* Values: Integer
* DateRange: 2020-04-11 through xxxx-xx-xx
* Missing values reason: This value may be missing if it is not provided in the report

PAPR_Filters
* Column: AE
* Description: Data from the Statewide Available PPE Tracking for COVID-19 table, variable "PAPR Filters"
* Values: Integer
* DateRange: 2020-04-11 through xxxx-xx-xx
* Missing values reason: This value may be missing if it is not provided in the report

PAPRs
* Column: AF
* Description: Data from the Statewide Available PPE Tracking for COVID-19 table, variable "PAPRs"
* Values: Integer
* DateRange: 2020-04-11 through xxxx-xx-xx
* Missing values reason: This value may be missing if it is not provided in the report

CAPRs
* Column: AG
* Description: Data from the Statewide Available PPE Tracking for COVID-19 table, variable "CAPRs"
* Values: Integer
* DateRange: 2020-04-11 through xxxx-xx-xx
* Missing values reason: This value may be missing if it is not provided in the report

Gloves
* Column: AH
* Description: Data from the Statewide Available PPE Tracking for COVID-19 table, variable "Gloves"
* Values: Integer
* DateRange: 2020-04-02 through xxxx-xx-xx
* Missing values reason: This value may be missing if it is not provided in the report

Coveralls
* Column: AI
* Description: Data from the Statewide Available PPE Tracking for COVID-19 table, variable "Coveralls"
* Values: Integer
* DateRange: 2020-04-02 through xxxx-xx-xx
* Missing values reason: This value may be missing if it is not provided in the report

Isolation_Gowns
* Column: AJ
* Description: Data from the Statewide Available PPE Tracking for COVID-19 table, variable "Surgical Isolation Gowns"
* Values: Integer
* DateRange: 2020-04-02 through xxxx-xx-xx
* Missing values reason: This value may be missing if it is not provided in the report

Surgical_Gowns
* Column: AK
* Description: Data from the Statewide Available PPE Tracking for COVID-19 table, variable "Surgical Gowns"
* Values: Integer
* DateRange: 2020-04-02 through xxxx-xx-xx
* Missing values reason: This value may be missing if it is not provided in the report

Surgical_Masks
* Column: AL
* Description: Data from the Statewide Available PPE Tracking for COVID-19 table, variable "Surgical Masks Facemasks"
* Values: Integer
* DateRange: 2020-04-02 through xxxx-xx-xx
* Missing values reason: This value may be missing if it is not provided in the report

N95_Masks
* Column: AM
* Description: Data from the Statewide Available PPE Tracking for COVID-19 table, variable "N95 Respirator Masks"
* Values: Integer
* DateRange: 2020-04-02 through xxxx-xx-xx
* Missing values reason: This value may be missing if it is not provided in the report

Shields
* Column: AN
* Description: Data from the Statewide Available PPE Tracking for COVID-19 table, variable "Face Shields"
* Values: Integer
* DateRange: 2020-04-03 through xxxx-xx-xx
* Missing values reason: This value may be missing if it is not provided in the report

Goggles
* Column: AO
* Description: Data from the Statewide Available PPE Tracking for COVID-19 table, variable "Goggles"
* Values: Integer
* DateRange: 2020-04-03 through xxxx-xx-xx
* Missing values reason: This value may be missing if it is not provided in the report

Reporting_Bed
* Column: AP
* Description: Total response rate for the Statewide Available Bed Tracking for COVID-19 table
* Values: Percentage
* Missing values reason: This value may be missing if it is not provided in the report

Reporting_PPE
* Column: AQ
* Description: Total response rate for the Statewide Available PPE Tracking for COVID-19 table
* Values: Percentage
* Missing values reason: This value may be missing if it is not provided in the report

Notes
* Column: AR
* Description: Additional notes provided underneath the tables
* Values: String
* Missing values reason: This value may be missing if it is not provided in the report

Link
* Column: AS
* Description: Link to the archival version of the tabular data, through the Wayback Machine Internet Archive
* Values: URL
* Missing values reason: This value may be missing if it is not provided in the report
