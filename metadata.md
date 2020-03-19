# Metadata for Coronavirus Data Scraper

`@context:` https://project-open-data.cio.gov/v1.1/schema/catalog.jsonld

`conformsTo:` [Project Open Data Metadata Schema v1.1](https://project-open-data.cio.gov/v1.1/schema/)

`Record ID:` b40a7fc7-ef3f-463a-babb-ed7bf5f2649f

`Record Title:` coronadatascraper

`Status:` underDevelopment

`access level:` public


#### Resource Types:

	- tabularDataset: data.csv
	- application: data.json
	- application: timeseries.json
	- application: timeseries-byLocation.json
	- tabularDataset: timeseries.csv
	- tabularDataset: timeseries-tidy.csv
	- tabularDataset: timeseries-jhu.csv


#### Default Resource Local
	
`Character Set:` UTF-8

`Country:` world

`Language:` english
	
	
## Abstract

The [Coronavirus Data Scraper](https://coronadatascraper.com/) team objective is to collect authoritative data that is being reported from local/state/national sources, in an aggregated [dataset](https://github.com/CoronaVirusDataTeam/docs/blob/master/metadata.md), during the SARS-CoV-2:COVID-19 pandemic with an origin in Wuhan China, December 2019.


### Short Abstract

Coronavirus Data Scraper (CDS) dataset collected during the SARS-CoV-2:COVID-19 pandemic of 2019-2020  



## Datasets 


### tabularDataset data.csv

`title:` data.csv

`mediaType:` text/csv

`format:` csv

`description:` The dataset contains the last retrieval of data.

`downloadURL:` [https://coronadatascraper.com/data.csv](https://coronadatascraper.com/data.csv)

`accrualPeriodicity:` once a day at 21:00 - 8 UTC (PST) | - 7 UTC DST (PST)

`temporal:` 2020-01-12

`spatial:` world

`modified:`

`identifier:` https://coronadatascraper.com/data.csv

`license:` Public Domain

`language:` English

	
#### Dataset Schema

`city:`

- `description:` reporting at the city level if a locality is reporting at the city level

- `standard:` [ISO 3166-2](https://en.wikipedia.org/wiki/ISO_3166-2)
	
- `datatype:` text/string


`county:`

-	`description:` Full name of a county as "{name} County"
	
-	`standard:` [Full County Name](https://en.wikipedia.org/wiki/County)
	
-	`datatype:` text/string

	
`state:`
	
-	description: State code

-	standard: [ISO 3166-2](https://en.wikipedia.org/wiki/ISO_3166-2)

-	datatype: text/character


`country:`

-	description: Country code

-	standard: [ISO 3166-2](https://en.wikipedia.org/wiki/ISO_3166-2)
		
-	datatype: text/character
	
	
`cases:`

-	description: Number of current cumulative confirmed positive cases.

-	standard: [CDC](https://www.cdc.gov/coronavirus/2019-ncov/cases-updates/cases-in-us.html?CDC_AA_refVal=https%3A%2F%2Fwww.cdc.gov%2Fcoronavirus%2F2019-ncov%2Fcases-in-us.html) 

-	datatype: integer
	
`deaths:`	

-	description: Number of current cumulative deaths

-	standard:

-	datatype: integer	

`recovered:`

-	description: Number of current cumulative recovered

-	standard:

-	datatype: integer
		
`tested:`

-	description: Number of current tests performed

-	standard:

-	datatype: integer
		
`active:`

-	description: Number of current active; outcome pending.

-	standard:

-	datatype: integer
		
`population:`

-	description: Census population for the given geographic boundary

-	standard:

-	datatype: integer
 		
`lat:`	

-	description: [Latitude](https://en.wikipedia.org/wiki/Latitude)

-	standard: [Decimal Degrees](https://en.wikipedia.org/wiki/Decimal_degrees)

-	datatype: integer	


`long:`

-	description: [Longitude](https://en.wikipedia.org/wiki/Longitude)

-	standard: [Decimal Degrees](https://en.wikipedia.org/wiki/Decimal_degrees)
	
-	datatype: integer	


`url:`

-	description: Source URL/URI for acquiring the data

-	standard: [URL](https://url.spec.whatwg.org/) 

-	datatype: string	
	
	
`rating:`

-	description: Corona Data Scraper pulls from a variety of official sources. Sources are rated based on how machine-readable, complete, and granular the data is.

-	standard: [Ratings](https://coronadatascraper.com/#sources)
	
-	datatype: integer 	


`featureId:`

-	description: The ID of the feature this location references (index in [features.json's](https://github.com/lazd/coronadatascraper/blob/master/tasks/findFeatures.js) FeatureCOllection)

-	standard: 

-	datatype: integer	

	
`aggregate:`

-	description: Whether this data source provides aggregate information (i.e. this county-level data was scraped from a state-level source)

-	standard: 

-	datatype: text/string		
	
	
### application data.json

### application timeseries.json

### application timeseries-byLocation.json

---

### tabularDataset timeseries.csv


`title:` timeseries.csv

`mediaType:` text/csv

`format:` csv

`description:` The dataset contains time series dataset.

`downloadURL:` [https://coronadatascraper.com/timeseries.csv](https://coronadatascraper.com/timeseries.csv)

`accrualPeriodicity:` once a day at 21:00 - 8 UTC (PST) | - 7 UTC DST (PST)

`temporal:` 2020-01-22

`spatial:` world

`modified:` 

`identifier:` https://coronadatascraper.com/timeseries.csv

`license:` Public Domain

`language:` English

	
#### Dataset Schema

`city:`

- `description:` reporting at the city level if a locality is reporting at the city level

- `standard:` [ISO 3166-2](https://en.wikipedia.org/wiki/ISO_3166-2)
	
- `datatype:` text/string


`county:`

-	`description:` Full name of a county as "{name} County"
	
-	`standard:` [Full County Name](https://en.wikipedia.org/wiki/County)
	
-	`datatype:` text/string

	
`state:`
	
-	description: State code

-	standard: [ISO 3166-2](https://en.wikipedia.org/wiki/ISO_3166-2)

-	datatype: text/character


`country:`

-	description: Country code

-	standard: [ISO 3166-2](https://en.wikipedia.org/wiki/ISO_3166-2)
		
-	datatype: text/character
	
	
`population:`

-	description: Census population for the given geographic boundary

-	standard: [WikiData](https://www.wikidata.org)
		
-	datatype: text/character

	
`lat:`	

-	description: [Latitude](https://en.wikipedia.org/wiki/Latitude)

-	standard: [Decimal Degrees](https://en.wikipedia.org/wiki/Decimal_degrees)

-	datatype: integer	


`long:`

-	description: [Longitude](https://en.wikipedia.org/wiki/Longitude)

-	standard: [Decimal Degrees](https://en.wikipedia.org/wiki/Decimal_degrees)
	
-	datatype: integer	


`url:`

-	description: Source URL/URI for acquiring the data

-	standard: [URL](https://url.spec.whatwg.org/) 

-	datatype: string		
	
	
`cases:`

-	description: Number of current cumulative confirmed positive cases.

-	standard: [CDC](https://www.cdc.gov/coronavirus/2019-ncov/cases-updates/cases-in-us.html?CDC_AA_refVal=https%3A%2F%2Fwww.cdc.gov%2Fcoronavirus%2F2019-ncov%2Fcases-in-us.html) 

-	datatype: integer
	

`deaths:`	

-	description: Number of current cumulative deaths

-	standard:

-	datatype: integer	


`recovered:`

-	description: Number of current cumulative recovered

-	standard:

-	datatype: integer


`active:`

-	description: Number of current active; outcome pending.

-	standard:

-	datatype: integer
	
	
`tested:`

-	description: Number of current tests performed

-	standard:

-	datatype: integer
		

`growthFacotr:`

-	description: Exponential growth factor for the given geographic boundary

-	standard: [Exponential Growth](https://en.wikipedia.org/wiki/Exponential_growth)

-	datatype: integer		

 		
`date:`

-	description: date for the observation/record

-	standard: [ISO 8601l Growth](https://en.wikipedia.org/wiki/ISO_8601)

-	datatype: string		
	





	
	

---

### tabularDataset timeseries-tidy.csv

### tabularDataset timeseries-jhu.csv


----
	
keyword: SARS, SARS-CoV-19, COVID-19, coronavisus, virus, infectious disease,








