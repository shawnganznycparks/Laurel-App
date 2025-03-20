# Street Tree Planting App

This is a quick how-to regarding the Street Tree Planting App. 


# Overview
![Overview](https://raw.githubusercontent.com/shawnganznycparks/STP-Redux-App/main/STP_Overview.png)
The app has seven main panels: 

 1. Layer
 2. Legend
 3. Filter
 4. Editor
 5. Table
 6. Block Planting Tool
 7. Map

## 1. Layer
![Overview](https://raw.githubusercontent.com/shawnganznycparks/STP-Redux-App/main/Layer_1.png)

The above panel controls what is visible in the map frame. Just simply **click** the box (▢) on the left of the layer name to display it on the map.

 - [ ] Hidden Layer
 - [x]  Viewable layer

In some cases, there are groupings of layers, which is denoted by the symbol **>**.  The layer group has a Group Name, like **Data: Assets** in the above example. You can choose to **click** the box (▢) to hide/show all layers of that grouping. However, clicking **>** will expand that grouping as seen below. 

![Overview](https://raw.githubusercontent.com/shawnganznycparks/STP-Redux-App/main/Layer_2.png)

Once the grouping is expanded, the **>** turns into a **v** and will show the once hidden layers for that group. Then you can select whichever layers you want shown by clicking the box (▢). When you are done, you can just close the group by clicking **v** and it will turn into **>**. 

## 2. Legend
![Overview](https://raw.githubusercontent.com/shawnganznycparks/STP-Redux-App/main/Legend_1.png)

The legend displays all the symbology (colors/shapes) of all the layers in the application. When you click on the **≣** it will expand the symbology menu for that specific layer. 

![Overview](https://raw.githubusercontent.com/shawnganznycparks/STP-Redux-App/main/Legend_2.png)

The above image shows the **Work Orders: STP** layer's expanded symbology. Reminder, symbology is only displayed for layers that are currently visible. Otherwise **≣** will be greyed out. 

## 3. Filter
![Overview](https://raw.githubusercontent.com/shawnganznycparks/STP-Redux-App/main/Filter_1.png)

This is a basic filter for both **Street Tree Planting & Parks Planting Work Orders**. Each filter has a group **▶** and clicking on that group will expand the menu for that specific filter. 

![Overview](https://raw.githubusercontent.com/shawnganznycparks/STP-Redux-App/main/Filter_2.png)

The above shows the filter **WO: STP Contract** in its **first** expanded state. As the filter states, this one filters all STP Work Orders by specific contract(s).

![Overview](https://raw.githubusercontent.com/shawnganznycparks/STP-Redux-App/main/Filter_3.png)

This is the **secondary** expanded state, where the **WO: STP Contract** shows a list of all filterable selections. In the above photo, **BG-123M** was selected (▢). However, one more step is required to actually apply the filter to the map. 

![Overview](https://raw.githubusercontent.com/shawnganznycparks/STP-Redux-App/main/Filter_4.png)

The above photo shows the filter now in an active state. To activate a filter, simply **click** the button on the right side of **WO: STP Contract**. The color should change to green once performed correctly and now will display that particular filter on the map. 

![Overview](https://raw.githubusercontent.com/shawnganznycparks/STP-Redux-App/main/Filter_5.png)

However, you can add multiple filters on-top of each other. So, in the above example **WO: STP Contract** is activated with a selected filter, but also **WO: Status** is also activated. Meaning that **Work Orders: STP** layer now is filtered by a Contract and also Status. In this example **Contract** = **BG-123M** and **Status = Open OR Closed**.

You can put as many filters as possible on **Work Orders: STP and Work Orders: PP** by using the Filter tool. 

## 4. Editor

![Overview](https://raw.githubusercontent.com/shawnganznycparks/STP-Redux-App/main/Editor_1.png)

The editor is responsible for creating shapefiles that are unique to an individual team/borough. The use case is for Senior Foresters to create zones of interest for reference or to be used by their foresters for surveying. 

![Overview](https://raw.githubusercontent.com/shawnganznycparks/STP-Redux-App/main/Editor_2.png)

To populate the editor, you must turn on the layer in the above image by clicking the ▢.

![Overview](https://raw.githubusercontent.com/shawnganznycparks/STP-Redux-App/main/Editor_3.png)

Afterwards you'll see a list of all boroughs along with some extra projects. You can turn off/on any of the features you need/don't need. 

![Overview](https://raw.githubusercontent.com/shawnganznycparks/STP-Redux-App/main/Editor_1.png)

Once you have your features visible, the editor will populate like shown above. If you'd like to add a shape, simply click the **New Feature**. 

![Overview](https://raw.githubusercontent.com/shawnganznycparks/STP-Redux-App/main/Editor_4.png)

One **New Feature** is clicked, the editor will show as above. You are given a couple of tools to create in the toolbox under **Create features**. The default polygon tool should suffice, and you draw your polygon on the map. Once the polygon is completed (double click the last point) simply click the **Create** button to finish the polygon. 

![Overview](https://raw.githubusercontent.com/shawnganznycparks/STP-Redux-App/main/Editor_5.png)

**The polygon is now finished**. Information can be added to the polygon, like an Assignment column where each polygon has a forester name (polygon color based on forester name). If you'd like to **delete** the polygon, you can click **Select** in the editor box (shown above) and then click on the polygon you want removed.   

![Overview](https://raw.githubusercontent.com/shawnganznycparks/STP-Redux-App/main/Editor_6.png)

After clicking the polygon, you can simply click **Delete** to remove the polygon (as shown above). 

## 5. Table
![Overview](https://raw.githubusercontent.com/shawnganznycparks/STP-Redux-App/main/Table_1.png)

The table allows you to see all the rows and columns associated with the feature you're viewing. The table is interactive, with tools located on the top left and top right of the table, along with a **Total / Selection** count in the bottom left. 

![Overview](https://raw.githubusercontent.com/shawnganznycparks/STP-Redux-App/main/Table_2.png)

**Top Left:** The app with always load the attribute table for **Work Orders: STP** as the default, however if you'd like to change the attribute table to a different feature, you can click the dialogue box and a list should appear. Afterwards just select the feature of which you'd like to see the attribute table. 

![Overview](https://raw.githubusercontent.com/shawnganznycparks/STP-Redux-App/main/Table_3.png)

**Top Right** There are five buttons, the first three aren't important. The fourth one **(⇆)** allows you to control what fields are visible on the attribute table. This is useful since some features have lots of columns and if you only care to use a couple, you can deselect the columns you don't want visible.  

![Overview](https://raw.githubusercontent.com/shawnganznycparks/STP-Redux-App/main/Table_4.png)

**Top Right** The fifth button **(∷)** is the most important. Pressing the button will expand a menu giving you several options: 

 - Set Filter
	 - Allows you to set custom filters for the attribute table. Helpful if you need specific queries. 
 - Zoom to
	 - Will move frame and zoom into the map frame for the items listed in the attribute (all or selected). 
 - Pan To
	 - Will pan to items listed in attribute (all or selected) but will not zoom.
 - Statistics
	 - Can run the following statistics for a column
		 - Count
		 - Sum
		 - Min
		 - Max
		 - Avg
		 - Std Dev
 - Export
	 - Allows to export the attribute table to a JSON / CSV / GeoJSON. This is perhaps one of the most used proponents of the application to send out queried listings. 

![Overview](https://raw.githubusercontent.com/shawnganznycparks/STP-Redux-App/main/Table_5.png)

## 6. Block Planting Tool



## 7. Map





