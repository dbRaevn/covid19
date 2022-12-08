# NT - Dataset guide

## Dataset - Public Health Emergency Declarations
[NT_PublicHealthEmergencyDeclarations.csv](https://github.com/dbRaevn/covid19/blob/main/pandemic/NT/NT_PublicHealthEmergencyDeclaration.csv)

This dataset lists the Declarations that started and extended the Public Health Emergency in the Northern Territory.

 * `GAZETTE_NO` - The Gazette Number the declaration appears in
 * `GAZETTE_DATE` - The Gazette Date the declaration appears in
 * `TITLE` - Title of the declaration
 * `URL` - Link to an official source containing the Direction (pdf)
 * `NOTE` - Note indicating nature and timeperiod of declaration

## Dataset - Pandemic Directions
[NT_PandemicDirections.csv](https://github.com/dbRaevn/covid19/blob/main/pandemic/NT/NT_PandemicDirections.csv)

This dataset contains a list of all Chief Health Officer Directions made under section 52 of the Public
and Environmental Health Act 2011.

 * `DATE_EFFECTIVE_START` - Date/Time when the Direction goes into effect
 * `DATE_EFFECTIVE_END_ORIGINAL` - Date/Time when the Direction was originally specified to no longer be in effect
 * `DATE_EFFECTIVE_END_ACTUAL` - Date/Time when the Direction was no longer in effect (taking into account amendments and revocations)
 * `DATE_PUBLISHED` - Date/Time when the Direction was published
 * `DIRECTION_NAME` - The official name of the Direction
 * `DIRECTION_ALTERNATE_NAME` - An alternate name given for this Direction
 * `CATEGORY` - A general classification of the nature of the Direction (see category list below)
 * `REVOKED_BY` - A list of Directions that revoke this Direction
 * `AMENDED_BY` - A list of Directions that amend this Direction
 * `URL` - Link to an official source containing the Direction (pdf)

**Categories**
The Category field may include the following values

 * Lockdown
 * Business Closure
 * Restriction
 * Mask Mandate
 * Aged Care
 * Border
 * Other

**Notes on this dataset**

 1. A Lockdown is defined as a legal requirement to remain within your residence except for specified purposes (not including individual requirements due to circumstance such as isolation or quarantine).
 2. A Business Closure is defined as a broad requirement for non-essential businesses to close.

**Sources**

 1. This dataset is collated from the list of NT pandemic Declarations found here: [Chief Health Officer directions](https://health.nt.gov.au/covid-19/restrictions/chief-health-officer-directions)

## Dataset - Lockdowns
[NT_Lockdowns.csv](https://github.com/dbRaevn/covid19/blob/main/pandemic/NT/NT_Lockdowns.csv)

This dataset contains a list of Lockdowns.

Per the category definitions listed under the "Pandemic Directions" dataset, the start and end dates in this list reflect both *Lockdowns* and *Business Closures* within a period.

 * `LOCKDOWN_NAME` - An unofficial name used for the lockdown period
 * `START` - Date/Time of the start of the lockdown or business closure
 * `END` - Date/Time of the end of the lockdown or business closure

## Dataset - Lockdown Populations
[NT_LockdownPopulations.csv](https://github.com/dbRaevn/covid19/blob/main/pandemic/NT/NT_LockdownPopulations.csv)

This dataset can be used to calculate the population under Lockdown Directions.

 * `LOCKDOWN_NAME` - An unofficial name used for the lockdown period
 * `DIRECTION_NAME` - The official name of the Direction
 * `START` - Date/Time of the start of when the area is affected under the Direction
 * `END` - Date/Time of the end of when the area is affected under the Direction
 * `AREA` - The area specified in the Direction
 * `AREA_TYPE` - The Type of area specified in the Direction
 * `POPULATION` - The estimated population of the area
 
**Area Types**  
The Area Types field may include the following values

 * LGA
 * State
 * Other
 
**Sources**

 1. For LGA & State area types, population estimates are based on ABS data: [Population estimates by LGA and electoral division (ASGS2021), 2001 to 2021](https://www.abs.gov.au/statistics/people/population/regional-population/2021)
 2. Other areas include various definitions (localities, geographic co-ordinates, descriptive boundaries, etc.), for which approximate population estimates are obtained from [2021 Census data](https://www.abs.gov.au/census/find-census-data/search-by-area).