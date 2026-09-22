# Food Hygiene Rating Tracker

Tracks establishments' food hygiene ratings over time.

Essentially all it needs to do is capture a snapshot of the variable data of the [UK food hygiene rating data API](https://ratings.food.gov.uk/open-data) every day, then store it in a date-queryable way.

Ideally, present the data in a date- and establishment-queryable API; e.g. "show me ratings for establishments within 2 miles of [lat/long] over the past 2 years", or "show me X establishment's historical ratings over the past 5 years".

> It doesn't look like the FSA hosts any historical data currently. Getting this data would be useful. Maybe worth an FOI to FSA.

> [A complete record, updated daily, of the FSA's open food hygiene rating data](https://ratings.food.gov.uk/open-data#:~:text=Downloadable%20open%20data%20file), is hosted at [https://safhrsprodstorage.blob.core.windows.net/opendatafileblobstorage/FHRS_All_en-GB.csv](https://safhrsprodstorage.blob.core.windows.net/opendatafileblobstorage/FHRS_All_en-GB.csv).
