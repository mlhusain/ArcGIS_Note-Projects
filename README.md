Lesson 1: Getting Started with ArcGIS
________________________________________
1. Connecting and Disconnecting Folders:
•	To Connect a Folder:
1.	Add Data → Connect To Folder → Select Folder → Click OK or Cancel.
•	To Disconnect a Folder:
1.	Go to Catalogue → Folder Connections → Right Click on Folder → Disconnect.
________________________________________
2. Adding Data and Saving for Lower Versions:
•	Adding Data:
1.	Add Data → Select multiple datasets → Add.
•	Saving for Lower Versions:
1.	Go to Save a Copy → Enter File Name → Choose Save as Type → Click Save.
________________________________________
3. ArcGIS Views and Data Frame Properties:
•	Data View: Use for data analysis.
•	Layout View: For creating and customizing map layouts.
•	Access Data Frame Properties:
o	Right-click on a layer → Properties → Data Frame Properties or Double-click on the layer.
________________________________________
4. ArcGIS Interface Overview (Menu Bar):
•	Bookmarks: Create spatial bookmarks for easy navigation.
•	Insert: Used for making map layouts.
•	New Data Frame or Layers:
o	Insert → Data Frame to activate a new data frame.
o	Right-click on the layer → Activate.
________________________________________
5. Geoprocessing Options:
•	Geoprocessing:
o	Go to Geoprocessing Options → Check the box for Overwrite the outputs of geoprocessing operations.
________________________________________
6. Customizing ArcGIS Toolbars:
•	Customize → Toolbars:
o	Enable Tools, Standard, Layout, and Extension toolbars (Check all).
•	Add-In Manager: Access Add-In manager via Customize.
•	ArcMap Options:
o	Mouse Wheel Drag: Customize for zoom-in.
o	Zoom to Center On Display: Set zoom preferences for mouse actions.
________________________________________
7. Window Components and Interface Customization:
•	Windows:
o	Table of Contents: Access to data layers.
o	Overview: Quick spatial view.
o	Catalogue: For managing spatial data.
o	Pin Sign: Minimize windows to the side using the Pin feature.
•	Preferred Interface Customization:
1.	Drag Tools Toolbar to the left side.
2.	Catalogue, Search, Arc Toolbox: Set to Auto Hide (use the Pin icon).
•	Toolbars:
o	Right-click on the layer → Open the Attribute Table.
•	Geoprocessing Options:
o	Enable Overwrite: Must be checked.
o	Background Processing: Uncheck Enable.
________________________________________
8. Toolbars and Data Export:
•	Centering Data on Display:
1.	Select a layer → Right-click → Zoom to Layer.
•	Selecting Data:
o	Select all data from a layer: Click first data item → Shift + Click the last data item.
•	Tool Components:
o	Zoom In, Zoom Out, Pan, Full Extent: To fully display data on the screen.
•	Selecting Features:
o	Select features using the Rectangle, Polyline, or Lasso Tool.
•	Clear Selected Features:
o	After selecting an area, Right-click on data → Open Attribute Table.
•	Creating a Subset:
1.	Select the area.
2.	Right-click on data → Data → Export Data.
3.	Choose Selected Features → Browse → Save as Type: Shapefile.
4.	Name the file (avoid spaces, e.g., ml_husian).
•	Measure Tool: Used to measure distances on the map.
________________________________________
9. Managing Data in ArcCatalog Window:
•	ArcCatalog: Used to check the metadata or details of a dataset before adding it to the working layer.
•	Layer Properties:
o	Right-click on data → Properties.
o	Categories include General, Source, Selection, Display, Symbology, Fields, Definition Query, etc.
________________________________________
10. Changing Symbols and Labels:
•	Changing Symbols:
o	Go to Layer Properties → Symbology → Categories → Unique Values.
o	Choose Value Field: Popup info → Add All Values.
o	Uncheck All Other Values → Double-click on the symbol to change.
•	Labeling:
o	Go to Layer Properties → Labels.
o	Choose Label Field → Customize Text Symbol (Font, Color, Size).
o	Adjust Placement for label positions.
•	Display Transparency: Adjust the transparency settings of the layers for better visual understanding.
________________________________________
This note captures the essential steps for getting started with ArcGIS, including folder connections, adding data, customizing toolbars, geoprocessing options, and data export processes.

Handwritten Note for Definition Query and Spatial Referencing
________________________________________
Definition Query (Part 1)
1.	Road width > 2
2.	Road width < 2
3.	Road = Pucca
4.	Road ≠ Katcha
5.	Structure Katcha and Demi-pucca
6.	Structure used as Residential, Mixed use, and Commercial purposes
7.	Structure Katcha used for Residential purposes
8.	Structure Katcha and Semi-Pucca used as Residential purposes
Query Building for Making Subset of Data
•	Steps:
1.	Open the data layer properties.
2.	Navigate to the definition query section.
3.	Click on query builder.
4.	Select Road width → set conditions like > 2 or < 2.
5.	Use != for not equal conditions.
________________________________________
Definition Query (Part 2)
•	OR = Same criteria
•	AND = Different criteria
________________________________________
Difference Between Layer and Shapefile
•	Layer: A layer is a representation of spatial data. It can reference different data sources.
•	Shapefile: A specific file format for storing vector data (points, lines, polygons).
________________________________________
Lesson 2: Spatial Referencing (Projection & Coordinate System)
1.	Spatial Reference, Datum, and Coordinate System
o	Spatial Reference: A way to communicate location.
o	Spatial Reference = Datum + Projection + Coordinate System.
2.	Geographic Coordinate System (WGS 84)
o	Datum + Coordinate System.
3.	Projected Coordinate System (UTM)
o	Datum + Projection + Coordinate System (e.g., UTM - Universal Transverse Mercator).
4.	WGS 84: World Geodetic System, established in 1984.
UTM: Universal Transverse Mercator.
________________________________________
What is Projection?
•	A mathematical model that converts locations from the 3D Earth surface to a 2D map.
________________________________________
Two Common Map Projections
1.	Cylindrical (Mercator/Transverse/Oblique Mercator)
2.	Conical (Lambert/Conformal)
________________________________________
Bangladesh and UTM Zones
•	Bangladesh is located between UTM Zones 45 and 46, requiring a local coordinate system like BUTM.
________________________________________
Key Terminology
•	Equator: Divides the Earth into the Northern and Southern hemispheres.
•	Latitude: An imaginary line creating an angle at the Earth’s center to the Equator.
•	Prime Meridian: 0° longitude; divides the Earth into Eastern and Western hemispheres.
•	Longitude: An imaginary line creating an angle at the Earth’s center to the Prime Meridian.
________________________________________
Concept of Data Frame and Coordinate System
1.	New Data Frame
o	To insert a new data frame:
	Go to Insert → Data Frame.
2.	Assign a New Coordinate System
o	Double-click on the Data Frame (Layer) → Coordinate System.
o	Geographic Coordinate System → World → WGS 1984 → Add to Favorite.
o	Projected Coordinate System → UTM → WGS 1984 UTM Zone 45N, 46N → Add to Favorite.
________________________________________
Assigning BUTM (Bangladesh UTM)
1.	Double-click on Data Frame (Layer) → Coordinate System → New.
2.	Choose Projected Coordinate System.
3.	Name it: BUTM (Traverse Mercator).
4.	Set the following parameters:
o	False Easting: 500,000
o	False Northing: 0.000
o	Central Meridian: 90.000
o	Scale Factor: 0.9996
o	Latitude of Origin: 0.000
5.	Add to Favorite.

Handwritten Note for Projection and Data Management in ArcGIS
________________________________________
1. Projection Definition and Changes
Assign Projection
•	Adding a Basemap:
o	Add Data → Add Basemap → Right-click on Basemap → Ungroup → Uncheck Reference.
•	Define Projection:
o	Search → Define Projection (Data Management) → Input Feature Class (e.g., Sundarban) → Set Coordinate System to WGS 1984 → Click OK.
•	Change Projection from WGS 1984 to BUTM:
o	Search → Project (Data Management) → Input Dataset (e.g., Sundarban) → Output Coordinate System: BUTM → Save as "sundarban_butm.shp" → Click Save.
________________________________________
2. Troubleshooting: Unknown Spatial Reference
•	When a .shp file is created, a .prj file is automatically created.
Problem: If the .prj file is deleted, it will show Unknown Spatial Reference.
•	Solution: Ensure each dataset has a .prj file. If missing, define the projection again using Define Projection.
•	Fixing Coordinate System:
o	Search → Define Projection (Data Management) → Input Feature Class (e.g., Sundarban) → Set Coordinate System.
________________________________________
3. Managing Data Projection Using Add-ins
•	Close GIS software before installing Add-ins.
•	Add-ins are useful for checking the projection of all data at once.
•	To install:
o	Customize Menu → Customize Mode → Command → Search for "Spatial Reference" → Drag GISNuts: Spatial Reference Info to the toolbar.
________________________________________
Lesson 3: Spatial Data, Data Types, and Formats
Data Types:
•	Raster: Data represented in cells (e.g., JPEG, GIF, PNG, TIFF).
•	Vector: Data represented as points, lines, polygons (e.g., Shapefiles, Geodatabases).
File Formats:
•	Raster: JPEG, GIF, PNG, TIFF.
•	Vector:
1.	Shapefiles.
2.	File Geodatabases.
3.	Personal Geodatabases.
•	File Size Comparison:
o	File Geodatabase < Shapefile < Personal Geodatabase.
Shapefile Components:
1.	.shp file = Feature class (geometry).
2.	.prj file = Projection information.
3.	.dbf file = Data attributes (can be opened in Excel).
________________________________________
Lesson 4: Spatial Data Preparation - Download and Processing
GIS Data Collection Methods:
•	GPS.
•	Digitizing and Georeferencing.
•	Remote Sensing.
•	Photogrammetry.
Data Collection Sites:
1.	Geofabrik: download.geofabrik.de.
2.	Maps.barc: maps.barcapps.gov.bd.
3.	State Silk: statesilk.com.
4.	OpenStreetMap: openstreetmapdata.com.
________________________________________
Steps for Data Processing in ArcGIS
Clip Tool (Example: Clipping Sundarban):
•	Step 1: Define query on reference data:
1.	Double-click on BD_District → Definition Query → Query Builder.
2.	Double-click Admin2Name → Use Equal Sign (=) → Select Sunamganj → Apply.
•	Step 2: Clip data:
1.	Geoprocessing → Clip.
2.	Input Features (e.g., gis_osm_road_free_1).
3.	Clip Feature: BD_District → Set output feature class and save.
________________________________________
Downloading and Processing OpenStreetMap (OSM) Data
•	Download from Geofabrik:
o	Geofabrik.de > Asia > Bangladesh.
•	Barc Maps:
o	Download from maps.barcapps.gov.bd → LRI Shapefile → Unzip → Assign coordinate and projection.
•	HDX (Humanitarian Data):
o	data.humdata.org.
•	Diva GIS:
o	diva-gis.org.
•	ESRI-GIS Hub:
o	hub.arcgis.com.
•	USGS (Remote Sensing Data):
o	earthexplorer.usgs.gov.
•	Earth Data (NASA):
o	search.earthdata.nasa.gov.
________________________________________
Google My Maps Survey: Creating and Exporting KML/KMZ
1.	Create Survey:
o	Double-click on data → Open Attribute Table → Select Road Code.
o	Query Build → Use code number → Apply.
2.	Clip Data:
o	Geoprocessing → Clip → Input Features (selected road) → Output Features.
3.	Convert to KML:
o	Search → Layer to KML → Convert selected data to KML/KMZ format.
4.	Upload to Google My Maps:
o	Open Google My Maps → Create new map → Import KMZ file → Add layers, share, and preview.
________________________________________
Processing KML/KMZ in ArcGIS
•	Convert KML to Layer:
o	Search → KML to Layer → Import KML → Set output location.
•	Export Data:
o	Right-click on data → Export Data → Save as shapefile.
________________________________________
Creating Campus Map (FEC):
•	Google My Maps:
1.	Create new map → Rename → Open data table → Insert names.
2.	Search for Campus → Add markers and details → Export to KML/KMZ.
•	Processing KML/KMZ in ArcGIS:
o	Search → KML to Layer → Import KML → Set output location.
o	Insert new data frame → Assign Coordinate System → Export data to the desired format.
________________________________________
This note summarizes the projection processes, spatial data handling, and KML/KMZ processing within ArcGIS and Google My Maps.

