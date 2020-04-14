# Scot_covid19
_Update 14 April 2020_ I've uploaded an improved scraper "Get Daily Data.Ipynb" If you have Jupyter Notebooks you can download and run it for yourself. It is a scraper - so it is brittle. Any small change in [the target page](https://www.gov.scot/publications/coronavirus-covid-19-tests-and-cases-in-scotland/) can break it - as has happened three times in development. I'm also now capturing NHS Scotland [staff absences](data/processed/staff_absences.csv).

On 08 Apr 2020 the main Scottish Government page of Coronavirus information was moved to a new location. See _data_ below. 

On 02 Apr 2020__ Today the Scottish Government [announced](https://www.gov.scot/news/new-process-for-reporting-covid-19-deaths/) that the process for recording deaths had been changed. The data was updated tonight to reflect that. 

I have added the number of [patients in Intensive Care](data/processed/intensive_case.csv) from news conferences attended by the First Minister or Chief Medical Officer. 

I [blogged](https://codethecity.org/2020/03/20/scotlands-covid-19-open-data/) about the need for better open data from the government in Scotland. 

This primarily consists of text files (CSV) containing results of Covid-19 testing in Scotland. 

## Data
This now sits in a /data directory with subdirectory for raw and processed data.

### Data Sources
* The source of data from 06 March to 13 March 2020 is the [Internet Wayback Machine](https://archive.org/search.php?query=https%3A%2F%2Fwww.gov.scot%2Fcoronavirus-covid-19%2F). 
* From 14 March 2020 the data is sourced directly from the Scottish Government's [webpage](https://www.gov.scot/coronavirus-covid-19/), and for now is manually added.
* From 8th April 2020 the main Scottish Government Coronovirus information moved to [this webpage](https://www.gov.scot/publications/coronavirus-covid-19-tests-and-cases-in-scotland/) although it appears that the page above is also still being maintained. 
* A friend supplied me with data from 24 Jan 2020 to 6th March to fill in gaps. 

Contains public sector information licensed under the Open Government Licence v3.0.

### Other data
I've added the Health Board codes from the [NHS Scotland Open Data Store](https://www.opendata.nhs.scot/dataset/geography-codes-and-labels/resource/652ff726-e676-4a20-abda-435b98dd7bdc) and a July 2019 [poulation estimate file](data/raw/hb2014_pop_est_01072019.csv) from [NHS Scotland Open Data Store](https://www.opendata.nhs.scot/dataset/population-estimates/resource/27a72cc8-d6d8-430c-8b4f-3109a9ceadb1). Both are published under OGL. 

### Processed data
I've created a Jupyter Notebook, [initial_data.ipynb](initial_data.ipynb) which is used to calculate the 2018 populations of each Health Board, and save that as [HB_Populations.csv](data/processed/HB_Populations.csv). 


## Other resources
I also recommend Tom White's Github repo [Covid-19-UK-Data](https://github.com/tomwhite/covid-19-uk-data) which is broader and more code-driven for now. We may start collaborating / merging these. 


