# EventBasedYearlyMean
Taking +/- 7 days from each Date in Table11.csv, each Date including the +/- 7 days is an Event for which we will compute a yearly Max/Min/Mean Wind Speed from a Period of Record Dataset for Multiple Gage Locations fom: https://mesonet.agron.iastate.edu/request/download.phtml?network=LA_ASOS

The gage locations chosen are shown in the image below:
![000_Gage Locations](https://user-images.githubusercontent.com/64209352/175986723-a8c6ef23-91d3-453d-be45-7b0df69e65a2.png)

Each gage location has its own Period of Record of wind speed data. For each year in the period of record, over the time window of the Event's days/months for each year, the Max/Min/Mean Wind Speed will be computed for each gage. For each Event/Gage combination, a plot is created via Plotly as - both an HTML and PNG file - to illustrate the yearly Max/Min/Mean Wind Speed. An example plot is shown below: 
![2019 13Apr - 27Apr NEW](https://user-images.githubusercontent.com/64209352/175987589-2b660e67-133d-4579-b4a7-06b0bb1bcf68.png)

Be Aware, should an event be used for which there is no data for a gage in it's respective period of record dataset, the output is a filename of "nan {eventDate}"
