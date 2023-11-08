## projections
* 53015
* 8859
--> Vector - Indicatrix mapper
## basics
* vector files
* raster files
* processing toolbox
* models

## hands on qgis
### general information
#### georeferencing
#### databases
* create database (spatialite)
* upload files to db
* sql --> select, make point
    ```sql
    select  id, 
            MakePoint(CAST("Y coordinate" as decimal),CAST("X coordinate" as decimal),4326) as geom 
    from deaths
    ```
### vector data
create point layer from table
#### visualize points
* single symbol
* categorized
* svg marker
* heatmap
#### analyse
* buffer
* voronoi --> count points in polygon

### raster data
* virtual raster --> make sure to place every input into a single band
    * rgb image (natural colors) --> bands 4,3,2
    * agriculture (highlight dense vegetation and monitor the health of crops) --> bands 11,8,2
* analyse
    * calculate ndvi
    * build model for savi
    * change detection (CLOUDS)
    

