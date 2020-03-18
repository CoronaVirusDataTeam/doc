# Metadata for Coronavirus Data Scraper

	@context: "https://project-open-data.cio.gov/v1.1/schema/catalog.jsonld"
	conformsTo: ["Project Open Data Metadata Schema v1.1"](https://project-open-data.cio.gov/v1.1/schema/)
	Record ID: b40a7fc7-ef3f-463a-babb-ed7bf5f2649f
	Record Title: coronadatascraper
	Status: underDevelopment
	access level: public

#### Resource Types:

	- tabularDataset: data.csv
	- application: data.json
	- application: timeseries.json
	- application: timeseries-byLocation.json
	- tabularDataset: timeseries.csv
	- tabularDataset: timeseries-tidy.csv
	- tabularDataset: timeseries-jhu.csv

#### Default Resource Local
	
	Character Set: UTF-8
	Country: world
	Language: english
	
	

## Abstract

Dataset for SARS-CoV-2/COVID-19 Pandemic

### Short Abstract

Dataset for SARS-CoV-2/COVID-19 Pandemic


	

## Datasets 

### tabularDataset: data.csv

	title: data.csv
	mediaType: text/csv
	format: csv
	description: The dataset contains the last retrieval of data.
	downloadURL: http://blog.lazd.net/coronadatascraper/data.csv
	accrualPeriodicity: every 60 minutes
	temporal: 2020-01-12
	spatial: world
	modified: 
	identifier: http://blog.lazd.net/coronadatascraper/data.csv
	license: Public Domain
	language: English

	
#### Dataset Schema

	city:
		description: reporting at the city level if a locality is reporting at the city level
		standard: [ISO 3166-2](https://en.wikipedia.org/wiki/ISO_3166-2)
		datatype: text/string
	county:
		description: Full name of a county as "{name} County"
		standard:[Full County Name](https://en.wikipedia.org/wiki/County)
		datatype: text/string
	state:	
		description: State code
		standard: [ISO 3166-2](https://en.wikipedia.org/wiki/ISO_3166-2)
		datatype: text/character
	country:
		description: Country code
		standard: [ISO 3166-2](https://en.wikipedia.org/wiki/ISO_3166-2)	
		datatype: text/character
	cases:	
		description: Number of current cumulative confirmed positive cases.
		standard: [CDC](https://www.cdc.gov/coronavirus/2019-ncov/cases-updates/cases-in-us.html?CDC_AA_refVal=https%3A%2F%2Fwww.cdc.gov%2Fcoronavirus%2F2019-ncov%2Fcases-in-us.html) 
		datatype: integer	
	deaths:	
		description: Number of current cumulative deaths
		standard:
		datatype: integer	
	recovered:
		description: Number of current cumulative recovered
		standard: 
		datatype: integer		
	tested:
		description: Number of current tests performed
		standard:
		datatype: integer		
	active:
		description: Number of current active; outcome pending.
		standard:
		datatype: integer		
	population:
		description: Census population for the given geographic boundry 
		standard:
		datatype: integer 		
	lat:	
		description: [Latitude](https://en.wikipedia.org/wiki/Latitude)
		standard: [Decimal Degrees](https://en.wikipedia.org/wiki/Decimal_degrees)
		datatype: integer	
	long:
		description: [Longitude](https://en.wikipedia.org/wiki/Longitude)
		standard: [Decimal Degrees](https://en.wikipedia.org/wiki/Decimal_degrees)	
		datatype: integer	
	url:
		description: Source URL/URI for acquiring the data
		standard: [URL](https://url.spec.whatwg.org/) 
		datatype: string		
	rating:
		description: Corona Data Scraper pulls from a variety of official sources. Sources are rated based on how machine-readable, complete, and granular the data is.
		standard: [Ratings](http://blog.lazd.net/coronadatascraper/#sources)	
		datatype: integer 	
	featureId:
		description: <needed>
		standard: 
		datatype: integer		
	aggregate:
		description:
		standard:
		datatype: text/string		
	
	
### tabularDataset: json.csv


----
	
keyword: SARS, SARS-CoV-19, COVID-19, coronavisus, virus, infectious disease,








