
# New York in QGIS: Geo-referencing Historical Maps [originally used Monday, April 4, 2016]
### By:       Modifications by Amber Jolly
### This tutorial is designed so you can practice the skills you learned in the [Programming Historian QGIS Tutorial Geo-referencing in QGIS](http://programminghistorian.org/lessons/georeferencing-qgis "Links to Programming Historian")

1.  [Note for future work: Each time you install a new version of QGIS, be sure to activate the Georeferencing toolbar in that installation]
2.  Open a new project; set the CRS by typing 26918 in the filter box and choosing NAD83/UTM zone 18N EPSG:26918
![CRS Selection](http://i1092.photobucket.com/albums/i405/finbar01/CRS%20selection_zpsatjakikv.png)
3. Download these data sets onto you computer. 
*  Basemaps: [http://gis.ny.gov/](http://gis.ny.gov/)
    *   For County_Shorelines.shp go to [https://gis.ny.gov/gisdata/inventories/details.cfm?DSID=927](https://gis.ny.gov/gisdata/inventories/details.cfm?DSID=927), download the NYS Civil Boundaries **SHAPE** folder.
    *   For NYS_Place_Points.shp file go to [https://gis.ny.gov/gisdata/inventories/details.cfm?DSID=930](https://gis.ny.gov/gisdata/inventories/details.cfm?DSID=930), download the NYS Place Points **SHAPE** folder.
3.  Set up your modern georeferencing canvas
    *   Add Vector and load Counties_Shoreline.shp [a modern shapefile] to serve as georeferencing canvas. Go to **Properties**, select **Simple Fill** and change to **Transparent**.
    *   Add Vector: NYS_Place_Points.shp
    *   Turn **Labels** on for the NYS_Place_Points files, **Label with** abcNAME.
 ![vector layers added](http://i1092.photobucket.com/albums/i405/finbar01/vector%20layers_zpsan9fgicn.png)
4.  Download an 1800s map from [David Rumsey Map Collection](http://www.davidrumsey.com/) and save to your project folder. _My example map is ["New York State, surrounding country,"](http://www.davidrumsey.com/luna/servlet/detail/RUMSEY~8~1~20005~510001:New-York-State,-surrounding-country?sort=Pub_List_No_InitialSort%2CPub_Date%2CPub_List_No%2CSeries_No&qvq=w4s:/who%2FBurr%25252C%2BDavid%2BH.%25252C%2B1803-1875;q:New%2BYork;sort:Pub_List_No_InitialSort%2CPub_Date%2CPub_List_No%2CSeries_No;lc:RUMSEY~8~1&mi=6&trs=142) published 1832, by David H. Burr, 1803-1875._
    *   Now you need to convert your map to a TIFF file. Right click on your JPEG file and open with **Paint**. Once in **Paint** select **Save As**, **Other Formats**, select file type **TIFF** and save.
    *   Use the georeferencer to add the TIFF version as a raster layer and add 6 or more control points
        *   Remember to use your **Zoom** feature in the **Georeferencer** to better identify features.
        *   Use manmade boundaries, not coastline or rivers which can change
        *   Use large cities, ports, or military bases that would have had precise lat/long readings in the 1800s
        *   Have at least 3 in the northern part of the state
        *   Have more than 3 in the southern part of the state, in heavily populated areas
5.  Specify transformation settings
    *   For a refresher revisit [Georeferencing in QGIS 2.0](http://programminghistorian.org/lessons/georeferencing-qgis)
6.  Compare geo-referenced map to modern shapefile
![Finished map](http://i1092.photobucket.com/albums/i405/finbar01/finished_zpsczus4sj4.png)
7.  Possible: create new vector layers to capture data on the old map

# Data sources for this tutorial

1.  Basemaps: [http://gis.ny.gov/](http://gis.ny.gov/)
    *   For County_Shorelines.shp go to [https://gis.ny.gov/gisdata/inventories/details.cfm?DSID=927](https://gis.ny.gov/gisdata/inventories/details.cfm?DSID=927), download the NYS Civil Boundaries **SHAPE** folder.
    *   For NYS_Place_Points.shp file go to [https://gis.ny.gov/gisdata/inventories/details.cfm?DSID=930](https://gis.ny.gov/gisdata/inventories/details.cfm?DSID=930), download the NYS Place Points **SHAPE** folder.
2.  Historic maps: [David Rumsey Map Collection](http://www.davidrumsey.com/)
