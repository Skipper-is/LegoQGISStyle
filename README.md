# LegoQGISStyle
Lego QGIS style, based on Cartocalypse's design on Twitter

# Process
Layer was created from Ordnance Surveys Terrain 50 Open Data
Contains OS data © Crown copyright and database right (2019)

The original .asc layer was loaded into QGIS, and the regular points tool applied to it. 
The parameters for this was:

- Extent: Extent of the .asc layer

- Point spacing: 50 meters (same as the resolution of the raster (and tick the "Use point spacing" box)

- Initial offset: half the point spacing, 25m - so it is in the centre of the pixel

A subset of that generated points layer was then taken using the clip tool (could also use select> copy>paste as new layer

Using SAGA's "add raster values to points" I gave the new points the value from the terrain layer

This new layer, and it's style is what is present here
