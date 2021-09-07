# Daily reports (csse_covid_19_daily_reports)
- This folder contains daily case reports. All timestamps are in UTC (GMT+0).

## File naming convention
- MM-DD-YYYY.csv in UTC.

## Dataset description

- FIPS: US only. Federal Information Processing Standards code that uniquely identifies counties within the USA.
- Admin2: County name. US only.
- Province_State: Province, state or dependency name.
- Country_Region: Country, region or sovereignty name. The names of locations included on the Website correspond with the official designations used by the U.S. Department of State.
- Last Update: MM/DD/YYYY HH:mm:ss (24 hour format, in UTC).
- Lat and Long_: Dot locations on the dashboard. All points (except for Australia) shown on the map are based on geographic centroids, and are not representative of a specific address, building or any location at a spatial scale finer than a province/state. Australian dots are located at the centroid of the largest city in each state.
- Confirmed: Counts include confirmed and probable (where reported).
- Deaths: Counts include confirmed and probable (where reported).
- Recovered: Recovered cases are estimates based on local media reports, and state and local reporting when available, and therefore may be substantially lower than the true number. US state-level recovered cases are from [COVID Tracking Project](https://covidtracking.com/). We stopped to maintain the recovered cases (see Issue #3464 and Issue #4465).
- Active: Active cases = total cases - total recovered - total deaths. This value is for reference only after we stopped to report the recovered cases (see Issue #4465)
- Incident_Rate: Incidence Rate = cases per 100,000 persons.
- Case_Fatality_Ratio (%): Case-Fatality Ratio (%) = Number recorded deaths / Number cases.
- All cases, deaths, and recoveries reported are based on the date of initial report. Exceptions to this are noted in the "Data Modification" and "Retrospective reporting of (probable) cases and deaths" subsections below.
Update frequency
Since June 15, We are moving the update time forward to occur between 04:45 and 05:15 GMT to accommodate daily updates from India's Ministry of Health and Family Welfare.
Files on and after April 23, once per day between 03:30 and 04:00 UTC.
Files from February 2 to April 22: once per day around 23:59 UTC.
Files on and before February 1: the last updated files before 23:59 UTC. Sources: archived_data and dashboard.

## Data Source
- https://github.com/CSSEGISandData/COVID-19