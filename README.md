# Citi_Bike_Visulization
To visualize using D3, Leaflet


# Citi Bike Maps
Used the Citi Bike API to get the status and location of every Citi Bike station in New York. 

### Steps

1. Used the [Citi Bike station information endpoint](https://gbfs.citibikenyc.com/gbfs/en/station_information.json) to get information about the station names and locations. In your browser.Note the following:

    * Each object in the `stations` array has `station_id`, `name`, `capacity`, `lat`, and `lon` properties.

    * The [logic.js](Unsolved/static/js/logic.js) file contains coordinates that you can use to position a Leaflet map over New York City.

      Developed code to perform a second API call to the [Citi Bike station status endpoint](https://gbfs.citibikenyc.com/gbfs/en/station_status.json). Take a few moments to           study the   data that the endpoint returns. In particular, notice `station_id`, `num_bikes_available`, `is_installed`, and `is_renting`.

2. Used the data that  from the second API call,  to add the following functionality:

    * In the popup for each marker, display the number of available bikes.

    * Added a layer control, and split the markers into the following layer groups:

        * **Coming Soon:** This applies if a station isn't yet installed.

        * **Empty Stations:** This applies if a station has no available bikes.

        * **Out of Order:** This applies if a station is installed but not renting.

        * **Low Stations:** This applies if a station has less than five available bikes.

        * **Healthy Stations:** This applies if a marker doesn't fall into any of the previous layer groups.

3. Used a Leaflet plugin to create different types of markers to represent the layers. The following step shows an example map that uses [Leaflet.ExtraMarkers](https://github.com/coryasilva/Leaflet.ExtraMarkers). 

4. Added a legend to map to explain the different markers. The following image shows an example of the final advanced map:    

5. Deployed it to GitHub Pages.

## Hints

* Make sure that you run `python -m http.server` in the folder that contains your files. Because you'll do all the work on the front end of your app, you won't need to restart the router for any changes that you make.

* Here are some helpful links:

  * [Leaflet map example](https://leafletjs.com/reference-1.7.1.html#map-example)

  * [Citi Bike station information API endPoint](https://gbfs.citibikenyc.com/gbfs/en/station_information.json)

  * [Leaflet popup documentation](http://leafletjs.com/reference.html#popup)

  * [Citi Bike station status API endPoint](https://gbfs.citibikenyc.com/gbfs/en/station_status.json)

  * [Leaflet layer groups documentation](http://leafletjs.com/examples/layers-control/)

  * [Leaflet.ExtraMarkers](https://github.com/coryasilva/Leaflet.ExtraMarkers)

  * [Leaflet legend documentation](http://leafletjs.com/examples/choropleth/#custom-legend-control)
	


## Visulization page link : https://ranjanianjurvenkatraman.github.io/Citi_Bank_Visulization/
