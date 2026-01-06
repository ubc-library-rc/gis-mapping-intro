---
layout: default
title: Project Set-up
nav_order: 7
has_children: true
---
# Project Set-up
{: .no_toc}
**Learning Objective 4: Be familiar with the QGIS interface, having downloaded the software and practiced setting up a QGIS project.**

This page demonstrates how to open & save a QGIS project as well as navigate the QGIS interface.

<details open markdown="block">
  <summary>
    On this page:
  </summary>
  {: .text-delta }
 - TOC
{:toc}
</details>




## Open & Save a new QGIS project
QGIS can be opened by opening a prepared QGIS project file, or simply by launching the application. For this introductory tutorial, a project has been prepared for you with some practice data for your exploration. 

To Do
{: .label .label-green }
Download the folder below to a location on your physical computer, such as Desktop or Downloads (do *not* download to OneDrive). Then, **unzip it**.  

[Download Data](../gis101-tutorial.zip){: .btn .btn-blue }

Unzipping the folder is important as this is the only way to access it's contents. Inside the unzipped folder `gis101-tutorial` there will be a file called `tutorial-project_YOURNAME.qgz`. This is a QGIS project. Double click it or right-click and choose to open it with QGIS. 

<!-- 
If you have successfully downloaded and installed QGIS, the application should open and look like this:


<img src="./images/qgis-new-empty-project.png" style="width:100%">

 Note that even though a project was prepared for you, because it doesn't have any data loaded into it yet, QGIS considers it an empty project.  Double click “New Empty Project” to open a new QGIS project. (If nothing changes, that's okay! Once you add data everything will be fine.) -->


To Do
{: .label .label-green }
To save your project, navigate to the `Project` Menu at the stop of your screen and go down to "Save As". Save the project to a location on your physical computer (such as Desktop or Downloads) and give it a name such as `tutorial-project_FirstnameLastname`. It's best practice to save your QGIS projects to the folder where you keep your data for the project. Once you save your project to your computer, you'll notice the file extension is `.qgz`. Learn more about QGIS file formats [here](https://docs.qgis.org/3.34/en/docs/user_manual/appendices/qgis_file_formats.html). 

<img src="./images/qgis-save-as.png" style="width:100%">

It is important to regularly save your project while working in QGIS by clicking the "Save" option. Just like with documents in a text editor, you can always "Save As" to save your project as a new file, thus creating multiple back-up versions of an original. 

You can also use the <img src="./images/save-tool.png" style="width:10%"> in your **Toolbar** to save your project regularly. 

<br>

## Navigate the Graphical User Interface (GUI) 
<img src="./images/qgis-interface.png" style="width:100%">

- **Menus** - At the very top of your screen you’ll see menus which, when clicked on, expand to show many more options and even sub-menus. Notice that these menus are only visible when you’ve clicked into the QGIS application. Though you can drag the application interface around your screen, the menus stay at the top. If you click out of the QGIS application, the menu will disappear. These menus provide easy access to a variety of tools you’ll use in your everyday mapping. Like any new interface, it may take some time to become familiar with what’s stored where.

- **Toolbars** - The toolbar is the area at the top of your QGIS application with all the icons. The toolbar actually contains multiple toolbars, which are groups of icons that, when clicked, allow you to navigate around your map canvas, make click-based selections, edit layer geometries, create spatial bookmarks, and much more. You can customize this area of your GUI to fit your needs, adding and removing sets of tools by clicking on the great area of the toolbar.

- **Browser and Layers Panel** - When you open the project prepared for you, you should see two panels on the left-hand side of your interface. The browser panel lets you easily navigate your file system for data and project files. Your layers panel displays your project’s data layers and provides access to configuration settings. If you ever accidentally close a Panel, you can open it again by going to the View menu at the top of your screen, down to Panels, and then selecting the ones you wish. You can also right-click anywhere in the toolbar’s greyspace and select the Panels and Toolbars you want to show or hide.

- **Status Bar** - The status bar displays current information about the map canvas, and allows you to make adjustments in the map’s scale and rotation.

- **Map Canvas or Map View** - Call it either one. This is where the map is displayed and updated as layers are loaded. You can zoom/pan the map canvas as well as select features and other operations.


To Do
{: .label .label-green }
Notice there is a layer in the Layers Panel called `vancouver-neighborhoods`. It's visibility is currently turned off. Click the box next to it to turn it on. If nothing shows up on your Map Canvas, right-click (control click) the layer and choose "Zoom to Layer(s)" from the top of the pop-up menu. Your screen should now look like the image below.

<img src="./images/explore-qgis-interface.png" style="width:100%"> 

<br>

> <img src="./images/zoom-tools.png" style="width:34%"> Take a moment to zoom in and out using the **Magnification tools** in your **Toolbar**.  


> <img src="./images/identify-tool.png" style="width:7%;"> Use the **Identify tool** to look up the names of different neighborhoods. To use the Identify tool, click the tool icon in the **Toolbar**, then click on any neighborhood polygon. 

<img src="./images/identifying-neighborhoods.png" style="width:100%"> 


> <img src="./images/pan-tool.png" style="width:7%"> To stop the Identify tool, close the pop-up window and click the **Pan tool**. 

<br>

## Customizing the interface
You can change the look and feel of your GUI, as well as adjust default settings from the menu **QGIS-LTR --> Preferences** or the menu **Settings --> Options.** Both menus are located at the top of your screen when QGIS is open and the application is active (meaning you've clicked anywhere on it). 

The application Options window looks like the image below. Most customizations you'll want to make at this stage will be under "General".     

<img src="./images/application-options.png" style="width:100%">



- **Light and Dark mode** - So long as your Style is set to Fusion and UI Theme is set to default, whether your QGIS application is light or dark depends on whether your computer System Settings have Appearance as light or dark. If you change your computer's Appearance settings, be sure quit (saving first, of course) and re-open your QGIS project for the changes to take effect. 

- **Increasing font and icon size** - Make sure to resize the Options dialogue window so you can see the drop-down for "icon size" and "font". (It is particularly difficult to see QGIS drop-down and close window icons in dark mode.) Now you can increase the font and/or icon size. Icon changes will happen as soon as you click OK. Changes in font size won't update until you quit and restart QGIS, so make sure you save your project now. 

<br>



## Loading Data 
Once you've acquainted yourself with the QGIS interface, it's time to add some data to your project. Vector and raster data has been prepared for you in the `data` subfolder of the `gis101-tutorial` folder you already downloaded and unzipped. The data within is all from the [City of Vancouver Open Data Portal](https://opendata.vancouver.ca/pages/home/), though modified slightly in preparation for your use.
 

### Understanding your data
{: .no_toc}

If you open the `data` subfolder from your computer, you will see a list of files with various file extensions:

<img src="./images/data-subfolder.png" style="width:70%;">

You might remember some of these file extensions from the page on spatial data. 
- `BCVANC15_M11.tif` is an aerial photo of a small area around Granville Bridge. As you can see in the screenshot above and on your own computer, this file is by far the largest in size. That's because it is raster data, and raster data is a grid of continuous pixels rather than a few points and vertices between them. Because of the size of aerial imagery, rather than downloading imagery for the entire city at once, you have to download it in small sections. Indeed, the true file size was over 100MB so the original file was cropped to show an even smaller area. Browse more imagery [here](https://opendata.vancouver.ca/explore/dataset/orthophoto-imagery-2022/information/). You'll also notice the file `BCVANC15_M11.tif.aux.xml`. This is a metadata file that includes statistics about each band of the raster. You don't need to know more now, just make sure to keep these two files together. 

- `cottonwood-street-trees.geojson` is a geoJSON of cottonwood street trees across the city. This is vector data comprised of points. You'll notice it has an attendant markdown file, `cottonwood-street-trees.qmd`. Again, you can ignore that for now—it just contains metadata—but be sure it stays with the geoJSON file. 
If you look at it from your computer - you'll recognize the file extensions - vector - shapefile and geojson and a tiff - sattelite imagery. 

- `street-network.geojson` is a vector dataset containing streets of Vancouver. Actually, it contains the street network for only a portion of the city as there are many many streets and thus to include data for the entire city would create a huge file. When you load this data to your project, you'll notice it takes a long time to load as it is. 

- You'll notice there are quite a few files for `vancouver-neighborhoods`, a data layer *already added* to your project. This is because the vector data for Vancouver neighborhoods is stored in shapefile format. `vancouver-neighborhoods.shp` is all you need to add to your project. The side-car files are only visible when viewing the data from your computer's finder window. As you will see shortly, if you load a shapefile from within QGIS, only one file is visible. 

- Finally, `vancouver-parks.geojson` is a geoJSON file containing vector data on city parks. 


### Loading data to QGIS
{: .no_toc}

There are a couple ways to add data to your map canvas. 

- **Browser panel** From the Browser panel, likely docked to the left of your screen, expand the `Home` directory (aka folder) and navigate to your workshop data folder. Expand that folder to see the data inside, then double-click or drag and drop each file to add it to your project. Alternatively, you can add a **Favorite** connection in the Browser panel to save you the trouble of finding your data folder. To do this, click “Favorites” at the top of the Browser panel's list and connect the workshop data folder as a favorite directory. Make sure not to click *into*, merely select it. 
- **Data Source Manager** The Data Source Manager is the same sort of portal as the Browser, just in a separate dialogue box rather than a docked panel. You can open the Data Source Manager by double-clicking the 3 colorful squares icon in the Toolbar, or from the Layer menu at the top of your screen.
- **Layer menu** A third way to add layers to your map canvas is through the Layer menu at the top of your screen. Under Layer, navigate to **Add Layer** (it should be the third item down) and select Add Vector Layer... or Add Raster Layer.... This will open the same Data Source Manager dialogue box as before.
- **Drag and drop** files from your data folder directly onto your map canvas. This method is not recommended as it can easily lead to data disorganization. 

To Do
{: .label .label-green }

Add your data files to your QGIS project:

1. `vancouver-parks.geojson`
2. `street-network.geojson` (You may have to wait a moment for it to load. Allow time for it to load before adding the next dataset.)
3. `cottonwood-street-trees.geojson`
4. `BCVANC15_M11.tif`


Save your project. Zoom out if you need so you can see all your layers loaded. 

<img src="./images/layers-loaded.png" style="width:100%">

    

Your data isn't saved _inside_ your QGIS project. Rather, the *filepath connections* are saved, as well as any modifications to symbology made to the layers in QGIS. When mapping in QGIS, it's important to keep track of where the data you're working with is stored. If you move your data, QGIS won't know where to look for it and a red exclamation mark will appear in the Layers Panel. You can click on this warning to tell QGIS where the data is now stored. 
{: .note}





## Managing Layers
Although this tutorial has only a handful of layers, some projects require you to juggle more than 10 layers. Having strategies to stay organized is therefore important. Additionally, layers that cover the entire earth are quite large and require lots of processing power to load anew each time you pan and zoom around your map canvas. Best practice is therefore to "hide" or "turn off" layers you aren't using so as not to slow your computer down. Below are some tips to stay organized.

- **Rendering order** Note that we added layers to our project in a very specific order. This is because QGIS will render layers from the top down, meaning the layers to the top of your Layers Panel list will sit above the layers below. We added the aerial photo last so it could bee seen above the other layers. You can reorder your layers at any time by dragging them up or down. 

     > Drag `cottonwood-street-trees` to the top of your layers. See how it disappears? Then drag it up again. 

- **Turning layers on and off** Turn layers on and off (or hide and show them) by clicking the little checkbox beside each layer. If you've added a layer but don't see it rendered, it is likely underneath another layer. Rather than rearranging every layer until you find it, you can successively turn each layer off until you find the one you're looking for.  

    > Turn `street-network` off. This will allow you to zoom and pan around your project more easily as your computer won't be working to re-load a large file each time. 

- **Zoom to layer** To zoom to a layer, simply right-click (control-click) any layer and select the top option to "Zoom to Layer(s)". Zooming to a layer simply centers the extent of that layer in your map canvas. Often times when you first open a QGIS project, even if data is loaded and turned on, your map canvas will appear blank. Zooming to a layer will immediately populate your screen with the loaded layers. If you zoom to any of the global layers, you will return to the global view. 

     > Try zooming to `BCVANC15_M11` (aerial photo).  

- **Renaming layers** You can rename layers in the Layers Panel. This does not change the datasets themselves, but rather their nicknames as they appear in your QGIS project. To rename a layer, simply right-click the layer in your Layers Panel and go to "Rename Layer". 

  
     > Try renaming your layers. For example, rename `vancouver-parks` to   `parks`. 


- **Grouping Layers**  If you're ever working with numerous layers, you can create layer groups through the group icon or by right-clicking anywhere that's empty in the Layers Panel and selecting "Add Group". Once you've added and named a group, you can drag layers into it. You can move layers out of a group at any time, and right-click the group to remove or rename it. Each layers group will have its own visibility checkbox, meaning that even as you set the visibility for each individual layer within the group, only by rendering the group itself visible will any of its nested layers appear on your screen. 

 <img src="./images/add-group-icon.png" style="width:7%">
   

- **Removing layers** Just as you can add layers to your QGIS project, you can remove layers at any time. This will not delete the datasets themselves; after all, they are not saved inside your QGIS project (as ArcGIS would do). Rather, it is the file connections that are saved, as well as edits to their symbology made in QGIS. To remove a layer connection from your project, simply right-click that layer in your Layers Panel and select "Remove Layer...". 

- **Checking file paths** If you are ever uncertain where a loaded layer is stored on your physical computer, hover over the layer to see its file path.

- **Refreshing Data Source**  If you add new data to your working folder already pinned as a favorite directory in your Browser Panel, you might need to "Refresh" the folder connection for the new files to appear. Simply right-click the folder connection and select "Refresh". You can also click the Refresh icon to refresh all connections. 

 <img src="./images/refresh-browser-icon.png" style="width:20%">



- **Exporting Layers** Exporting a layer essentially makes a copy of the dataset on your computer with a name, file type, and location of your choice. This can be useful if you want to make a copy of a layer, save a temporary layer as a permanent file, or save a selection as a new layer/dataset. To export a layer, simply right-click the layer, go to "Export" --> "Save Feature As...". Note that your new file will not have the same symbology, though you can copy/paste one layer's symbology to another. "Duplicating" a layer, which you can also do by right-clicking a layer in your Layers Panel, doesn't create a copy of the dataset, just adds it twice to your project. 

- **Copy/Paste Symbology** Right-click the layer whose symbology you want to copy in the Layers Panel, go to "Styles" --> "Copy Style" --> "Symbology". Then right-click the target layer, and go to "Styles" --> "Paste Style" --> "Symbology".


<!-- - **Managing data from browser panel** Note that you _can_ delete data on your computer from the Browser Panel by right-clicking the layer  (deleting files) -->

## Project Properties
You can access the Project Properties from the the **Project** menu. Open the Project Properties and click down to **CRS**. CRS stands for Coordinate Reference System, and describes the mathematics behind transforming a 3-dimensional Earth to fit on a 2-dimensional screen. A projection is part of the Coordinate Reference System, and is responsible for projecting a set of points from a 3-dimensional space onto a 2-dimensional plane. There are a variety of projections, each one preserving some characteristics of shape, area, distance, and direction, while distorting others. When choosing the best projection for your map, it is important to consider the content you are visualizing and the extent of the geographic area. Every spatial data layer comes with its own stored projection, often noted at the point of download. Note: If you don't set a projection at the start, your QGIS project will assume the projection of the first layer you add.



Setting the project CRS doesn’t change the stored projection of each layer, only how they are rendered ‘on the fly’ by QGIS. QGIS will reproject all the project layers ‘on the fly’ to match the project CRS. You can change the stored projection of layers with the Warp and Reproject Layer tools.

For more on Coordinate Reference Systems, see [here](https://ubc-library-rc.github.io/gis-georeferencing/content/projections.html) or check out our resource on [Understanding Map Projections](https://ubc-library-rc.github.io/map-projections/) for more. QGIS also has extensive documentation on [coordinate reference systems](https://docs.qgis.org/3.40/en/docs/gentle_gis_introduction/coordinate_reference_systems.html), and [pbcGIS](https://www.pbcgis.com/projection_fundamentals/) offers more background information if you're curious.
{: .note}



## Spatial Bookmarks
Another tip, especially if you're using a single layer to make a map of different locations, is to make **spatial bookmarks**. A spatial bookmark is exactly what it sounds like: a way to bookmark a canvas extent to return to layer. You can add a spatial bookmark from the bookmark icon in the **Toolbar**, from the **View menu**, or from the Spatial Bookmark tab in your **Browser Panel**. You can then set it to your map canvas, or a layer, etc. You can then save the bookmark with a name to your project (this project alone) or to your user settings (every QGIS project you ever make and open). 

<img src="./images/adding-spatial-bookmarks.png" style="width:100%">


To Do
{: .label .label-green }
Make a spatial bookmark of the aerial photo. If you've already zoomed to the provinces layer, set your spatial bookmark extent to "Map Canvas Extent". Otherwise, be sure `BCVANC15_M11` is centered on your screen first, or set the that layer as your extent. Save to Project Bookmarks. 




<br>

You are now setup to begin mapping! Be sure to **SAVE YOUR PROJECT** before continuing on. Save from either the save icon in your toolbar or from the **Project menu** --> **Save**. 






---
#### Resources for Project Setup
{: .no_toc}
- [QGIS GUI comprehensive documentation](https://docs.qgis.org/3.34/en/docs/user_manual/introduction/qgis_gui.html#qgis-gui)
- [QGIS Configuration](https://docs.qgis.org/3.34/en/docs/user_manual/introduction/qgis_configuration.html#)
- [QGIS Project Properties](https://docs.qgis.org/3.34/en/docs/user_manual/introduction/qgis_configuration.html#project-properties)