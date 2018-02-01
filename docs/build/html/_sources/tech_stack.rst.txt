**********
Tech Stack
**********

Considerations
^^^^^^^^^^^^^^
While choosing the tech stack for the web portal we need think about scalability in terms of the following things

- Storage
- Performance 
- Customizability


Vector Tiles
^^^^^^^^^^^^

Vector data would best in terms of storage but it could cause performance issue in the client side. Serving raster tiles will allow getting around this issue but will require high storage and also customization would be restricted. 
Vector tiles is a developing technology that would allow to serve high performing and customizable. 

To display vector tiles we will need two types of files
Style: A JSON style specification which describes how your map looks like
Data: Vector Tiles as data source for your style

Software Stack and Process
^^^^^^^^^^^^^^^^^^^^^^^^^^

**Creating and serving vector tiles will require following tools**

- Ogr2org from the GDAL package to convert the shapefile to geojson
- Tippecanoe - a command line tool to convert geojson to mbtiles
- Maputnik - a visual editor to create map styles for MapboxGL specification
- Tileserver - to serve the generated tiles
- MapboxGL - to display the generated tiles


**The process of converting the shapefiles to vector tiles**

1. Before using tippecanoe, you need to transform your data into EPSG:4326 coordinate system. We can use ogr2ogr utility which is part of gdal.

    ogr2ogr -f GeoJSON your_data_in_4326.json -t_srs EPSG:4326 your_data.shp
2. Having your data in correct coordinate system, we can do the conversion using tippecanoe.

    tippecanoe -o your_data.mbtiles your_data_in_4326.json

3. It will convert your data into MBTiles for zoom levels 0 to 14. This is the most simple use case and Tippecanoe enables much more sophisticated options for which we can check the documentation. https://github.com/mapbox/tippecanoe#options
4. Style files can be generated using the Maputnik style editor. https://github.com/maputnik/editor
5. The tileserver will now host the map tiles. It can use used from a docker image docker 

    run --rm -it -v $(pwd):/data -p 8080:80 klokantech/tileserver-gl

    It is also available as a npm package. Docs for tileserver is available at https:// tileserver.readthedocs.io/en/latest/index.html
6. Mapbox GL JS is a web mapping library based on WebGL. Mapbox GL JS can be used for rendering the vector tileset.

Outputs
^^^^^^^

We will have output file of 70 spices which will be provided as shapefiles.

Size of the outputs (for zoom level 1 to 14)

- Base map of OpenStreetMap for Nepal can be stored in about 170 MB
- The output of HLZ classification can be stored in about 10 MB
- The output of species distribution modeling can be stored at about 1 MB

