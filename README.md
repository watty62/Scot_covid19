# Scot_covid19
* Update 20 Mar 2020 * I have now [blogeed](https://codethecity.org/2020/03/20/scotlands-covid-19-open-data/) about the need for better open data from the government in Scotland. 

This primarily consists of text files (CSV) containing results of Covid-19 testing in Scotland. 

## Data
This now sits in a /data directory with subdirectory for raw and processed data.

### Data Sources
* The source of data from 06 March to 13 March 2020 is the [Internet Wayback Machine](https://archive.org/search.php?query=https%3A%2F%2Fwww.gov.scot%2Fcoronavirus-covid-19%2F). 
* From 14 March 2020 the data is sourced directly from the Scottish Government's [webpage](https://www.gov.scot/coronavirus-covid-19/), and for now is manually added.

* A friend supplied me with data from 24 Jan 2020 to 6th March to fill in gaps. 

I am currently looking for an API similar to Public Health England's one to automate updates. 

### Other data
I've added the Health Board codes from the [NHS Scotland Open Data Store](https://www.opendata.nhs.scot/dataset/geography-codes-and-labels/resource/652ff726-e676-4a20-abda-435b98dd7bdc) and a July 2019 [poulation estimate file](data/raw/hb2014_pop_est_01072019.csv) from [NHS Scotland Open Data Store](https://www.opendata.nhs.scot/dataset/population-estimates/resource/27a72cc8-d6d8-430c-8b4f-3109a9ceadb1). Both are published under OGL. 

### Processed data
I've created a Jupyter Notebook, [initial_data.ipynb](initial_data.ipynb) which is used to calculate the 2018 populations of each Health Board, and save that as [HB_Populations.csv](data/processed/HB_Populations.csv). 


## Other resources
I also recommend Tom White's Github repo [Covid-19-UK-Data](https://github.com/tomwhite/covid-19-uk-data) which is broader and more code-driven for now. We may start collaborating / merging these. 


