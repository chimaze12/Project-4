# Projects 3&4: GeoWeb APP with a Mapbox Layer on Traffick Incidents

ENGO 651 - Advanced Geospatial Topics

## Overview:
This website is an assignment for Advanced Geospatial Topics (ENGO 651) by group 6. We created a web mapping application for building permits in Calgary, Canada, which is taken from the Open Calgary API dataset. Users can find all building permits on the map by selecting the issue date range they like. Moreover, some useful information, such as contractor name and community name, of any building permit exists on the pop-up content of the marker that represents the specific building permit. To make the map visually appealing, we handled the problem of overlapping markers and made a cluster of the neighboring markers on the map.

## Lab 4
For Lab 4, we have added a mapbox layer showing the locations of traffic incidents in Calgary, from csv dataset found on Open Calgary Data website. We created a layer on Mapbox layer and imported the data from the outlet mentioned above and added some personal touch to the map. This Geoweb Application will now be able to display not just building permits in Calgary when users search for it, it will also be able to display locations of traffic incidences in Calgary. All  marker and map styles were done in Mapbox.


## Libraries required to install:
- Flask 
- requests <br>
You can find both libraries in the `requirements.txt` and install them by running this command `pip3 install -r requirements.txt` in the terminal window.

## Tools and Resources used:
- HTML 5
- CSS
- Python flask 
- Javascript
- [Leaflet](https://leafletjs.com/)
- [GeoJSON](https://leafletjs.com/examples/geojson/)
- [Open Calgary API dataset](https://data.calgary.ca/Business-and-Economic-Activity/Building-Permits/c2es-76ed)
- [Open Calgary Dataset on Traffic Incidents](https://data.calgary.ca/Transportation-Transit/Traffic-Incidents-Archive-2017/himp-urp7/data)



## what’s contained in each file:
- `application.py`: is responsible for python flask coding and getting JSON data from Open Calgary API dataset and then passes it to the `building_permit_search.html` file.
- `templates/building_permit_search.html`: has the structure of the webpage and all links of Leaflet code.   
- `static/styles/building_permit_search.css`: this is a specified style sheet file for `building_permit_search.html` file.
- `static/js/building_permit_search.js`: The codes for creating Leaflet map and date range widget algorithm, as well as the separate map layers are located in this file.
- `static/js/building_permits_after_searching.js`: all algorithms after searching, including adding markers to the map, handling overlapping markers, and markers clustering, exists in this file. 







