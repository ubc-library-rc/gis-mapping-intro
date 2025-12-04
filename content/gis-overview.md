---
layout: default
title: GIS Overview
nav_order: 2
has_children: true
---

# Geographic Information Systems (GIS)

GIS is an abbreviation for Geographic Information System. A nice description of GIS that provides a bit of relevancy comes from QGIS's [*A Gentle Introduction to GIS*](https://docs.qgis.org/3.10/en/docs/gentle_gis_introduction/introducing_gis.html):

  >*Just as we use a word processor to write documents and deal with words on a computer, we can use a GIS application to deal with spatial information on a computer*

With that in mind, there are 3 main forms of GISs:

 1. **Utilities and Services (tasks)** - Scripts and programming libraries that manipulate spatial data in specific ways. For example, [**geocoding**](https://desktop.arcgis.com/en/arcmap/latest/manage-data/geocoding/what-is-geocoding.htm) services geolocate a set of points based on address or coordinate attribute data. [MMQGIS](https://plugins.qgis.org/plugins/mmqgis/) is a QGIS plugin which contains a tool for geocoding. 

2. **Desktop (analyses)** - Software that provides a suite of tools for processing and spatially analyzing data. In other words, GIS applications you interact with through a graphical user interface from a computer. Examples include the QGIS desktop app we will use today and Esri ArcGIS Pro. 

3. **Infrastructure (management)** - Server and web resources that manage, curate, and distribute collections of spatial data. While Esri offers Server web services with ArcGIS Online, many [open source GIS servers](https://mapscaping.com/open-source-gis-servers/) are out there. 


<br>

There are a variety of GIS available, some proprietary and some free and open source. Free and open source means... It is for this reason that Research Commons workshops on GIS and Mapping use QGIS, a popular free and open-source GIS you can download directly to your computer. 


<br>

<img src="./images/QGIS-logo.png" style="width:30%">

[QGIS](https://qgis.org/) is a popular desktop GIS software, and considered a free and open source software (FOSS) with a very active development community.

### QGIS Advantages  ⇡

 - Free and open source 
 - Runs on Windows, Mac, Linux, Android
 - Extensive online documentation 
 - Intuitive interface
 - Active development and user communities, meaning people are constantly posing and answering questions on platforms such as Reddit and StackExchange. This makes troubleshooting a whole lot easier. 
 - Robust [plugin](https://plugins.qgis.org/) repository for extended functionality

### QGIS Disadvantages ⇣

 - Most recent features can be buggy, which is why we recommend always downloading the latest Long Term Release, often small hyperlink below main download button. 
 - Plugins lack standardized documentation as they are largely user-community developed and contributed
 - Troubleshooting often amounts to searching the web, though this is an important skill to have as a cartographer. 


### QGIS Resources 
{: .no_toc}
- UBC Research Commons has two workshops to get you started: [Intro to Map Production with QGIS](https://ubc-library-rc.github.io/gis-intro-qgis/) and [Tools and Workflows in QGIS](https://ubc-library-rc.github.io/gis-tools-workflows/). 
- QGIS itself has extensive online documentation, including a robust [User Guide](https://docs.qgis.org/3.40/en/docs/user_manual/index.html) *and* [Training Manual](https://docs.qgis.org/3.40/en/docs/training_manual/index.html). QGIS also has a vibrant user community, with answers to nearly any question you might have only a web search away. Many helpful tutorial demonstrations can be found on Youtube. [CWU Geography](https://www.youtube.com/@cwugeography3290) offers especially clear and helpful content. 



## Installing QGIS

QGIS can be downloaded from [qgis.org's Downloads page](https://qgis.org/en/site/forusers/download.html). In most cases, you'll want to download and install the **Long term release** instead of the latest release. This will give you most of the functionality you'll need without encountering the software bugs of newly released versions.

To Do
{: .label .label-green }
Install QGIS for your operating system. 

<img src="./images/download-qgis-mac.png" style="width:90%">
<img src="./images/download-qgis-windows.png" style="width:90%">

    
    
<br>

### Troubleshooting
If you're working on a MacOS and get the message: _"QGIS-LTR can’t be opened because Apple cannot check it for malicious software"_ when you try to open the application, go to System Preferences --> Security & Privacy --> General and unlock your settings. At the bottom of the dialogue box you will see an option to Open Anyway. Click that, then re-lock your settings and try again to open the QGIS-LTR application. 

<img src="./images/download-error_20230123.png" style="height:450px; width:500px;">
