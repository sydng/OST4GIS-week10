# Final Project Proposal
Sydney Goldstein
CPLN 692 JavaScript
April 11, 2018

## Problem / Question

This application will explore the factors around flood inundation post Hurricane Harvey in the Woodlands subdivision in Texas. The Woodlands is known for its historical environmental planning initiatives, however, as the subdivision was constructed the environment became increasingly less important. This application will allow the user to discover and interact with the various factors contributing to flood inundation within each phase of development. By knowing what features were important here, this could help someone who is trying to understand flood inundation in a different area.

## The data

Currently, the data is in raster form and represents soil type, elevation, land use classification, and inundation. I will create points for the centroid of each raster grid cell and spatial join this information to the points. These points will be saved as a GeoJSON, so vector tiles can be made.

## Technologies used

I would like to produce heat maps for both inundation and development to be used in the application. To do this, I am planning to use Mapbox GL to create vector tiles and the heat maps.

I also plan on using openlayers, specifically ol.source.Raster, to interactively display land cover information. Similar to an example found online, I would like to interactively display NDVI and the percentage of land by specific land cover (open space, forest, developed, water, and inundation).

I will use Leaflet Draw as well. If the user draws a shape within the study area, I would like only that area to be selected and have the analysis only show for the area they are interested in.

## Design spec

#### User experience

I expect people to use this application as an exploratory tool to better understand the features that are related to flood inundation. Hurricane Harvey was an extreme event and I believe people who are interested in resilience and climate change would use this application to gain insight into the variables associated with environmental planning that could prevent flood inundation.

#### Layouts and visual design

I picture my application using header with different clickable tabs. When a tab is clicked and that analysis requires more input, a modal or floating side bar will appear for the user to enter information. I imagine that the map will take up the rest of the page. I will most likely use bootstrap to help with the visual design and functionality of the application.

## Anticipated difficulties

I anticipate getting the data to work and performing the analyses on the data to be the most difficult part of this project. If difficulties should arise, I will use the API documentation and other example sources to try to fix the issues.
