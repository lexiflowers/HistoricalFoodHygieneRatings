# Food Hygiene Rating Tracker API

Tracks establishments' food hygiene ratings over time.

This is the API part of a two-part system. It does no fetching of data from the FSA itself and merely serves already-fetched data.

1. [Part one of the system](https://github.com/lexiflowers/FoodHygieneRatingDataFetcher) merely fetches FSA data daily and adds it to a database.

2. Part two of the system (this project) is the API. This serves the DB data sensibly over a REST API.

(3. An archiver saves FSA data to a GitHub repo daily.)

---

## Food Hygiene Rating Tracker

Essentially all it needs to do is capture a snapshot of the variable data of the [UK food hygiene rating data API](https://ratings.food.gov.uk/open-data) every day, then store it in a date-queryable way.

Ideally, present the data in a date- and establishment-queryable API; e.g. "show me ratings for establishments within 2 miles of [lat/long] over the past 2 years", or "show me X establishment's historical ratings over the past 5 years".

> ~~It doesn't look like the FSA hosts any historical data currently. [An FOI to the FSA asking for any historical data](https://www.whatdotheyknow.com/request/historical_fhrs_ratings).~~
>
> After an FOI with an extremely helpful response, it is confirmed that historical FSA data is available on the National Archives website. [See the FOI response for more details](/FOI%2000539.pdf).

> [A complete record, updated daily, of the FSA's open food hygiene rating data](https://ratings.food.gov.uk/open-data#:~:text=Downloadable%20open%20data%20file), is hosted at [https://safhrsprodstorage.blob.core.windows.net/opendatafileblobstorage/FHRS_All_en-GB.csv](https://safhrsprodstorage.blob.core.windows.net/opendatafileblobstorage/FHRS_All_en-GB.csv).
