# Street Tree Planting App

This is a quick how-to guide for the Street Tree Planting App.

A glossary of technical terms is available at the end of this document for users unfamiliar with certain terminology.

## Overview

![Overview](https://raw.githubusercontent.com/shawnganznycparks/STP-Redux-App/main/STP_Overview.png)

The app has seven main panels:

1.  Layer
    
2.  Legend
    
3.  Filter
    
4.  Editor
    
5.  Table
    
6.  Block Planting Tool
    
7.  Map
    

Each panel of the app serves a distinct purpose to streamline street tree management and planting tasks.

## 1. Layer

The Layer panel allows users to control the visibility of data layers on the map.

![Layer](https://raw.githubusercontent.com/shawnganznycparks/STP-Redux-App/main/Layer_1.png)

This panel controls what is visible in the map frame. Simply **click** the box (▢) to the left of a layer name to display it on the map.

-   Hidden Layer
    
-   Viewable Layer
    

Some layers are grouped under a category, denoted by the symbol **>**. For example, **Data: Assets**. Clicking the box (▢) next to the group name toggles visibility for all layers in the group. Clicking **>** expands the group:

![Layer Expanded](https://raw.githubusercontent.com/shawnganznycparks/STP-Redux-App/main/Layer_2.png)

Once expanded, **>** becomes **v**. You can toggle individual layers on or off. Click **v** again to collapse the group.

## 2. Legend

The Legend panel provides a key to interpret the colors and symbols of visible map layers.

![Legend](https://raw.githubusercontent.com/shawnganznycparks/STP-Redux-App/main/Legend_1.png)

The legend displays symbology (colors/shapes) for visible layers. Clicking **≣** expands the symbology menu:

![Legend Expanded](https://raw.githubusercontent.com/shawnganznycparks/STP-Redux-App/main/Legend_2.png)

Only layers that are visible have symbology; otherwise, **≣** is greyed out.

## 3. Filter

The Filter panel helps users narrow down displayed data by specific criteria such as contract, status, or planting season.

![Filter](https://raw.githubusercontent.com/shawnganznycparks/STP-Redux-App/main/Filter_1.png)

This tool filters **Street Tree Planting** and **Parks Planting Work Orders**. Click **▶** to expand a filter group:

![Filter Contract](https://raw.githubusercontent.com/shawnganznycparks/STP-Redux-App/main/Filter_2.png)

Each filter lets you choose specific criteria. For example, selecting **BG-123M** in **WO: STP Contract**:

![Filter Selection](https://raw.githubusercontent.com/shawnganznycparks/STP-Redux-App/main/Filter_3.png)

To activate the filter, click the button next to the filter name. It will turn green when active:

![Filter Activated](https://raw.githubusercontent.com/shawnganznycparks/STP-Redux-App/main/Filter_4.png)

You can apply multiple filters simultaneously:

![Multiple Filters](https://raw.githubusercontent.com/shawnganznycparks/STP-Redux-App/main/Filter_5.png)

In this case, **Contract = BG-123M** and **Status = Open OR Closed**. You can stack as many filters as needed for **Work Orders: STP** and **Work Orders: PP**.

## 4. Editor

The Editor panel enables users to create custom shapefiles for defining zones, planning work, and assigning responsibilities.

![Editor](https://raw.githubusercontent.com/shawnganznycparks/STP-Redux-App/main/Editor_1.png)

The editor allows teams/boroughs to create shapefiles. Senior Foresters can define zones for reference or surveying.

First, enable the appropriate layer:

![Enable Layer](https://raw.githubusercontent.com/shawnganznycparks/STP-Redux-App/main/Editor_2.png)

Select boroughs or projects as needed:

![Select Features](https://raw.githubusercontent.com/shawnganznycparks/STP-Redux-App/main/Editor_3.png)

Click **New Feature** to add a shape:

![New Feature](https://raw.githubusercontent.com/shawnganznycparks/STP-Redux-App/main/Editor_4.png)

Use the default polygon tool to draw. Double-click the last point to complete. Click **Create** to finalize the shape:

![Polygon Complete](https://raw.githubusercontent.com/shawnganznycparks/STP-Redux-App/main/Editor_5.png)

You can then add attributes, like forester name. To delete a shape, click **Select**, choose the shape, then click **Delete**:

![Delete Polygon](https://raw.githubusercontent.com/shawnganznycparks/STP-Redux-App/main/Editor_6.png)

## 5. Table

The Table panel displays detailed attributes of map features, providing tools to query, analyze, and export data.

![Table](https://raw.githubusercontent.com/shawnganznycparks/STP-Redux-App/main/Table_1.png)

The table displays rows/columns of visible features. Key areas include:

**Top Left:** Change which feature's attribute table is shown:

![Change Table](https://raw.githubusercontent.com/shawnganznycparks/STP-Redux-App/main/Table_2.png)

**Top Right:**

-   **⇆** = Choose visible fields
    
-   **∷** = Opens the tools menu:
    
    -   **Set Filter** – custom queries
        
    -   **Zoom to** – zoom to selected features
        
    -   **Pan To** – pan without zoom
        
    -   **Statistics** – run count, sum, min, max, avg, std dev
        
    -   **Export** – download as JSON / CSV / GeoJSON
        

![Tools Menu](https://raw.githubusercontent.com/shawnganznycparks/STP-Redux-App/main/Table_4.png)

## 6. Block Planting Tool

This tool allows foresters to efficiently track planting and survey status of city blocks through batch editing.

![Block Tool](https://raw.githubusercontent.com/shawnganznycparks/STP-Redux-App/main/Block_1.png)

This tool tracks whether blocks are planted or surveyed.

**Top Left:** Four widgets:

1.  Layers (show work orders)
    
2.  **Batch Attribute Editor** – select/edit multiple blocks
    

![Batch Editor](https://raw.githubusercontent.com/shawnganznycparks/STP-Redux-App/main/Block_3.png)

Use the polygon/blob tool to select blocks:

![Polygon Tool](https://raw.githubusercontent.com/shawnganznycparks/STP-Redux-App/main/Block_7.png)

3.  **Political Filter** – filter by political boundaries
    
4.  **Contract Filter** – filter by contracts
    

![Contract Filter](https://raw.githubusercontent.com/shawnganznycparks/STP-Redux-App/main/Block_5.png)

Sidewalks are either green (surveyed) or black (not surveyed). Each sidewalk has an ID number:

![Sidewalk Status](https://raw.githubusercontent.com/shawnganznycparks/STP-Redux-App/main/Block_6.png)

After selection, use the menu to mark planting as **Yes**, and optionally add season, year, or comments:

![Edit Block](https://raw.githubusercontent.com/shawnganznycparks/STP-Redux-App/main/Block_8.png)

## 7. Map

The Map panel is the primary interface for viewing, interacting with, and managing geospatial data.

![Map](https://raw.githubusercontent.com/shawnganznycparks/STP-Redux-App/main/Map_1.png)

The main visual workspace. Tool locations:

**Top Right:**

-   **Search** – find WOIDs or addresses  
    ![Search Tool](https://raw.githubusercontent.com/shawnganznycparks/STP-Redux-App/main/Map_2.png)
    
-   **Basemap** – switch backgrounds  
    ![Basemap](https://raw.githubusercontent.com/shawnganznycparks/STP-Redux-App/main/Map_3.png)
    
-   **Measure** – measure distances

![Measure](https://raw.githubusercontent.com/shawnganznycparks/STP-Redux-App/main/Map_4.png)

**Top Left:** Zoom (+/-), Home button (reset view), and Select tool:

![Zoom & Select](https://raw.githubusercontent.com/shawnganznycparks/STP-Redux-App/main/Map_6.png)

**Bottom Right:** Displays selected feature count. Use the Select tool to draw a polygon and select WOs for the count to appear. 

![Select Tool](https://raw.githubusercontent.com/shawnganznycparks/STP-Redux-App/main/Map_7.png)


## Glossary

-   **WO**: Work Order
    
-   **STP**: Street Tree Planting
    
-   **PP**: Parks Planting
    
-   **Shapefile**: A geospatial vector data format
    
-   **Polygon Tool**: A digital drawing tool used to create shapes on a map
    
-   **Batch Attribute Editor**: Tool used for simultaneously editing multiple map features
