# usgs-map

A webpage for visualizing earthquake geoJSON data obtained from US Geological Surveys website. 

## Summary 
This visualization turns raw geoJSON data into an interactive visualization.

Raw geoJSON: <br>
`{"type":"FeatureCollection",
"metadata":
    {"generated":1619824149000,"url":"https://earthquake.usgs.gov/earthquakes/feed/v1.0/summary/all_month.geojson","title":"USGS All Earthquakes, Past Month","status":200,"api":"1.10.3","count":2617},
    "features":[{"type":"Feature","properties":{"mag":1.3,"place":"30 km SW of Hawthorne, Nevada","time":1619821705199,...}`

## Visualization 
![image](images/overall.png)
The webpage uses Leaflet and Javascript to plot the geoJSON data. Each marker size represents an earthquake's magnitude and the color represents the depth. Users can click on each point to learn more about the event. 

![image](images/depth.png)
The visualization offers three layers to choose from: 'Satellite', 'Grayscale', and 'Outside' (tile layers obtained from Mapbox). 