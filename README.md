# rooftop-solar
An analysis of rooftop solar potential and deployment across US states


## Project overview
### Context
With photovoltaic panels continuing to plunge in price, rooftop solar is taking off across America. But deployment is uneven: despite being neighbors, Massachusetts higher per-capita rooftop solar installations than New York. That's because state policy can significantly help or hinder the deployment of rooftop solar. And while we have have good data on solar _deployment_, we usually miss the denominator: _potential_.

### Questions

- What percentage of New York State's rooftops could have solar panels on them? 
- What percentage actually do?
- What predicts that rooftop panel installations?

# Business Objective:

### Why does this matter?

### Key stakeholders
- Win Climate
- May be of use to solar advocacy groups in NYC

## Data: 

| Name                                                                                                                                                           | Author                    | Level        | Type                            | Geography      | Format         | \# Rows   | Size     | Sample                                                                   | Dataset                                                                                                                                         |
| -------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------- | ------------ | ------------------------------- | -------------- | -------------- | --------- | -------- | ------------------------------------------------------------------------ | ----------------------------------------------------------------------------------------------------------------------------------------------- |
| [Distributed Solar Projects in NYS](data.ny.gov/Energy-Environment/Statewide-Solar-Projects-Beginning-2000/wgsj-jt5f)                                  | NYSERDA                   | Project      | Distributed solar installations | New York State | CSV            | 203,981   | 25.2 MB  | [Link](data/nyserda_solar_installations_sample.csv)               | [Link](https://data.ny.gov/api/views/wgsj-jt5f/rows.csv?accessType=DOWNLOAD&sorting=true)                                                       |
| [Distributed Solar Projects in NYS subsidized by NYSERDA](https://data.ny.gov/Energy-Environment/Solar-Electric-Programs-Reported-by-NYSERDA-Beginn/3x8r-34rs) | NYSERDA                   | Project      | Distributed solar installations | New York State | CSV            | 153,923   | 61.4 MB  | [Link](data/nyserda_solar_installations_subsidized_sample.csv)    | [Link](https://data.ny.gov/api/views/3x8r-34rs/rows.csv?accessType=DOWNLOAD&sorting=true)                                                       |
| [Project Sunroof](https://console.cloud.google.com/marketplace/product/project-sunroof/project-sunroof)                                                        | Google                    | Census Tract | Rooftop solar potential         | National       | BigQuery Table | 56,940    | 29.38 MB | [Link](data/google_solar_potential_sample.csv)                    | [Link](https://console.cloud.google.com/projectselector2/bigquery?p=bigquery-public-data&d=sunroof_solar&page=dataset&supportedpurview=project) |
| [DeepSolar++](http://web.stanford.edu/group/deepsolar/ds)                                                                                                      | Stanford University       | Census Tract | Rooftop solar insallations      | National       | CSV            | 54,493    | 9.8 MB   | [Link](data/deepsolar_residential_solar_installations_sample.csv) | [Link](https://opendatasharing.s3.us-west-2.amazonaws.com/DeepSolar2/data/residential_solar_installations_panel_data_420counties.csv)           |
| [Tracking the Sun](https://emp.lbl.gov/tracking-the-sun/)                                                                                                      | Law Berkeley National Lab | Project      | Distributed solar installations | National       | CSV            | 2,362,538 | 1.04 GB  | [Link](data/nbnl_solar_installations_sample.csv)                  | [Link](https://emp.lbl.gov/sites/default/files/public_datafile.zip)                                                                             |

## Deliverables:


## Primary Contacts
@jpvelez
@mshron
