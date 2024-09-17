Handwritten Note for ArcGIS Initial Tasks and Interface Overview
Lesson 1: Getting Started with ArcGIS
1. Connecting and Disconnecting Folders:

    To Connect a Folder:
        Add Data → Connect To Folder → Select Folder → Click OK or Cancel.
    To Disconnect a Folder:
        Go to Catalogue → Folder Connections → Right Click on Folder → Disconnect.

2. Adding Data and Saving for Lower Versions:

    Adding Data:
        Add Data → Select multiple datasets → Add.
    Saving for Lower Versions:
        Go to Save a Copy → Enter File Name → Choose Save as Type → Click Save.

3. ArcGIS Views and Data Frame Properties:

    Data View: Use for data analysis.

    Layout View: For creating and customizing map layouts.

    Access Data Frame Properties:
        Right-click on a layer → Properties → Data Frame Properties or Double-click on the layer.

4. ArcGIS Interface Overview (Menu Bar):

    Bookmarks: Create spatial bookmarks for easy navigation.
    Insert: Used for making map layouts.
    New Data Frame or Layers:
        Insert → Data Frame to activate a new data frame.
        Right-click on the layer → Activate.

5. Geoprocessing Options:

    Geoprocessing:
        Go to Geoprocessing Options → Check the box for Overwrite the outputs of geoprocessing operations.

6. Customizing ArcGIS Toolbars:

    Customize → Toolbars:
        Enable Tools, Standard, Layout, and Extension toolbars (Check all).
    Add-In Manager: Access Add-In manager via Customize.
    ArcMap Options:
        Mouse Wheel Drag: Customize for zoom-in.
        Zoom to Center On Display: Set zoom preferences for mouse actions.

7. Window Components and Interface Customization:

    Windows:
        Table of Contents: Access to data layers.
        Overview: Quick spatial view.
        Catalogue: For managing spatial data.
        Pin Sign: Minimize windows to the side using the Pin feature.

    Preferred Interface Customization:
        Drag Tools Toolbar to the left side.
        Catalogue, Search, Arc Toolbox: Set to Auto Hide (use the Pin icon).

    Toolbars:
        Right-click on the layer → Open the Attribute Table.

    Geoprocessing Options:
        Enable Overwrite: Must be checked.
        Background Processing: Uncheck Enable.

8. Toolbars and Data Export:

    Centering Data on Display:
        Select a layer → Right-click → Zoom to Layer.

    Selecting Data:
        Select all data from a layer: Click first data item → Shift + Click the last data item.

    Tool Components:
        Zoom In, Zoom Out, Pan, Full Extent: To fully display data on the screen.

    Selecting Features:
        Select features using the Rectangle, Polyline, or Lasso Tool.

    Clear Selected Features:
        After selecting an area, Right-click on data → Open Attribute Table.

    Creating a Subset:
        Select the area.
        Right-click on data → Data → Export Data.
        Choose Selected Features → Browse → Save as Type: Shapefile.
        Name the file (avoid spaces, e.g., ml_husian).

    Measure Tool: Used to measure distances on the map.

9. Managing Data in ArcCatalog Window:

    ArcCatalog: Used to check the metadata or details of a dataset before adding it to the working layer.

    Layer Properties:
        Right-click on data → Properties.
        Categories include General, Source, Selection, Display, Symbology, Fields, Definition Query, etc.

10. Changing Symbols and Labels:

    Changing Symbols:
        Go to Layer Properties → Symbology → Categories → Unique Values.
        Choose Value Field: Popup info → Add All Values.
        Uncheck All Other Values → Double-click on the symbol to change.

    Labeling:
        Go to Layer Properties → Labels.
        Choose Label Field → Customize Text Symbol (Font, Color, Size).
        Adjust Placement for label positions.

    Display Transparency: Adjust the transparency settings of the layers for better visual understanding.


    Definition Query and Spatial Referencing
Definition Query (Part 1)

    Road width > 2
    Road width < 2
    Road = Pucca
    Road ≠ Katcha
    Structure Katcha and Demi-pucca
    Structure used as Residential, Mixed use, and Commercial purposes
    Structure Katcha used for Residential purposes
    Structure Katcha and Semi-Pucca used as Residential purposes

Query Building for Making Subset of Data

    Steps:
        Open the data layer properties.
        Navigate to the definition query section.
        Click on query builder.
        Select Road width → set conditions like > 2 or < 2.
        Use != for not equal conditions.

Definition Query (Part 2)

    OR = Same criteria
    AND = Different criteria

Difference Between Layer and Shapefile

    Layer: A layer is a representation of spatial data. It can reference different data sources.
    Shapefile: A specific file format for storing vector data (points, lines, polygons).

Lesson 2: Spatial Referencing (Projection & Coordinate System)

    Spatial Reference, Datum, and Coordinate System
        Spatial Reference: A way to communicate location.
        Spatial Reference = Datum + Projection + Coordinate System.

    Geographic Coordinate System (WGS 84)
        Datum + Coordinate System.

    Projected Coordinate System (UTM)
        Datum + Projection + Coordinate System (e.g., UTM - Universal Transverse Mercator).

    WGS 84: World Geodetic System, established in 1984.
    UTM: Universal Transverse Mercator.

What is Projection?

    A mathematical model that converts locations from the 3D Earth surface to a 2D map.

Two Common Map Projections

    Cylindrical (Mercator/Transverse/Oblique Mercator)
    Conical (Lambert/Conformal)

Bangladesh and UTM Zones

    Bangladesh is located between UTM Zones 45 and 46, requiring a local coordinate system like BUTM.

Key Terminology

    Equator: Divides the Earth into the Northern and Southern hemispheres.
    Latitude: An imaginary line creating an angle at the Earth’s center to the Equator.
    Prime Meridian: 0° longitude; divides the Earth into Eastern and Western hemispheres.
    Longitude: An imaginary line creating an angle at the Earth’s center to the Prime Meridian.

Concept of Data Frame and Coordinate System

    New Data Frame
        To insert a new data frame:
            Go to Insert → Data Frame.

    Assign a New Coordinate System
        Double-click on the Data Frame (Layer) → Coordinate System.
        Geographic Coordinate System → World → WGS 1984 → Add to Favorite.
        Projected Coordinate System → UTM → WGS 1984 UTM Zone 45N, 46N → Add to Favorite.

Assigning BUTM (Bangladesh UTM)

    Double-click on Data Frame (Layer) → Coordinate System → New.
    Choose Projected Coordinate System.
    Name it: BUTM (Traverse Mercator).
    Set the following parameters:
        False Easting: 500,000
        False Northing: 0.000
        Central Meridian: 90.000
        Scale Factor: 0.9996
        Latitude of Origin: 0.000
    Add to Favorite.
