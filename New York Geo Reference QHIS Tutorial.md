# New York in QGIS: Geo-referencing Historical Maps

[originally used Monday, April 4, 2016]

### By:  Modifications by Amber Jolly
##### Additional Modifications By: Sebastian Fuentes

### This tutorial is designed so you can practice the skills you learned in the [Programming Historian QGIS Tutorial Geo-referencing in QGIS](http://programminghistorian.org/lessons/georeferencing-qgis "Links to Programming Historian")

1.  Note for future work: Each time you install a new version of QGIS, be sure to activate the Geo-referencing toolbar in that installation

2.  Open a new project; set the CRS by typing 26918 in the filter box and choosing NAD83/UTM zone 18N EPSG:26918
![CRS Selection](http://i1092.photobucket.com/albums/i405/finbar01/CRS%20selection_zpsatjakikv.png)

3. The following data sets will need to be downloaded to create this project's data visualization. [Note: The below files will need to be downloaded to your computer.]
*  Basemaps: [http://gis.ny.gov/](http://gis.ny.gov/)
    *   For County_Shorelines.shp go to [https://gis.ny.gov/gisdata/inventories/details.cfm?DSID=927](https://gis.ny.gov/gisdata/inventories/details.cfm?DSID=927), download the NYS Civil Boundaries **SHAPE** folder.
    *   For NYS_Place_Points.shp file go to [https://gis.ny.gov/gisdata/inventories/details.cfm?DSID=930](https://gis.ny.gov/gisdata/inventories/details.cfm?DSID=930), download the NYS Place Points **SHAPE** folder.
4.  To begin, you will need to set up a modern geo-referenced visualization.
    *   Click on the Vector icon and load the downloaded Counties_Shoreline.shp [a modern shapefile] to serve as your modern geo-referenced canvas. Go to **Properties**, select **Simple Fill** and change to **Transparent**.
    *   Add Vector: NYS_Place_Points.shp
    *   Turn **Labels** on for the NYS_Place_Points files, Label with: **abc** NAME.

 ![vector layers added](http://i1092.photobucket.com/albums/i405/finbar01/vector%20layers_zpsan9fgicn.png)
5.  Download an 1800s map from [David Rumsey Map Collection](http://www.davidrumsey.com/) and save to your project folder. _My example map is ["New York State, surrounding country,"](http://www.davidrumsey.com/luna/servlet/detail/RUMSEY~8~1~20005~510001:New-York-State,-surrounding-country?sort=Pub_List_No_InitialSort%2CPub_Date%2CPub_List_No%2CSeries_No&qvq=w4s:/who%2FBurr%25252C%2BDavid%2BH.%25252C%2B1803-1875;q:New%2BYork;sort:Pub_List_No_InitialSort%2CPub_Date%2CPub_List_No%2CSeries_No;lc:RUMSEY~8~1&mi=6&trs=142) published 1832, by David H. Burr, 1803-1875.

6. Now you need to convert your map to a TIFF file.
* Right click on your JPEG file and open with **Paint**. Once in **Paint** select **Save As**, **Other Formats**, select file type **TIFF** and save.
7. Use the Georeferencer option, under the Raster menu in QGIS, to add the TIFF version as a raster layer and add 6 or more control points
* Remember to use your **Zoom** feature in the **Georeferencer** to better identify features.
* Use manmade boundaries, not coastline or rivers which can change
* Use large cities, ports, or military bases that would have had precise lat/long readings in the 1800s
* Have at least 3 in the northern part of the state
* Have more than 3 in the southern part of the state, in heavily populated areas
8.  Specify transformation settings
    *   For a refresher revisit [Georeferencing in QGIS 2.0](http://programminghistorian.org/lessons/georeferencing-qgis)
9.  Compare the geo-referenced map to modern shapefile
![Finished map](http://i1092.photobucket.com/albums/i405/finbar01/finished_zpsczus4sj4.png)

10. Now that a geo-referenced visualization has been created, it is important to think about how you might share your work with others.  The following sets provide information on using the Print Composer feature of QGIS.

11. To begin, select the *New Print Composer* option under **Project** in the toolbar menu.
* A pop-up window will appear asking you title your new print composer.

* An additional pop-up window will appear that features a blank canvas.

12. Within the new pop-up window, select *Layout*, then *Add Map* to show your geo-referenced map.
* Leave enough space at the top or bottom of the canvas.  Further below, you will be asked to insert a title of the geo-referenced map and other map features.

* Use the *Move Item Content* and *Select/Move Item* buttons to the right of the canvas as needed to adjust the now inserted geo-referenced map.

* Notice to the right of the Print Composer pop-up window there are fields within the *Item properties* window.  Review what item properties are available.  For this purpose of this activity, we added a red frame and increased the frame thickness to 2.00 mm.
![Image_001_Map Boarders](https://dl.dropboxusercontent.com/u/101767455/Print%20Composer%20Images/Image_001_Map%20Boarders.PNG)

13. Add a Title to the geo-referenced map.  May use this path in the Print Composer pop-up window [**Layout** > **Add Label**], or you may click on the icon titled *Add new label* on the left-hand toolbar.

14. Add another label and use this new label for providing a description of your map, sources used, your name, and any other information in text format you desire to have displayed.
* For this purposes of this project, we will only put the description and a name.

* Refer to Image_002_New Label fields - Title and Description.PNG for how both labels were added to the Print Composer image.
![Image_002_New Label fields](https://dl.dropboxusercontent.com/u/101767455/Print%20Composer%20Images/Image_002_New%20Label%20fields%20-%20Title%20and%20Description.PNG)
15. Besides lables, there are other features you may add to your Print Composer Image.  Those features include a:
* Scalebar to show distance
 
* Legend to show distinctions in aspects of the map displayed
* Images, if you wish to display of visual aids like photographs.

* Note: Remember, it is important when working in Print Composer, you think about your audience - those that will see and potentially use your newly created map.  You want to make sure you include as much information as necessary to both serve your purposes and at the same time, be easily viewed and understood by others.  

16. To save the printer composer file, click *Save Project* under **Composer** in the Print Composer pop-up window.

17. Now that the print composer project has been saved, you will want to also export as an Image or PDF.  In this exercise, we exported as an image.  Use this path to do so: **Composer** > **Export as Image**.  Note: When exporting as an image, you will be asked to, if you want, denote the size of the image.  You may change the size accordingly, if you know dimensions in pixels for instance, otherwise you may click okay and save to complete the process.
![Image_003_Final Print Composer Map](https://dl.dropboxusercontent.com/u/101767455/Print%20Composer%20Images/Image_003_Final%20Print%20Composer%20Map.png)
### Data sources for this tutorial
1.  Basemaps: [http://gis.ny.gov/](http://gis.ny.gov/)
    *   For County_Shorelines.shp go to [https://gis.ny.gov/gisdata/inventories/details.cfm?DSID=927](https://gis.ny.gov/gisdata/inventories/details.cfm?DSID=927), download the NYS Civil Boundaries **SHAPE** folder.
    *   For NYS_Place_Points.shp file go to [https://gis.ny.gov/gisdata/inventories/details.cfm?DSID=930](https://gis.ny.gov/gisdata/inventories/details.cfm?DSID=930), download the NYS Place Points **SHAPE** folder.
2.  Historic maps: [David Rumsey Map Collection](http://www.davidrumsey.com/)
