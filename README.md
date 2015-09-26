# bike-share-analysis

I used NYC citibike <a href="http://www.citibikenyc.com/system-data" target="_blank">system data</a> to implement a classification system to predict routes of citi-bikers given starting station, gender & age of user, day of the week, and time of day.


####Data:
- Merged NYC boundaries geometry file (<a href = "http://catalog.opendata.city/dataset/nyc-neighborhood-tabulation-areas-polygon" target="_blank">source</a>) with station lat/lon data in CartoDB to link each station to its associated neighborhood. (see nyc_neighborhoods.csv)
- Downloaded Dec 2014, Jan & Feb 2015 citibike data and merged with nyc_neighborhoods to find associated neighborhoods for each bike route. (see citibike_dec.csv, citibike_jan.csv & citibike_feb.csv)

####Models:
- Data was merged and cleaned (see citibike notebook)
- Ran different classification algorithms to predict destination <i>neighborhood</i> and scored each on accuracy and precision. Made sure models sampled evenly from each class, given class imbalance. Each destination neighborhood is either correct or incorrect, so accuracy is an effective metric. (see citibike_models notebook)

####Results:
- See my <a href = "http://cgerson.github.io/citimodels/" target="_blank">blog post</a> for a write up of results and a copy of the final presentation