# COVID-19 data, outbreak maps and charts

I try to make sense of the large amounts of information about the covid-19 pandemic in Australia by visually presenting it in a way that tells the story of the data.

This repository contains most of the maps, charts and diagrams that were created to track the spread of covid-19 across Australia.

These and the rest of my work can also be found on Twitter - [@dbRaevn](https://twitter.com/dbRaevn)

[☕ Support my work](https://www.buymeacoffee.com/dbRaevn)

## Data sources

 * NSW	[Twitter](https://twitter.com/NSWHealth)
 * VIC	[Twitter](https://twitter.com/VicGovDH)
 * QLD	[Twitter](https://twitter.com/qldhealth)
 * WA	[Twitter](https://twitter.com/MarkMcGowanMP)
 * SA	[Twitter](https://twitter.com/SAHealth)
 * ACT	[Twitter](https://twitter.com/ACTHealth)
 * NSW	[Website](https://www.health.nsw.gov.au/Infectious/covid-19/Pages/stats-nsw.aspx)
 * VIC	[Website (Daily)](https://www.coronavirus.vic.gov.au/)
 * VIC	[Website](https://www.coronavirus.vic.gov.au/victorian-coronavirus-covid-19-data)
 * VIC	[Website (Additional data)](https://www.coronavirus.vic.gov.au/victorian-coronavirus-covid-19-data)
 * VIC	[Media Release](https://www.health.vic.gov.au/media-centre/media-releases)
 * QLD	[Website](https://www.qld.gov.au/health/conditions/health-alerts/coronavirus-covid-19/queensland-covid-19-statistics)
 * WA	[Dashboard](https://experience.arcgis.com/experience/359bca83a1264e3fb8d3b6f0a028d768)
 * WA	[Media Release](https://ww2.health.wa.gov.au/News/Media-releases-listing-page)
 * SA	[Media Release](https://www.sahealth.sa.gov.au/wps/wcm/connect/public+content/sa+health+internet/about+us/news+and+media/all+media+releases?mr-sort=date-desc&mr-pg=1)
 * TAS	[Website](https://www.coronavirus.tas.gov.au/facts/tasmanian-statistics)
 * ACT	[Website (inc. detailed breakdown)](https://www.covid19.act.gov.au/updates/act-covid-19-statistics)
 * NT	[Website](https://health.nt.gov.au/covid-19/data)
 * NSW	[Dataset - (PCR, RAT) Age](https://data.nsw.gov.au/data/dataset/nsw-covid-19-cases-by-age-range/resource/4b03bc25-ab4b-46c0-bb3e-0c839c9915c5)
 * NSW	[Dataset - (PCR, RAT) Location](https://data.nsw.gov.au/data/dataset/covid-19-cases-by-location/resource/5d63b527-e2b8-4c42-ad6f-677f14433520)
 * VIC	[Dataset - (RAT)](https://discover.data.vic.gov.au/dataset/all-victorian-rat-sars-cov-2-cases-by-local-government-area-postcode/resource/a7c149f8-4ad3-4768-84b3-477a054f80bb)
 * VIC	[Dataset - (PCR) Source](https://discover.data.vic.gov.au/dataset/all-victorian-sars-cov-2cases-by-acquired-source/resource/d35dd0fb-5288-4194-8f77-373e2b2cc44d)
 * VIC	[Dataset - (PCR) LGA, Source](https://discover.data.vic.gov.au/dataset/all-victorian-sars-cov-2-cases-by-local-government-area-postcode-and-acquired-source/resource/890da9b3-0976-4de3-8028-e0c22b9a0e09)
 * VIC	[Dataset - (PCR) LGA](https://discover.data.vic.gov.au/dataset/all-victorian-sars-cov-2-cases-by-local-government-area/resource/cc6d89f4-046c-4486-b4a9-63a58fcf9785)
 * VIC	[Dataset - (PCR) Age](https://discover.data.vic.gov.au/dataset/all-victorian-sars-cov-2-cases-by-age-group/resource/b98245c0-f42c-4df8-bced-62f5bcde67f6)
 * VIC	[Dataset - (Total) Active  - Postcode](https://docs.google.com/spreadsheets/d/e/2PACX-1vTwXSqlP56q78lZKxc092o6UuIyi7VqOIQj6RM4QmlVPgtJZfbgzv0a3X7wQQkhNu8MFolhVwMy4VnF/pub?gid=0&single=true&output=csv)
 * VIC	[Dataset - (Total) Active  - LGA](https://docs.google.com/spreadsheets/d/e/2PACX-1vQ9oKYNQhJ6v85dQ9qsybfMfc-eaJ9oKVDZKx-VGUr6szNoTbvsLTzpEaJ3oW_LZTklZbz70hDBUt-d/pub?gid=0&single=true&output=csv)
 * VIC	[Dataset - (Total) Age, Gender](https://public.tableau.com/views/GenderAgeGroup/CasesDashboard?%3Alanguage=en-US&%3Aembed=y&%3Aembed_code_version=3&%3AloadOrderID=4&%3Adisplay_count=y&publish=yes&%3Aorigin=viz_share_link&%3Asize=1056%2C25&&%3AshowVizHome=n&%3Atabs=n&%3AapiID=host2#navType=1&navSrc=Parse) (1)
 * QLD	[Dataset - (PCR) Location, Source](https://www.data.qld.gov.au/dataset/queensland-covid-19-case-line-list-location-source-of-infection)
 * NSW	[Weekly Surveillance Report](https://www.health.nsw.gov.au/Infectious/covid-19/Pages/weekly-reports.aspx)
 * WA	[Weekly Surveillance Report](https://ww2.health.wa.gov.au/Articles/F_I/Infectious-disease-data/COVID19-Weekly-Surveillance-Report)
 * TAS	[Weekly Surveillance Report](https://www.coronavirus.tas.gov.au/facts/tasmanian-statistics/weekly-report)
 * ACT	[Weekly Surveillance Report](https://www.covid19.act.gov.au/updates/act-covid-19-statistics)
 * National	[Monthly Epidemiology Report](https://www1.health.gov.au/internet/main/publishing.nsf/Content/novel_coronavirus_2019_ncov_weekly_epidemiology_reports_australia_2020.htm)
 * National	[Weekly Trends Dashboard](https://www.health.gov.au/health-alerts/covid-19/case-numbers-and-statistics) (2)

(1) To download this dataset, select then deselect an age group. This will enabled the "Data" option under downloads, allowing the dataset to be downloaded as a csv.

(2) Use the following javascript bookmark to show the datatables on this page:  
```javascript:(function () {document.querySelectorAll('[id^="hc-linkto-highcharts-data-table-"]').forEach(button=>button.click())})()```

The following tables outline the data available from each of the above sources.

**Legend:**  
🔵W = Weekly  
🔵M = Monthly  
🔵T = Total (available weekly)  
🟢D = Daily  
🟡A = Daily average over last 7 days  
🟡# = Mixed/complex  
🔴N = Not available  
⚪- = Not applicable

\* Can be calculated or derived from other data in the same source

 * There may be nuances and/or caveats to the data that aren't indicated.
 * Additional metrics may be capturable by comparing week-on-week or day-on-day data (eg., cumulative totals).
 * Surveillance reports and vaccination data are not yet included.

### Information available by data source

This table shows the available information that can be obtained from each official data source.

![Information available by data source](./data/InformationByDataSource_20221014.PNG)

**Notes:**
1. Daily, weekly and total cases available by LGA via the map
2. Weekly total cases provided as a figure, but chart contains daily new cases
3. Contains a breakdown of deaths by age group
4. Active cases provided as PCR/RAT/Total
5. NSW Datasets are missing 180,433 RAT cases recorded between 12-19 January 2022
6. Contains 1 day, weekly and total active cases by postcode
7. Contains 1 day, weekly and total active cases by LGA
8. Total cases only provided for 2022
9. Cases by LGA provided as a rate per 100,000 population
10. Total PCR and RAT cases only provided for 2022
11. Total cases by SA3 Region only provided since 2022
12. Total deaths only provided since 2022
13. Cases by age provided as a rate per 100,000 population
14.	Totals since 15th December 2021
15.	Some information requires accessing raw data tables

**Changelog:**

 - **30/09/2022**
   - Added datasource *TAS - Weekly Surveillance Report*
     - Weekly data for TAS now available for the following: New RAT & PCR cases, total RAT & PCR cases, cases by age and LGA since December 15th 2021, reinfections, deaths, new PCR tests, total PCR tests
   - Removed datasource *National - Weekly Trends Report (no longer exists)*
   - Updated datasource *National - Weekly Trends Dashboard (raw data now accessible)*
     - National new cases, new deaths interval now daily (was 7-day average)
 - **14/10/2022**
   - Update datasource *ACT - Website*
	 - Daily data for the following: New cases, New RAT cases, New PCR cases, Active cases
	 
### Information Available by state

This table shows the sum of available data for each state across all the sources, at the highest frequency available.

![Information Available by state](./data/InformationAvailableByState_20221014.PNG)

## Charts

Primarily charts of the vaccination rollout, but also includes some charts relating to Victorian and NSW outbreaks.

## Maps

These show cases within outbreaks or clusters, and how transmission occurred.

Outbreaks/cluster names are unofficial, and only intended to help identify the outbreak or clusters involved.

 * ACT - Gungahlin cluster
 * NSW - Bondi outbreak
 * NT - Granites Gold Mine outbreak
 * QLD - Portuguese Restaurant outbreak
 * QLD - Taringa/Indooroopilly outbreak
 * SA - Modbury cluster
 * VIC - Black Rock cluster
 * VIC - Lockdown 4 (Whittlesea & West Melbourne outbreaks)
 * VIC - Lockdown 5 (Coolaroo & Maribyrnong clusters)
 * VIC - Lockdown 6 (West Footscray & Hobsons Bay clusters)
 * AUS - Outbreak maps
 * NZ - Auckland cluster
 * WORLD - Initial Omicron Spread
