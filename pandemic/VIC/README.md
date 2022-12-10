# VIC - Dataset guide
 
## Dataset - Daily COVID-19 Data
[VIC_DailyData.csv](https://github.com/dbRaevn/covid19/blob/main/pandemic/VIC/VIC_DailyData.csv)

Daily reported COVID-19 data for Victoria.

 * `REPORT_DATE` - Date the data was reported
 * `NEW_CASES_TOTAL` - Total new COVID-19 cases reported (via PCR and RAT)
 * `NEW_CASES_PCR` - New COVID-19 cases reported via PCR
 * `NEW_CASES_RAT` - New COVID-19 cases reported via RAT
 * `IN_HOSPITAL` - Active COVID-19 cases in hospital
 * `IN_ICU` - Active COVID-19 cases in the ICU
 * `DEATHS` - Reported COVID-19 deaths
 * `PCR_TESTS` - Number of PCR test results returned

**Notes on this dataset**

 1. All numbers are as-reported on the day, and do not include historic corrections
 2. `REPORT_DATE` is based on when the numbers were reported; these relate to cases, test results etc. from the previous day.
 3. `NEW_CASES_PCR` is taken as the difference between `NEW_CASES_TOTAL` and `NEW_CASES_RAT`, as the number is not reported separately
 4. `PCR_TESTS` prior to 1st September 2022 is determined by the delta between total PCR tests on subsequent days. After 1st September 2022, it is the number reported on the given date.
 5. `DEATHS` prior to 1st September 2022 is determined by the delta between total Deaths on subsequent days. After 1st September 2022, it is the number reported on the given date.
 6. There are 15 days between September 2022 and November 2022 that are missing values in the `PCR_TESTS` field. These will be added if they can be determined.
 
**Sources**

 1. Data for `NEW_CASES_TOTAL`, `IN_HOSPITAL`, `IN_ICU`, `DEATHS`,and `PCR_TESTS` before 1st September 2022 is taken from https://covidlive.com.au/. 
 2. Data for the above fields from 1st September 2022, and for all other fields, is collected daily from https://www.coronavirus.vic.gov.au/.
 
## Dataset - Cumulative COVID-19 deaths by age group
[VIC_DeathsByAge.csv](https://github.com/dbRaevn/covid19/blob/main/pandemic/VIC/VIC_DeathsByAge.csv)

Cumulative reported COVID-19 Deaths, broken down by age group.

 * `REPORT_DATE` - Date the data was reported
 * `DEATHS_<Age Band>` - COVID-19 deaths reported in <Age Band>, broken down by decade, 90+, and unknown age.
 * `DEATHS_TOTAL` - Total COVID-19 deaths reported
 * `SOURCE` - Where the data was collected from (see Sources)

**Notes on this dataset**

 1. Reported deaths by age may not align with other reported total death numbers, if ages haven't yet been determined for all cases.
 2. Data is only present for days in which it was collected, able to be retrieved from archive.org or confirmed by cross-referencing other sources; there are significant gaps in this data.
 3. Hostoric deaths were sometimes removed from the total due to duplication or other reasons. Where these were reported in the media released and it was not known which age group it belonged to, a negative death was added to the Unknown age group until the totals could be re-baselined from the totals table on the DHHS site or coronavirus.vic.org.au.
 
**Sources**

 1. Data is collected from a number of sources. Which datasource was used for each date is listed in the `SOURCE` field.
 2. The source is one of:
    * *dhhs.vic.gov.au* - Taken from the [Case locations and outbreaks](https://www.dhhs.vic.gov.au/case-locations-and-outbreaks) page (retrieved via archive.org).
    * *coronavirus.vic.gov.au* - Taken from the [Additional COVID-19 case data](https://www.coronavirus.vic.gov.au/additional-covid-19-case-data) page.
    * *Media Release* - Uses the notified ages of deaths contained in the [daily Coronavirus updates](https://www.health.vic.gov.au/media-centre/media-releases) to determine the cumulative total, only where it can be reliably determined.
    * *No Change* - No source determined, but there was no change in deaths.
 
## Dataset - Hospitalised COVID-19 cases by age group
[VIC_HospitalisedByAge.csv](https://github.com/dbRaevn/covid19/blob/main/pandemic/VIC/VIC_HospitalisedByAge.csv)

Daily number of hospitalised COVID-19 cases, broken down by age group (28th August 2020 - 10th February 2021)

 * `REPORT_DATE` - Date the data was reported
 * `HOSPITALISED_<Age Band>` - COVID-19 cases in hospital in <Age Band>, broken down by decade and 90+.
 * `HOSPITALISED_TOTAL` - Total COVID-19 cases in hospital

**Notes on this dataset**

 1. Data is only present for days in which it was collected or able to be retrieved from archive.org; there are significant gaps in this data.
 
**Sources**

 1. Numbers are taken from the [Case locations and outbreaks](https://www.dhhs.vic.gov.au/case-locations-and-outbreaks) page (retrieved via archive.org). This data was present between 28th August 2020 and 10th February 2021.
	
## Dataset - Ambulance Code Red
[VIC_AmbulanceCodeRed.csv](https://github.com/dbRaevn/covid19/blob/main/pandemic/VIC/VIC_AmbulanceCodeRed.csv)

A list of declared Ambulance Victoria Code Red events.

 * `START` - Date/Time of start of Code Red period
 * `END` - Date/Time of end of Code Red period
 * `DURATION_MIN` - How long the Code Red period lasted (in minutes)
 * `SOURCE_NEWS` - URL to news source of the Code Red period
 * `SOURCE_AMBULANCEVIC_START` - URL to announcement from @AmbulanceVic of the start of the Code Red period (Twitter)
 * `SOURCE_AMBULANCEVIC_END` - URL to announcement from @AmbulanceVic of the end of the Code Red period (Twitter)