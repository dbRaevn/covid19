# VIC - Dataset guide

## Dataset - Ambulance Code Red
[VIC_AmbulanceCodeRed.csv](https://github.com/dbRaevn/covid19/blob/main/pandemic/VIC/VIC_AmbulanceCodeRed.csv)

A list of declared Ambulance Victoria Code Red events.

 * `START` - Date/Time of start of Code Red period
 * `END` - Date/Time of end of Code Red period
 * `DURATION_MIN` - How long the Code Red period lasted (in minutes)
 * `SOURCE_NEWS` - URL to news source of the Code Red period
 * `SOURCE_AMBULANCEVIC_START` - URL to announcement from @AmbulanceVic of the start of the Code Red period (Twitter)
 * `SOURCE_AMBULANCEVIC_END` - URL to announcement from @AmbulanceVic of the end of the Code Red period (Twitter)
 
## Dataset - Daily COVID-19 data
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
 2. Data from 1st September 2022 is collected daily from https://www.coronavirus.vic.gov.au/.