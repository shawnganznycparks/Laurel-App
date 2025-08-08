# Laurel App

This is a quick how-to guide for the Street Tree Planting App.

A glossary of technical terms is available at the end of this document for users unfamiliar with certain terminology.

## Overview

![Overview](https://raw.githubusercontent.com/shawnganznycparks/STP-Redux-App/main/Intro.png)

The app has seven main panels:

1.  Layer
    
2.  Editor
    
3.  Filter
    
4.  Query
    
5.  Table
    
6.  Help
    
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

## 2. Editor

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

This tool allows foresters to efficiently track planting and survey status of city blocks through batch editing.

### 2. Editor - Block Planting Tool

The purpose of the Block Planting Tool originally was to allow updates to be performed on the sidewalks of the city, to say if they were either planted or surveyed. While, this is still true, we split Surveyed for Neighborhood Tree Planting (blocks) into two components, Surveyed and Planted. This allows the Street Tree Planting team to track, blocks that are surveyed and blocks that are planted. 

**The Block Planting App** has been replaced by the **Editing Tool** within the Laurel App, meaning there is no need for an external app to make changes to the following:
- Surveyed for Neighborhood Tree Planting: Surveyed
    - **Fields:**
    - Surveyed
        - List: Yes / No / Partial
    - Season Year
        - Text: "Season + Year" 
    - Comment
        - Text: "[insert comments]"
- Surveyed for Neighborhood Tree Planting: Planted
    - **Fields:**
    - Planted
        - List: Yes / No / Partial
    - Season Year
        - Text: "Season + Year" 
    - Comment
        - Text: "[insert comments]"

In order to edit either layer, the first step is to turn on the layer you want to edit--please only do one at a time. 

![Block Tool](https://raw.githubusercontent.com/shawnganznycparks/STP-Redux-App/main/Block_Planting_Editing_1.png)

Once your layer is visible, we can see that the **Editor** box changes and shows a couple of different options. 
    
![Block Tool](https://raw.githubusercontent.com/shawnganznycparks/STP-Redux-App/main/Block_Planting_Editing_2.png)

Here is a list of what they do: 
    1. Pan
        - Allows you to move the screen without selecting features.
    2. Select by Point
        - Allows you to select a feature (shape) at the point of the cursor.
    3. Rectangle
        - Allows you to create a rectangle by clicking, holding the left mouse button, and dragging. 
    4. Lasso
        - Allows you to create a free-hand style shape by holding the left mouse button and creating a shape. 
    5. Create New Features
        - Allows you to create a new block feature, in case one doesn't already exist. 

![Block Tool](https://raw.githubusercontent.com/shawnganznycparks/STP-Redux-App/main/Block_Planting_Editing_3.png)

Below is an example of using the Lasso tool. 

![Block Tool](https://raw.githubusercontent.com/shawnganznycparks/STP-Redux-App/main/Block_Planting_Editing_4.png)

Once you finish the shape, you'll see that the selection is highlighted in a bright blue, while the **Editor** panel shows all the features that are selected. Below is an example, and within the example we see that we have 33 different features that we are editing. So, we will press *Edit*. 

![Block Tool](https://raw.githubusercontent.com/shawnganznycparks/STP-Redux-App/main/Block_Planting_Editing_5.png)

After pressing *Edit*, we are brought to a new panel, which allows us to alter the fields as was listed previously:
1. Planted
    - List: Yes / No / Partial
2. Season Year
    - Text: "Season + Year" 
3. Comment
    - Text: "[insert comments]"

*Reminder* you can alter any blocks from any surveyed status to another. So, if it's already marked as Surveyed = Yes or Planted = Yes, you can change it to Planted = Partial, if you'd like. Anyway, once you're doine with your comments, you will press the update button and the changes should be made!

![Block Tool](https://raw.githubusercontent.com/shawnganznycparks/STP-Redux-App/main/Block_Planting_Editing_6.png)

Here is an example, of the changes being made, you'll notice that the **Editor** panel is back to showing the selected features, however the changes have been made, as you can see the highlighted blocks are now tinged a little darker due to the udnerlying asset now being dark green, which in this example means Surveyed = Yes or Planted = Yes.

![Block Tool](https://raw.githubusercontent.com/shawnganznycparks/STP-Redux-App/main/Block_Planting_Editing_7.png)

Last portion of the Block Planting integration into Laurel, is the creation of new features (sidewalks). Sometimes the data that generates the sidewalks don't get everything. In these instances you can then create new sidewalks to then record. The data will be stored and kept safe!

To start, we will press *New Feature*

![Block Tool](https://raw.githubusercontent.com/shawnganznycparks/STP-Redux-App/main/Block_Planting_Editing_8.png)

This brings up a new menu in **Editor"** where we are given a choice of how we want to create these new sidewalks: 
    1. Polyline
        - Create a point at the cursor, any new points will create a line to the previous point. 
    2. Free Hand
        - Create a line using free hand. 
        
Pretty self explanatory, I recommend going with *Polygon* creation tool since it will be a straight line. After selecting one of the creation tools, once you hover over the map, you'll see an orange dot, that would be your first point once you left click on the map.  

![Block Tool](https://raw.githubusercontent.com/shawnganznycparks/STP-Redux-App/main/Block_Planting_Editing_9.png)

Here is an example of using the *Polyline* tool. There are two vertices (points), white being the initial or previous point, and the orange being the new point. Double click the left mouse to finish building at the point where you want the sidewalk to end. 

![Block Tool](https://raw.githubusercontent.com/shawnganznycparks/STP-Redux-App/main/Block_Planting_Editing_10.png)

Once you finish creating the sidewalk, you'll get a menu to alter the field attributes of the sidewalk. Same as before, fill it out. 

![Block Tool](https://raw.githubusercontent.com/shawnganznycparks/STP-Redux-App/main/Block_Planting_Editing_11.png)

Once the sidewalk is filled out, then press *Create*.

![Block Tool](https://raw.githubusercontent.com/shawnganznycparks/STP-Redux-App/main/Block_Planting_Editing_12.png)

Once finished, you'll see that the sidewalk is now created. 

![Block Tool](https://raw.githubusercontent.com/shawnganznycparks/STP-Redux-App/main/Block_Planting_Editing_13.png)

But let's say you want to remove it. All you have to do is select the *Edit features* subpanel and select one of the selection tools and select the sidewalk. 

![Block Tool](https://raw.githubusercontent.com/shawnganznycparks/STP-Redux-App/main/Block_Planting_Editing_14.png)

Once the sidewalk is selected a new menu appears where you can edit the attributes, update, and delete. We will just be selecting delete and that should be it! 

![Block Tool](https://raw.githubusercontent.com/shawnganznycparks/STP-Redux-App/main/Block_Planting_Editing_15.png)

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

## 4. Query

The Query tool allows you to perform spatial operations, which means you can select assets like either the *TP Workorders* or *PP Workorders* if they overlap with another feature. This is useful if you need to know things that aren't normally sought or built into the fields/filters of either the STP or PP work orders. For instance, finding out how many work orders are within a certain *Capital Project*. We will explain later, but the panels menu will allow you to select what layer you want to perform a spatial operation on, see below: 

![Block Tool](https://raw.githubusercontent.com/shawnganznycparks/STP-Redux-App/main/Query_1.png)

So, what I want to do first is to make sure I enable visibility for the layers I want to perform the operations on. 
    1. I want to turn on *Work Orders: STP*
    2. I want to turn on *NYS Disadvantaged Communities (DAC)*
Then I want to use the selection tool within the map, near the *+ -*. 

![Block Tool](https://raw.githubusercontent.com/shawnganznycparks/STP-Redux-App/main/Query_2.png)

So now I have the layers visible, I want to make sure of a couple of things:
    1 / 2. Please make sure your layer is visible. 
    3. Filter Types
        - How you are going to select the features, via hand or another feature. 
    4. Filter Layer
        - If we decide on a feature, what layer is that feature called. 
    5. Relationship
        - **Intersect:** features that exist inside of other features. 
        - **Within:** features that exist within certain distance of another feature. 

![Block Tool](https://raw.githubusercontent.com/shawnganznycparks/STP-Redux-App/main/Query_3.png)

Below is an example of the filter types. There isn't a need to use the *drawn graphic* so just keep it as *selecting features from data souce*

![Block Tool](https://raw.githubusercontent.com/shawnganznycparks/STP-Redux-App/main/Query_4.png)

However, if you do choose *drawn graphic* the selection menu changes and gives you a couple of shape options. 

![Block Tool](https://raw.githubusercontent.com/shawnganznycparks/STP-Redux-App/main/Query_5.png)

*Filter layer* so here you want to select the feature you want to parse with the WO selection.

![Block Tool](https://raw.githubusercontent.com/shawnganznycparks/STP-Redux-App/main/Query_6.png)

 Originally it was DAC, but I changed my mind to do NYC City Council Districts, so in this instance we will select the NYC Council Districts feature and make sure the NYC City Council Districts layer is visible. 
 
![Block Tool](https://raw.githubusercontent.com/shawnganznycparks/STP-Redux-App/main/Query_7.png)

So, now my **Query** is set up, all that is left is to select the feature from the NYC City Council Districts layer that I want to use as the spatial filter. So, I'll use the map selection tool to select a feature from that feature layer. Aftewards I'll press *Apply* in the query window that is next to *Reset*

![Block Tool](https://raw.githubusercontent.com/shawnganznycparks/STP-Redux-App/main/Query_8.png)

The **Query** window now shows the results. So in this case, I have 949 features that were inside that City Council District feature. The window only shows 100 features per page, so I'll click the 4 circle menu in the top right of the **Query** window and you'll see it says *Loaded* and *All Data*. I want *All Data* so I'll select *Add to table* or even just *Export*, where *Add to table* will show all the features within the table of the Laurel App, while *Export* I can just create a csv.

![Block Tool](https://raw.githubusercontent.com/shawnganznycparks/STP-Redux-App/main/Query_9.png)

This is just showing the table option, which in the next section you can learn what you can do with tables!

![Block Tool](https://raw.githubusercontent.com/shawnganznycparks/STP-Redux-App/main/Query_10.png)

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
