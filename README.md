# Exploring Parks in Los Angeles County

## What this map shows

This project is an interactive Web GIS map showing parks and open spaces across Los Angeles County. Users can explore the distribution of parks, zoom in to different areas, and click on individual parks to view more information, including the park name, city, area, type, and agency.

## Starting sample

I used Esri's official **Intro to FeatureLayer** sample from the ArcGIS Maps SDK for JavaScript (version 5.1) as the starting point.

Sample: https://developers.arcgis.com/javascript/latest/sample-code/get-started-layers/

## What I changed

The original sample displayed tree data and used different symbol sizes to represent carbon storage. I replaced the tree layer with park polygons in Los Angeles County. I changed the basemap to Streets Vector and used green fill symbols with darker green outlines to make the parks easier to identify.

I also changed the map's initial location and zoom level, updated the popup information, and added a green header and a short introduction above the map.

## Data source

The park data comes from a public ArcGIS Feature Service called **LA_greenspace**.

Data URL: https://services3.arcgis.com/kfmqp6kwSeDnDKNY/ArcGIS/rest/services/LA_greenspace/FeatureServer/0

I used FeatureLayer to load the data directly from this online service through the ArcGIS REST API. This means the geographic data does not need to be stored in my GitHub repository. I chose this dataset because it covers parks and open spaces throughout Los Angeles County, which matches my project topic.

## Component I added

I kept the Zoom, Legend, and Layer List components from the original sample. I also added Home to return to the initial map view and Scale Bar to show distances. These components make the map easier to navigate and understand.

## Problems and what I'd improve next

One problem I encountered was that the Layer List panel overlapped the popup window, making some popup buttons difficult to use. I addressed this by placing Layer List inside an Expand component so users can open it only when needed.

In the future, I would like to add a search function so users can find specific parks by name. I could also add filters for park types to make the map more useful.

## Credits

The original code structure was adapted from Esri's Intro to FeatureLayer sample. Park data was accessed through the public LA_greenspace ArcGIS Feature Service.

I used ChatGPT to help me understand the sample code and provide guidance on code modifications and debugging.
