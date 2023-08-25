# rooftop-solar
An analysis of rooftop solar potential and deployment across New York State


### Context
As photovoltaic panels continue to plunge in price, rooftop solar is starting to take off across America. But some states have deployed far more panels then others, and not just because of geography: despite being neighbors, Massachusetts has higher per-capita rooftop solar installations than New York. That's because state policy can significantly help or hinder the deployment of rooftop solar. But before we can fix this gap between potential and actual rooftop solar, we need to measure it. To our knowledge, nobody has done this for New York State.

### Questions

1. What percentage of New York State's rooftops could have solar panels on them? What percentage actually do?
2. How does this gap vary by race, income, and location?
3. What predicts location of rooftop panel installations?
4. How have federal and state solar subsidies affected the pace of installations?

### Why does this matter?
- **Question 1**: New York State's goal is to install 50GW of solar capacity in the next 17 years, a healthy portion of which should be rooftop solr. So even just measuring the gap between actual and potential rooftop solar, and how quickly we're closing it, could dramatically help distributed solar advocates like [SolarOne](https://solar1.org/), [VoteSolar](https://votesolar.org/), and [NYSEIA](https://www.nyseia.org/) push the state legislature to adopt their proposed policies. 

- **Question 2**: These policies aren't just about speeding up distributed solar deployment in general, but about closing the solar equity gap: anecdotally, low and moderate in New Yorkers don't appear to be benefitting from rooftop solar, even though they have the most to gain from cheaper power. So being able to characterize how the gap between potential and actual deployment varies by race and income would be even more valuable.

- **Question 3**: Understanding the correlates of solar panel installation through statistical modeling could help design policies to close the gap, or allow advocates to exert political pressure on specific legislators, which is even more important.

- **Question 4**: besides dropping prices, advocates that rooftop solar subsidies have the main driver of how quickly solar has been deployed over the past two decades. Given that the subsidy levels have fluctuated over time, we may be able to measure the price elasticity of demand for solar panels, and thereby measure the extent to which subsidy level drive installations. This can help advocates design and campaign for revised state solar subsidies, particularly with an eye to closing the equity gap.

### Key stakeholders
- Think tank [Win Climate](http://climate.win)
- Possibly: solar advocates [SolarOne](https://solar1.org/), [VoteSolar](https://votesolar.org/), and [NYSEIA](https://www.nyseia.org/)

### Data: 

| Name                                                                                                                                                           | Author                    | Level        | Type                            | Geography      | Format         | \# Rows   | Size     | Sample                                                                   | Dataset                                                                                                                                         |
| -------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------- | ------------ | ------------------------------- | -------------- | -------------- | --------- | -------- | ------------------------------------------------------------------------ | ----------------------------------------------------------------------------------------------------------------------------------------------- |
| [Distributed Solar Projects in NYS](http://data.ny.gov/Energy-Environment/Statewide-Solar-Projects-Beginning-2000/wgsj-jt5f)                                  | NYSERDA                   | Project      | Distributed solar installations | New York State | CSV            | 203,981   | 25.2 MB  | [Link](data/nyserda_solar_installations_sample.csv)               | [Link](https://data.ny.gov/api/views/wgsj-jt5f/rows.csv?accessType=DOWNLOAD&sorting=true)                                                       |
| [Distributed Solar Projects in NYS subsidized by NYSERDA](https://data.ny.gov/Energy-Environment/Solar-Electric-Programs-Reported-by-NYSERDA-Beginn/3x8r-34rs) | NYSERDA                   | Project      | Distributed solar installations | New York State | CSV            | 153,923   | 61.4 MB  | [Link](data/nyserda_solar_installations_subsidized_sample.csv)    | [Link](https://data.ny.gov/api/views/3x8r-34rs/rows.csv?accessType=DOWNLOAD&sorting=true)                                                       |
| [Project Sunroof](https://console.cloud.google.com/marketplace/product/project-sunroof/project-sunroof)                                                        | Google                    | Census Tract | Rooftop solar potential         | National       | BigQuery Table | 56,940    | 29.38 MB | [Link](data/google_solar_potential_sample.csv)                    | [Link](https://console.cloud.google.com/projectselector2/bigquery?p=bigquery-public-data&d=sunroof_solar&page=dataset&supportedpurview=project) |
| [DeepSolar++](http://web.stanford.edu/group/deepsolar/ds)                                                                                                      | Stanford University       | Census Tract | Rooftop solar insallations      | National       | CSV            | 54,493    | 9.8 MB   | [Link](data/deepsolar_residential_solar_installations_sample.csv) | [Link](https://opendatasharing.s3.us-west-2.amazonaws.com/DeepSolar2/data/residential_solar_installations_panel_data_420counties.csv)           |
| [Tracking the Sun](https://emp.lbl.gov/tracking-the-sun/)                                                                                                      | Law Berkeley National Lab | Project      | Distributed solar installations | National       | CSV            | 2,362,538 | 1.04 GB  | [Link](data/nbnl_solar_installations_sample.csv)                  | [Link](https://emp.lbl.gov/sites/default/files/public_datafile.zip)                                                                             |

### Deliverables
* A report that answers the questions above
    - Ideally in the form of a Quarto notebook with code that can reproduce all results from raw data
    - To the extent possible, the code should work for other US states

* A data evaluation that
    - Documents the datasets
    - Explains how they overlap, diverge, and relate
    - Evaluates their quality
    - Details their limitations
    - Advocates for data improvements


### Primary Contacts
* Juan-Pablo Velez, Executive Director, Win Climate (jpv@climate.win)
* Max Shron, Research Director, Win Cliamte (max@climate.win)
