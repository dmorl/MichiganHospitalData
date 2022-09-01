# Michigan Hospital Overview Tracking

-------------------------------------------

**Author:** Daria Orlowska <br />
**Contact:** daria.orlowska@wmich.edu <br />
**Last Updated:** 2022-09-01 11:46 <br />

-------------------------------------------

## Spreadsheet Overviews

### MichiganOverview_HospitalTracking.csv

**Source:** Data is found under the Cumulative Data link of Michigan's Coronavirus webpage, under the link "Hospital", under the url https://www.michigan.gov/coronavirus/stats/data-about-places/statewide-available-ppe-and-bed-tracking (previously under the url https://www.michigan.gov/coronavirus/0,9753,7-406-98159-523641--,00.html) <br />
**Description:** Tabular data from the first three tables, Statewide Hospital Capacity Report for COVID-19, COVID-19 Metrics, and Statewide Hospital Avaiable PPE Tracking for COVID-19, contained within Statewide Available PPE and Bed Tracking <br />
**Date range:** 2020-04-02 through 2022-08-31 <br />
**Missing dates:** 2020-04-07, 2020-05-04, 2020-05-09, 2020-05-16, 2020-05-17, 2020-05-25, 2020-07-03, 2020-08-04, 2020-08-07, 2020-11-26, 2020-12-24, 2020-12-25, 2020-12-31, 2021-01-01, 2021-11-26 <br />

**Website notes:** 2020-8-19: Changes have recently been made to the clinical variables shared on the MDHHS website. These changes were made to align with the new reporting requirements from the federal government. To better accommodate all users of this data, MDHHS is expanding the data provided from the previous clinical variables section to the information described in the new clinical variables section. Data users should carefully consider which variables meet their current or ongoing needs for information
**Author notes:** Tables were released without variable descriptions. If Author felt confident about a new variable being a name change, tracking remained in same column and is noted in the "Note" field. When Author was uncertain if newly introduced variables were a name change or just a new way of tracking, a new column was added in the spreadsheet.
As of 2020-08-05, the first table "Statewide Available Bed Tracking for COVID-19" has changed names to "Statewide Hospital Capacity Report for COVID-19". The reintroduction, addition and omission of variables has lead to the structure of the dataset changing. As of 2020-08-06, the table Statewide Hospital Available PPE Tracking for COVID-19 has underwent reorganization, with some variables now being reported in aggregate. On 2020-08-11, and again on 2020-08-19, the table COVID-19 Metrics has underwent reorganization.
As of 2021-02-03, the table Statewide Hospital Available PPE Tracking for COVID-19 will only be updated every Wednesday.
As of 2021-07-02, COVID data will be posted twice a week on Tuesdays and Fridays.
As of 2021-08-09, COVID case and testing data will be posted three times a week on Mondays, Wednesdays and Friday.
As of 2022-04-22, the website url was updated to https://www.michigan.gov/coronavirus/stats/data-about-places/statewide-available-ppe-and-bed-tracking

### MichiganOverview_HospitalTracking_PatientCensus.csv

**Source:** Data is found under the Cumulative Data link of Michigan's Coronavirus webpage, under the link "Hospital", under the url https://www.michigan.gov/coronavirus/stats/data-about-places/statewide-available-ppe-and-bed-tracking (previously under the url  https://www.michigan.gov/coronavirus/0,9753,7-406-98159-523641--,00.html) <br />
**Description:** Totals from the table "Patient Census", contained within Statewide Available PPE and Bed Tracking <br />
**Date range:** 2020-04-23 through 2022-07-26 <br />

**Website notes:** This information has been compiled by the Michigan Health & Hospital Association (MHA) on behalf of the Michigan Department
of Health & Human Services (MDHHS). The data is from the state of Michigan's EMResource data system. Hospitals are required
to enter data into EMResource. The data reflects the status in the hospital or health system from the previous 48 hour period.
The information is aggregated by health system for those hospitals that are part of a health system. This is because systems are
centrally tracking and distributing personal protection equipment (PPE) amongst their various facilities and looking at patient
surge and load from a system perspective. Non-system hospitals are identified as individual hospitals.
The data reflects the status in health systems and hospitals 48 hours prior to the time that the data was posted to this website.
https://public.tableau.com/profile/mhapublic#!/vizhome/COVIDPublicDashboard/PleaseRead

**Author notes:** This information is not being updated on a regular schedule. It is usually updated on Mondays.
As of 2022-04-22, the website url was updated to https://www.michigan.gov/coronavirus/stats/data-about-places/statewide-available-ppe-and-bed-tracking

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

## Spreadsheet Variables

### MichiganOverview_HospitalTracking.csv

Date
* Column: A
* Description: Date of report in format YYYY-MM-DD, contained within the first table title, Statewide Hospital Capacity Report for COVID-19
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
* Description: Data from the Statewide Hospital Capacity Report for COVID-19 for COVID-19 table, variable "Hospital Beds" (see Note)
* Values: Integer
* DateRange: 2020-04-02 through xxxx-xx-xx
* Missing values reason: This value may be missing if it is not provided in the report <br />
Note: Appears as "Total Beds" between 2020-04-02 through 2020-04-15 ("Total Bed Capacity" on 2020-04-05), "Total Number of Hospital Beds" on 2020-04-16 through 2020-08-03, and "Hospital Beds" 2020-08-05 onward

BedAdult_TOT
* Column: D
* Description: Data from the Statewide Hospital Capacity Report for COVID-19 table, variable "Adult Hospital Beds" (see Note)
* Values: Integer
* DateRange: 2020-08-05 through xxxx-xx-xx
* Missing values reason: This value may be missing if it is not provided in the report <br />

CriticalCare
* Column: E
* Description: Data from the Statewide Available Bed Tracking for COVID-19 table, variable "Critical Care"
* Values: Integer
* DateRange: 2020-04-02 through 2020-04-03
* Missing values reason: This value may be missing if it is not provided in the report <br />
Note: Possibly reorganized into the COVID-19 Metrics table as "# In Critical Care" (see variable Inpatients_Crit)

ED
* Column: F
* Description: Data from the Statewide Available Bed Tracking for COVID-19 table, variable "Emergency Department" (see Note)
* Values: Integer
* DateRange: 2020-04-02 through 2020-04-15
* Missing values reason: This value may be missing if it is not provided in the report <br />
Note: Appears as "Emergency Dept." on 2020-04-02 and 2020-04-03, then as "Emergency Department" on 2020-04-04 until 2020-04-15

Inpatient
* Column: G
* Description: Data from the Statewide Hospital Capacity Report for COVID-19 table, variable "Hospital Inpatient Beds"
* Values: Integer
* DateRange: 2020-04-16 through xxxx-xx-xx
* Missing values reason: This value may be missing if it is not provided in the report <br />

Inpatient_Used
* Column: H
* Description: Data from the Statewide Hospital Capacity Report for COVID-19 table, variable "Hospital Inpatient Bed Occupancy"
* Values: Integer
* DateRange: 2020-04-16 through xxxx-xx-xx
* Missing values reason: This value may be missing if it is not provided in the report

InpatientAdult
* Column: I
* Description: Data from the Statewide Hospital Capacity Report for COVID-19 table, variable "Adult Hospital Inpatient Beds"
* Values: Integer
* DateRange: 2020-08-05 through xxxx-xx-xx
* Missing values reason: This value may be missing if it is not provided in the report <br />

InpatientAdult_Used
* Column: J
* Description: Data from the Statewide Hospital Capacity Report for COVID-19 table, variable "Adult Hospital Inpatient Bed Occupancy"
* Values: Integer
* DateRange: 2020-08-05 through xxxx-xx-xx
* Missing values reason: This value may be missing if it is not provided in the report

ICU
* Column: K
* Description: Data from the Statewide Hospital Capacity Report for COVID-19 table, variable "ICU Beds" (see Note)
* Values: Integer
* DateRange: 2020-04-16 through xxxx-xx-xx
* Missing values reason: This value may be missing if it is not provided in the report <br />

ICU_Used
* Column: L
* Description: Data from the Statewide Hospital Capacity Report for COVID-19 table, variable "ICU Bed Occupancy"
* Values: Integer
* DateRange: 2020-04-16 through xxxx-xx-xx
* Missing values reason: This value may be missing if it is not provided in the report

ICUAdult
* Column: M
* Description: Data from the Statewide Hospital Capacity Report for COVID-19 for COVID-19 table, variable "Adult ICU Beds" (see Note)
* Values: Integer
* DateRange: 2020-04-02 through 2020-04-15 and 2020-08-05 through 2022-01-28
* Missing values reason: This value may be missing if it is not provided in the report <br />
Note: Appeared as "Adult ICU" between 2020-04-02 through 2020-04-15, and then was reintroduced as "Adult ICU Beds" on 2020-08-05

ICUAdult_Used
* Column: N
* Description: Data from the Statewide Hospital Capacity Report for COVID-19 for COVID-19 table, variable "Adult ICU Bed Occupancy" (see Note)
* Values: Integer
* DateRange: 2020-08-05 through 2022-01-28
* Missing values reason: This value may be missing if it is not provided in the report <br />

BurnCare
* Column: O
* Description: Data from the Statewide Available Bed Tracking for COVID-19 table, variable "Available Burn Care" (see Note)
* Values: Integer
* DateRange: 2020-04-02 through 2020-08-03
* Missing values reason: This value may be missing if it is not provided in the report <br />
Note: Appears as "Burn Care" on 2020-04-02 through 2020-04-15, and then as "Available Burn Care" from 2020-04-16 onward

MedSurg
* Column: P
* Description: Data from the Statewide Available Bed Tracking for COVID-19 table, variable "Available Adult MedSurg" (see Note)
* Values: Integer
* DateRange: 2020-04-02 through 2020-08-03
* Missing values reason: This value may be missing if it is not provided in the report <br />
Note: Appears as "Adult Medical/Surgical Unit" on 2020-04-02 and 2020-04-03, then as "Adult Med Surg"/"Adult MedSurg" on 2020-04-04 until 2020-04-15, and then as "Available Adult MedSurg" from 2020-04-16 onward

Obstetric
* Column: Q
* Description: Data from the Statewide Available Bed Tracking for COVID-19 table, variable "Obstetric"
* Values: Integer
* DateRange: 2020-04-02 through 2020-04-15
* Missing values reason: This value may be missing if it is not provided in the report

OR
* Column: R
* Description: Data from the Statewide Available Bed Tracking for COVID-19 table, variable "Available Operating Room" (see Note)
* Values: Integer
* DateRange: 2020-04-02 through 2020-08-03
* Missing values reason: This value may be missing if it is not provided in the report <br />
Note: Appears as "Operating Room" on 2020-04-02 through 2020-04-15, and then as "Available Operating Room" from 2020-04-16 onward

InpatientPediatric
* Column: S
* Description: Data from the Statewide Hospital Available PPE Tracking for COVID-19 table, variable "All Inpatient Pediatric Beds" (see Note)
* Values: Integer
* DateRange: 2020-04-02 through 2020-08-03 and 2022-01-31 through xxxx-xx-xx
* Missing values reason: This value may be missing if it is not provided in the report <br />
Note: Appears as "Pediatric" on 2020-04-02 through 2020-04-15, and then as "Available Pediatric" from 2020-04-16 onward. As of 2022-01-31, this variable reappeared as "All Inpatient Pediatric Beds"

InpatientPediatric_Used
* Column: T
* Description: Data from the Statewide Hospital Available PPE Tracking for COVID-19 table, variable "Pediatric Inpatient Bed Occupancy"
* Values: Integer
* DateRange: 2022-01-31 through xxxx-xx-xx
* Missing values reason: This value may be missing if it is not provided in the report <br />

PediatricICU
* Column: U
* Description: Data from the Statewide Available Bed Tracking for COVID-19 table, variable "Pediatric ICU"
* Values: Integer
* DateRange: 2020-04-02 through 2020-04-15
* Missing values reason: This value may be missing if it is not provided in the report

Psychiatric
* Column: V
* Description: Data from the Statewide Available Bed Tracking for COVID-19 table, variable "Available Psychiatric" (see Note)
* Values: Integer
* DateRange: 2020-04-02 through 2020-08-03
* Missing values reason: This value may be missing if it is not provided in the report <br />
Note: Appears as "Psychiatric" on 2020-04-02 through 2020-04-15, and then as "Available Psychiatric" from 2020-04-16 onward

Morgue_Avail
* Column: W
* Description: Data from the Statewide Available Bed Tracking for COVID-19 table, variable "Morgue Availability" (see Note)
* Values: Integer
* DateRange: 2020-04-02 through 2020-08-03
* Missing values reason: This value may be missing if it is not provided in the report

Morgue_TOT
* Column: X
* Description: Data from the Statewide Available Bed Tracking for COVID-19 table, variable "Total Morgue Capacity"
* Values: Integer
* DateRange: 2020-04-16 through 2020-08-03
* Missing values reason: This value may be missing if it is not provided in the report

NegPress_Avail
* Column: Y
* Description: Data from the Statewide Available Bed Tracking for COVID-19 table, variable "Negative Pressure Isolation Available"
* Values: Integer
* DateRange: 2020-04-02 through 2020-08-03
* Missing values reason: This value may be missing if it is not provided in the report

NegPress_TOT
* Column: Z
* Description: Data from the Statewide Available Bed Tracking for COVID-19 table, variable "Negative Pressure Isolation Total" (see Note)
* Values: Integer
* DateRange: 2020-04-02 through 2020-08-03
* Missing values reason: This value may be missing if it is not provided in the report <br />
Note: Appears as "Bed Capacity: Neg Pressure Isolation" on 2020-04-02 through 2020-04-14, and as "Negative Pressure Isolation Total" 2020-04-15 onward

MechVent_Used
* Column: AA
* Description: Data from the Statewide Hospital Capacity Report for COVID-19 table, variable "Mechanical Ventilators in Use"
* Values: Integer
* DateRange: 2020-04-16 through 2020-04-18 and 2020-08-05 through 2021-07-30
* Missing values reason: This value may be missing if it is not provided in the report

MechVent
* Column: AB
* Description: Data from the Statewide Available Bed Tracking for COVID-19 table, variable "Mechanical Ventilators"
* Values: Integer
* DateRange: 2020-04-16 through 2020-04-26
* Missing values reason: This value may be missing if it is not provided in the report <br />
Note: Possibly a replacement for Statewide Available Bed Tracking for COVID-19 table, variable "Total Ventilators" (see variable Vent_TOT), because MechVent is only reported when Vent_TOT stops being reported

Vent_Avail
* Column: AC
* Description: Data from the Statewide Available Bed Tracking for COVID-19 table, variable "Available Ventilators" (see Note)
* Values: Integer
* DateRange: 2020-04-02 through 2020-08-03
* Missing values reason: This value may be missing if it is not provided in the report <br />
Note: Appears as "Ventilators Not in Use" from 2020-04-02 to 2020-04-10, then as "Available Ventilators" on 2020-04-11 onwards

Vent_TOT
* Column: AD
* Description: Data from the Statewide Hospital Capacity Report for COVID-19 table, variable "Total Ventilators"
* Values: Integer
* DateRange: 2020-04-04 through 2021-07-30
* Missing values reason: This value may be missing if it is not provided in the report

NumInpatients
* Column: AE
* Description: Data from the COVID-19 Metrics table, variable "# of Inpatients" (see Note)
* Values: Integer
* DateRange: 2020-04-08 through 2020-08-03
* Missing values reason: This value may be missing if it is not provided in the report <br />
Website note: The total number of positive tests for COVID-19 among admitted patients  <br /> 
Note: Appears as "COVID Inpatients" in the COVID-19 Capacity Metrics table on 2020-04-08, then as "# of Inpatients" in the COVID-19 Metrics table on 2020-04-09 onwards. This variable is potentially represented by the sum of new variables "AdultCases_TOT_pos" and "PedCases_TOT_pos"

NumInpatients_Crit
* Column: AF
* Description: Data from the COVID-19 Metrics table, variable "# in Critical Care" (see Note)
* Values: Integer
* DateRange: 2020-04-08 through 2020-08-03
* Missing values reason: This value may be missing if it is not provided in the report <br />
Website note: The CURRENT number of patients in critical care units with suspected or confirmed COVID-19. INCLUDE non-critical care areas being used for surge critical care. DO NOT INCLUDE ED boarding/overflow (patients currently admitted and awaiting bed).  <br /> 
Note: Appears as "COVID Inpatients in Critical Care" in the COVID-19 Capacity Metrics table on 2020-04-08, then as "# in Critical Care" in the COVID-19 Metrics table on 2020-04-09 onwards

NumInpatients_Vent
* Column: AG
* Description: Data from the COVID-19 Metrics table, variable "# on Ventilators" (see Note)
* Values: Integer
* DateRange: 2020-04-08 through 2020-08-03
* Missing values reason: This value may be missing if it is not provided in the report <br />
Website note: The CURRENT number of patients receiving mechanical ventilation with suspected or confirmed COVID-19. DO NOT INCLUDE ED boarding/overflow (patients currently admitted and awaiting bed) and surge critical care areas.  <br /> 
Note: Appears as "COVID Inpatients on Ventilators" in the COVID-19 Capacity Metrics table on 2020-04-08, then as "# on Ventilators" in the COVID-19 Metrics table on 2020-04-09 onwards

NumInpatients_Dis
* Column: AH
* Description: Data from the COVID-19 Metrics table, variable "# of ED Discharges" (see Note)
* Values: Integer
* DateRange: 2020-04-08 through 2020-08-03
* Missing values reason: This value may be missing if it is not provided in the report <br />
Website note: The number of patients discharged home (or equivalent) from ED with suspected or confirmed COVID-19 in past 24 hours. INCLUDE hospital urgent care and ED drive through <br /> 
Note: Appears as "COVID ED Discharges" in the COVID-19 Capacity Metrics table on 2020-04-08, then as "# of ED Discharges" in the COVID-19 Metrics table on 2020-04-09 onwards

AdultCases_TOT
* Column: AI
* Description: Data from the COVID-19 Metrics table, variable "Total Adult Suspected/Confirmed"
* Values: Integer
* DateRange: 2020-08-11 through xxxx-xx-xx
* Missing values reason: This value may be missing if it is not provided in the report <br />
Website note: Patients currently hospitalized in an adult inpatient bed who have laboratory-confirmed or suspected COVID-19. Patients in observation beds are included

AdultCases_TOT_pos
* Column: AJ
* Description: Data from the COVID-19 Metrics table, variable "Adult Confirmed-Positive COVID"
* Values: Integer
* DateRange: 2020-08-19 through xxxx-xx-xx
* Missing values reason: This value may be missing if it is not provided in the report <br />
Website note: Patients currently hospitalized in an adult inpatient bed who have laboratory-confirmed COVID-19. Patients in observation beds are included  <br />
Note: Potentially can be summed with the variable "PedCases_TOT_pos" to obtain a continuation of the variable "NumInpatients"

PedCases_TOT
* Column: AK
* Description: Data from the COVID-19 Metrics table, variable "Hospitalized Peds Confirmed/Suspected"
* Values: Integer
* DateRange: 2020-08-19 through xxxx-xx-xx
* Missing values reason: This value may be missing if it is not provided in the report <br />
Website note: Patients currently hospitalized in a pediatric inpatient bed, including NICU, newborn, and nursery, who are suspected or laboratory-confirmed-positive for COVID-19. Patients in observation beds are included  <br />
Author note: Website listed the description with the expanded variable name "Total hospitalized pediatric suspected or confirmed positive COVID patients", so author felt confident designating this variable as "TOT"

PedCases_TOT_pos
* Column: AL
* Description: Data from the COVID-19 Metrics table, variable "Adult Confirmed-Positive COVID"
* Values: Integer
* DateRange: 2020-08-19 through xxxx-xx-xx
* Missing values reason: This value may be missing if it is not provided in the report <br />
Website note: Patients currently hospitalized in a pediatric inpatient bed, including NICU, newborn, and nursery, who are laboratory-confirmed-positive for COVID-19. Patients in observation beds are included  <br />
Note: Potentially can be summed with the variable "AdultCases_TOT_pos" to obtain a continuation of the variable "NumInpatients"

VentedCases
* Column: AM
* Description: Data from the COVID-19 Metrics table, variable "Hospitalized and Vented COVID"
* Values: Integer
* DateRange: 2020-08-11 through xxxx-xx-xx
* Missing values reason: This value may be missing if it is not provided in the report <br />
Website note: Patients currently hospitalized in an adult, pediatric or neonatal inpatient bed who have suspected or laboratory-confirmed COVID-19 and are on a mechanical ventilator

AdultCases_ICU
* Column: AN
* Description: Data from the COVID-19 Metrics table, variable "Adult ICU Confirmed/Suspected COVID"
* Values: Integer
* DateRange: 2020-08-11 through xxxx-xx-xx
* Missing values reason: This value may be missing if it is not provided in the report <br />
Website note: Patients currently hospitalized in an adult ICU bed who have suspected or laboratory-confirmed COVID-19

AdultCases_ICU_pos
* Column: AO
* Description: Data from the COVID-19 Metrics table, variable "ICU Adult Confirmed-Positive COVID"
* Values: Integer
* DateRange: 2020-08-19 through xxxx-xx-xx
* Missing values reason: This value may be missing if it is not provided in the report <br />
Website note: Patients currently hospitalized in an adult ICU bed who have laboratory-confirmed COVID-19

EDCases_Prev
* Column: AP
* Description: Data from the COVID-19 Metrics table, variable "Prev Day COVID Related ED Visits"
* Values: Integer
* DateRange: 2020-08-11 through xxxx-xx-xx
* Missing values reason: This value may be missing if it is not provided in the report <br />
Website note: The total number of ED visits who were seen on the previous calendar day who had a visit related to COVID-19 (meets suspected or confirmed definition, or presents for COVID diagnostic testing). Patients presenting for pre-procedure screening are not counted

Elasto_Filters
* Column: AQ
* Description: Data from the Statewide Available PPE Tracking for COVID-19 table, variable "Elastomeric Respirator Filters"
* Values: Integer
* DateRange: 2020-04-11 through 2020-08-03
* Missing values reason: This value may be missing if it is not provided in the report

Elasto_Resp
* Column: AR
* Description: Data from the Statewide Available PPE Tracking for COVID-19 table, variable "Elastomeric Respirator"
* Values: Integer
* DateRange: 2020-04-11 through 2020-08-03
* Missing values reason: This value may be missing if it is not provided in the report <br />
Note: This variable may now be reported in the aggregate variable "Respirators_TOT"

PAPR_Batteries
* Column: AS
* Description: Data from the Statewide Available PPE Tracking for COVID-19 table, variable "PAPR Batteries"
* Values: Integer
* DateRange: 2020-04-11 through 2020-08-03
* Missing values reason: This value may be missing if it is not provided in the report

PAPR_Filters
* Column: AT
* Description: Data from the Statewide Available PPE Tracking for COVID-19 table, variable "PAPR Filters"
* Values: Integer
* DateRange: 2020-04-11 through 2020-08-03
* Missing values reason: This value may be missing if it is not provided in the report

PAPRs
* Column: AU
* Description: Data from the Statewide Available PPE Tracking for COVID-19 table, variable "PAPRs"
* Values: Integer
* DateRange: 2020-04-11 through 2020-08-03
* Missing values reason: This value may be missing if it is not provided in the report <br />
Note: This variable is now reported in the aggregate variable "Respirators_TOT"

CAPRs
* Column: AV
* Description: Data from the Statewide Available PPE Tracking for COVID-19 table, variable "CAPRs"
* Values: Integer
* DateRange: 2020-04-11 through 2020-08-03
* Missing values reason: This value may be missing if it is not provided in the report <br />
Note: This variable may now be reported in the aggregate variable "EyeProtect_TOT"

Respirators_TOT
* Column: AW
* Description: Data from the Statewide Available PPE Tracking for COVID-19 table, variable "PAPRS and Other Respirators On Hand"
* Values: Integer
* DateRange: 2020-08-06 through 2022-02-02
* Missing values reason: This value may be missing if it is not provided in the report <br />
Note: This variable may now aggregate previously reported variables "Elasto_Resp" and "PAPRs". Appeared as "PAPR/Other Respirators" between 2020-08-06 through 2021-07-16, and "PAPRS and Other Respirators On Hand" from 2021-08-11 onwards

Gloves
* Column: AX
* Description: Data from the Statewide Available PPE Tracking for COVID-19 table, variable "Exam Gloves (Single) On Hand"
* Values: Integer
* DateRange: 2020-04-02 through 2022-02-02
* Missing values reason: This value may be missing if it is not provided in the report <br />
Note: Appeared as "Gloves" from 2020-04-02 through 2020-08-03, "Exam Gloves (single)" from 2020-08-06 through 2021-07-16, "Exam Gloves (Single) On Hand" from 2021-08-11 onwards

Coveralls
* Column: AY
* Description: Data from the Statewide Available PPE Tracking for COVID-19 table, variable "Coveralls"
* Values: Integer
* DateRange: 2020-04-02 through 2020-08-03
* Missing values reason: This value may be missing if it is not provided in the report <br />
Note: This variable may now be reported either in the aggregate variable "Gowns_TOT" or "GownsReuse_TOT"

Isolation_Gowns
* Column: AZ
* Description: Data from the Statewide Available PPE Tracking for COVID-19 table, variable "Surgical Isolation Gowns"
* Values: Integer
* DateRange: 2020-04-02 through 2020-08-03
* Missing values reason: This value may be missing if it is not provided in the report <br />
Note: This variable may now be reported either in the aggregate variable "Gowns_TOT" or "GownsReuse_TOT"

Surgical_Gowns
* Column: BA
* Description: Data from the Statewide Available PPE Tracking for COVID-19 table, variable "Surgical Gowns"
* Values: Integer
* DateRange: 2020-04-02 through 2020-08-03
* Missing values reason: This value may be missing if it is not provided in the report <br />
Note: This variable may now be reported either in the aggregate variable "Gowns_TOT" or "GownsReuse_TOT"

Surgical_Masks
* Column: BB
* Description: Data from the Statewide Available PPE Tracking for COVID-19 table, variable "Surgical Masks on Hand"
* Values: Integer
* DateRange: 2020-04-02 through 2022-02-02
* Missing values reason: This value may be missing if it is not provided in the report <br />
Note: Appeared as "Surgical Masks Facemasks" from 2020-04-02 through 2020-08-03, "Surgical Mask" from 2020-08-06 through 2021-07-16, and "Surgical Masks on Hand" from 2021-08-11 onwards

N95_Masks
* Column: BC
* Description: Data from the Statewide Available PPE Tracking for COVID-19 table, variable "N95 Masks On Hand"
* Values: Integer
* DateRange: 2020-04-02 through 2022-02-02
* Missing values reason: This value may be missing if it is not provided in the report <br />
Note: Appeared as "N95 Respirator Masks" from 2020-04-02 through 2020-08-03, "N95 Masks" from 2020-08-06 through 2021-07-16, and "N65 Masks On Hand" from 2021-08-11 onwards

Shields
* Column: BD
* Description: Data from the Statewide Available PPE Tracking for COVID-19 table, variable "Face Shields"
* Values: Integer
* DateRange: 2020-04-03 through 2020-08-03
* Missing values reason: This value may be missing if it is not provided in the report <br />
Note: This variable may now be reported in the aggregate variable "EyeProtect_TOT"

Goggles
* Column: BE
* Description: Data from the Statewide Available PPE Tracking for COVID-19 table, variable "Goggles"
* Values: Integer
* DateRange: 2020-04-03 through 2020-08-03
* Missing values reason: This value may be missing if it is not provided in the report <br />
Note: This variable may now be reported in the aggregate variable "EyeProtect_TOT"

EyeProtect_TOT
* Column: BF
* Description: Data from the Statewide Available PPE Tracking for COVID-19 table, variable "Eye Protection On Hand"
* Values: Integer
* DateRange: 2020-08-06 through 2022-02-02
* Missing values reason: This value may be missing if it is not provided in the report <br />
Note: This variable may now aggregate previously reported variables "CAPRs", "Shields", and "Goggles". Appeared as "Eye Protection" from 2020-08-06 through 2021-07-16, and "Eye Protection On Hand" from 2021-08-11 onwards

Gowns_TOT
* Column: BG
* Description: Data from the Statewide Available PPE Tracking for COVID-19 table, variable "Gowns On Hand"
* Values: Integer
* DateRange: 2020-08-06 through 2022-02-02
* Missing values reason: This value may be missing if it is not provided in the report <br />
Note: This variable may now aggregate previously reported variables "Coveralls", "Isolation_Gowns", and "Surgical_Gowns". Appeared as "Gowns" from 2021-08-06 through 2021-07-16, and as "Gowns On Hand" from 2021-08-11 onwards

GownsReuse_TOT
* Column: BH
* Description: Data from the Statewide Available PPE Tracking for COVID-19 table, variable "Launderable Gowns On Hand"
* Values: Integer
* DateRange: 2020-08-06 through 2022-02-02
* Missing values reason: This value may be missing if it is not provided in the report <br />
Note: This variable may now aggregate previously reported variables "Coveralls", "Isolation_Gowns", and "Surgical_Gowns". Appeared as "Launderable Gowns from 2020-08-06 through 2021-07-16, and "Launderable Gowns On Hand" from 2021-08-11 onwards

Gloves_0_3
* Column: BI
* Description: Data from the Statewide Available PPE Tracking for COVID-19 table, variable "Exam Gloves (Unable to obtain or less than 3 day supply)"
* Values: Integer
* DateRange: 2022-02-09 through xxxx-xx-xx
* Missing values reason: This value may be missing if it is not provided in the report <br />
Note: This variable lists the amount of hospitals in a region that have 3 days or less of exam gloves

Gloves_4_7
* Column: BJ
* Description: Data from the Statewide Available PPE Tracking for COVID-19 table, variable "Exam Gloves (Duration less than 7 days)"
* Values: Integer
* DateRange: 2022-02-09 through xxxx-xx-xx
* Missing values reason: This value may be missing if it is not provided in the report <br />
Note: This variable lists the amount of hospitals in a region that have between 4 and 7 days of exam gloves

N95_0_3
* Column: BK
* Description: Data from the Statewide Available PPE Tracking for COVID-19 table, variable "N95 Masks (Unable to obtain or less than 3 day supply)"
* Values: Integer
* DateRange: 2022-02-09 through xxxx-xx-xx
* Missing values reason: This value may be missing if it is not provided in the report <br />
Note: This variable lists the amount of hospitals in a region that have 3 days or less of N95 masks

N95_4_7
* Column: BL
* Description: Data from the Statewide Available PPE Tracking for COVID-19 table, variable "N95 Masks (Duration less than 7 days)"
* Values: Integer
* DateRange: 2022-02-09 through xxxx-xx-xx
* Missing values reason: This value may be missing if it is not provided in the report <br />
Note: This variable lists the amount of hospitals in a region that have between 4 and 7 days of N95 masks

SurgicalMasks_0_3
* Column: BM
* Description: Data from the Statewide Available PPE Tracking for COVID-19 table, variable "Surgical Masks (Unable to obtain or less than 3 day supply)"
* Values: Integer
* DateRange: 2022-02-09 through xxxx-xx-xx
* Missing values reason: This value may be missing if it is not provided in the report <br />
Note: This variable lists the amount of hospitals in a region that have 3 days or less of surgical masks

SurgicalMasks_4_7
* Column: BN
* Description: Data from the Statewide Available PPE Tracking for COVID-19 table, variable "Surgical Masks (Duration less than 7 days)"
* Values: Integer
* DateRange: 2022-02-09 through xxxx-xx-xx
* Missing values reason: This value may be missing if it is not provided in the report <br />
Note: This variable lists the amount of hospitals in a region that have between 4 and 7 days of surgical masks

EyeProtect_0_3
* Column: BO
* Description: Data from the Statewide Available PPE Tracking for COVID-19 table, variable "Eye Protection (Unable to obtain or less than 3 day supply)"
* Values: Integer
* DateRange: 2022-02-09 through xxxx-xx-xx
* Missing values reason: This value may be missing if it is not provided in the report <br />
Note: This variable lists the amount of hospitals in a region that have 3 days or less of eye protection (possibly face shields and goggles)

EyeProtect_4_7
* Column: BP
* Description: Data from the Statewide Available PPE Tracking for COVID-19 table, variable "Eye Protection (Duration less than 7 days)"
* Values: Integer
* DateRange: 2022-02-09 through xxxx-xx-xx
* Missing values reason: This value may be missing if it is not provided in the report <br />
Note: This variable lists the amount of hospitals in a region that have between 4 and 7 days of surgical masks (possibly face shields and goggles)

Gowns_0_3
* Column: BQ
* Description: Data from the Statewide Available PPE Tracking for COVID-19 table, variable "Gowns (Unable to obtain or less than 3 day supply)"
* Values: Integer
* DateRange: 2022-02-09 through xxxx-xx-xx
* Missing values reason: This value may be missing if it is not provided in the report <br />
Note: This variable lists the amount of hospitals in a region that have 3 days or less of single-use gowns

Gowns_4_7
* Column: BR
* Description: Data from the Statewide Available PPE Tracking for COVID-19 table, variable "Single-Use Gown (Duration less than 7 days)"
* Values: Integer
* DateRange: 2022-02-09 through xxxx-xx-xx
* Missing values reason: This value may be missing if it is not provided in the report <br />
Note: This variable lists the amount of hospitals in a region that have between 4 and 7 days of single-use gowns

Reporting_Capacity
* Column: BS
* Description: Total response rate for the Statewide Hospital Capacity Report for COVID-19 table
* Values: Percentage
* DateRange: 2020-04-02 through 2021-07-30
* Missing values reason: This value may be missing if it is not provided in the report

Reporting_PPE
* Column: BT
* Description: Total response rate for the Statewide Available PPE Tracking for COVID-19 table
* Values: Percentage
* DateRange: 2020-04-02 through 2021-07-14
* Missing values reason: This value may be missing if it is not provided in the report

Notes
* Column: BU
* Description: Additional notes provided underneath the tables
* Values: String
* Missing values reason: This value may be missing if it is not provided in the report

Link
* Column: BV
* Description: Link to the archival version of the tabular data, through the Wayback Machine Internet Archive
* Values: URL
* Missing values reason: This value may be missing if the Wayback Machine was unresponsive

### MichiganOverview_HospitalTracking_PatientCensus.csv

Date
* Column: A
* Description: Date of report in format YYYY-MM-DD, contained within the first table title, Statewide Hospital Capacity Report for COVID-19
* Values: Date
* Missing values reason: This value should never be missing

COVID_Patients
* Column: B
* Description: Data from the Patient Census table, variable "COVID-19 Patients" (see Note)
* Values: Integer
* DateRange: 2020-04-23 through xxxx-xx-xx
* Missing values reason: This value may be missing if it is not provided in the report <br />
Website Note: Confirmed positive patients, as well as patients who are currently pending and under investigation (PUI). This includes COVID-19 patients in the ICU 

COVID_ICUPatients
* Column: C
* Description: Data from the Patient Census table, variable "COVID-19 Patients in ICU"
* Values: Integer
* DateRange: 2020-04-23 through xxxx-xx-xx
* Missing values reason: This value may be missing if it is not provided in the report <br />
Website Note: Confirmed postive patients and suspected patients in intensive care unit (ICU)

Bed_Occupancy
* Column: D
* Description: Data from the Patient Census table, variable "Bed Occupancy %"
* Values: Percentage
* Missing values reason: This value may be missing if it is not provided in the report <br />
Website Note: The percentage of staffed inpatient beds occupied by any patient regardless of COVID-19 status. This includes surge or overlow beds

Link
* Column: E
* Description: Link to the archival version of the tabular data, through the Wayback Machine Internet Archive
* Values: URL
* Missing values reason: This value may be missing if the Wayback Machine was unresponsive