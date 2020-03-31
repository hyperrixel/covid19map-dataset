# Dataset to visualize covid-19-history

## About dataset

We are providing preprocessed dataset about COVID-19 (corona virus) disease. The source data comes from [ECDC](https://www.ecdc.europa.eu/en). The beginning of time series is 2020-01-01. We are trying to keep the repository up to date. If you have any question, don't hesitate to ask.

Currently we provide numbers of confirmed cases and death per date and country. Dataset contains 6 columns in the following order:
` date ` | ` areacode ` | ` cumulated cases ` | ` cumulated death ` | ` additional cases ` | ` additional death `.

Sidenotes:
- ` date ` field is in ` YYYY-MM-DD ` format.
- ` areacode ` field follows the phone country codes but U.S.A. is ` 1000 `.

## Working example

On [rixel](https://hyperrixel.com/covid19map)'s website we use this dataset to show various aspects of COVID-19 epidemic.
![screenshot](https://hyperrixel.com/covid19map/screenshot.jpg)

## Notes

The dataset contains data from USA in aggregated format. The dataset doesn't contain data from International conveyance in Japan (such as Diamond Princess Cruise Ship). If there is a missing additional datapoint, we automatically set it to 0. If there is a missing cumulative datapoint, we use the last valid cumulative datapoint.

## Future plans

- update regularly
- add recovered data
- use other sources to confirm data such as: WHO or John Hopkins CSSE

