---
layout: post
title:  "Welcome to Massively: The Jekyll Theme!"
date:   2017-10-31
excerpt: "Huge thanks to HTML5 UP for making this awesome template! Let's see what it can do"
image: "/images/pic02.jpg"
---



# AR for Architecture: Generate City Meshes

The ability to quickly generate meshes for any city is an effective tool for prototying and demonstrations for any architect or student, especially when combined with AR. 

In this short tutorial, we will demonstrate how to take a map in Open Street Maps, and export it to an OBJ file, which you can then import to your modelling software of choice, in my case, Unity.  

## Prerequisites:

1. A Web Browser
2. A Model Viewer (For me, Unity 2017.2)

### Quick Steps:

1. Open OpenStreetMap
2. Select area and Export to a OSM file
3. Download OSM2World viewer.
4. Import the OSM File
5. Export the OBJ File
6. Use it in Unity!

### A more in depth walk through.

This process shouldn't take long at all, perhaps 5 minutes to get you up and running with a mesh of your favourite city, what you do after that is up to you. Lets get started.

#### Find your city

Open up (OpenStreetMap)[http://www.openstreepmap.org] and find the city you are interested in using the search bar.

Start the export process by clicking Export on the top tool bar, which will start the export sidebar. You can export the enire area, or click 'Manually select a different area' to draw a smaller rectangle. Here I focus on exporting the city center area focusing on Sheffields Arts tower, and the Ponderosa Park.

<div class="img_row">
	<img style="max-height: 100%"  src="{{ site.baseurl }}/img/Blogs/Tracked_AR_Vuforia/OSM_export.PNG" alt="Exporting a OSM map" title="Export OSM"/>
</div>

When you are ready, click export, annd download the maps.osm file. 

#### Get the OSM2World viewer 

Now that we have the exported .osm map, we need to convert it into a recognisable format, that is where OSM2World viewer comes in. You can download the latest binaries at (OSM2World)[osm2world.org/download/].

This will download a zip file, which you can extract to a OSM2world folder, and run using the osm2world-windows batch file by double clicking it. This will load up a terminal, which then loads up OSM2World Viewer



<div class="img_row">
	<img style="max-height: 100%"  src="{{ site.baseurl }}/img/Blogs/Tracked_AR_Vuforia/OSM_Viewer.PNG" alt="Starting OSM2World Viewer" title="OSM2World"/>
</div>


#### Convert your Map to a Meshes

Using the OSW2World Viewer, you can import the OSM map you downloaded earlier, using:

File> Open OSM Model

And select your map, after some processing, this will show you your city mesh.

[Image: OSM_Mesh]<div class="img_row">
	<img style="max-height: 100%"  src="{{ site.baseurl }}/img/Blogs/Tracked_AR_Vuforia/OSM_Mesh.PNG" alt="Loading an OSM Mesh" title="OSM2World Mesh"/>
</div>

From here you can easily export your mesh as an .obj file, for use in your favourite modelling software, using:

File > Export OBJ File

#### Use your mesh

At this point you're free to do as you wish with your shiny new mesh. As a unity developer interested in AR, I can use this to create instant Sheffield maps appearing on the floor in front of me.

<div class="img_row">
	<img style="max-height: 100%"  src="{{ site.baseurl }}/img/Blogs/Tracked_AR_Vuforia/Unity_Sheffield.PNG" alt="Mesh In Unity" title="Unity Mesh"/>
</div>

In a few short minutes, you can follow (Augmented Reality Tutorial)[http://adamrtomkins.github.io/2018/01/05/Unity_Vuforia.html] to get up and running with a Sheffield City Mesh in AR. 

<div class="img_row">
	<img style="max-height: 100%"  src="{{ site.baseurl }}/img/Blogs/Tracked_AR_Vuforia/Unity_Sheffield_AR.jpeg" alt=Sheffield in AR" title="Sheffield_in_AR"/>
	
</div>





