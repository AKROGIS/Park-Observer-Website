This file allows me to edit the content of the index.html file in markdown.
This file is considered the source of the content for each of the sections
(aside from the header) in index.html.

To update index.html, copy/paste each of the sections from here to a
markdown to html converter and paste into the appropriate section of index.html


## Getting Started

Park Observer is an iPhone/iPad application for collecting spatial data.
It is **not** available on the app store. It is only available
to NPS users, or partners working on NPS projects. If your device has
access to the Arrowhead WiFi, then you can install the app by browsing
to the downloads page of this website using your device's browser and following
the instructions there, otherwise, see the
[Offline Installation Instruction.](../help2/install.html)

Installing Park Observer is usually the most difficult part of using
the app. After it is installed, you might be able to learn all you
need to know just using the app. A short [user guide](user_guide.html) is also available
if you want to get the most out of the features of Park Observer.

Once Park Observer is installed, you can immediately begin experimenting With
the sample survey provided with the application provided you have internet
access for the online base maps. Online basemaps are provide for testing.
Since most surveys are offline, you will need to install an [existing basemap](../maps2/)
of your survey area, or if one is not available then [create a new basemap](#new-map),
and [install](install.html#add-files) it. The GIS team is able to help create basemaps.

Before doing a real survey, you will need to either load an existing
survey that you wish to add to, or create a new empty survey from a protocol file.
A protocol file defines the features you will survey and their attributes.
It also defines additional characteristics of the survey such as how locations
are collected. You can load an [existing protocol file](../protocols2/),
or if there is not one
suitable for your survey, then you can [create a new protocol file](#new-protocol)
and [install](install.html#add-files) it.
The GIS team is able to help create protocols.


## New Survey

Coming soon.


## View Survey in ArcMap

Coming soon.


## Creating A Protocol File

The protocol file define your survey, most importantly it specifies what features that you can collect,
and the attributes of those features.
You must have a protocol file to create a survey and collect data.

The easiest way to create a new protocol is to copy one of the
[existing protocols](../protocols2/)
and then edit it to meet your needs in a text editor like Notepad,
[Notepad++](https://notepad-plus-plus.org/)
or [atom](https://atom.io/) (do not use MS Word).
The [Protocol Specification](../specs/Protocol_Specification_V2.html)
is the definitive guide to the content and format of a protocol file.
The specifications closely mirror the application code, and while it is long and boring,
it is defines exactly what is allowed and what is not.
The [Protocol Guide](../specs/Protocol_Guide_V2.html) provides a more readable discussion of some
of the considerations in making a protocol file suitable for your needs.

The protocol file must be a valid [JSON](http://json.org/) file, a single misplaced comma will
cause it to fail to load in the app.
You should validate it first by using an [online validator](http://jsonlint.com/).

Once you have a valid protocol, you can use iTunes to load it onto your device.
It will then appear in the list of local protocols in your app.
If you want your protocol to appear in the list of protocols available to all users
send a request to the contact below.

The Park Observer app is not very friendly when you feed it a protocol that does not meet the specifications.
It usually just crashes without any explanation. Always thoroughly test your protocols before doing real
field work. If you have a problem, consult the specification, send a help request to the contact below.


## Creating A Base Map

Please check the list of [existing maps](../maps2/) before creating a new basemap.

Basemaps can be created in ArcMap or ArcGIS Pro.
The map is converted into a collection of small images at various scales for rapid
rendering on the device. You can use any image or vector datasets that you like in your map,
however you can **not** use proprietary online basemaps (like Google, Bing, or ArcGIS).
  
To create a basemap (aka tilecache) in ArcMap:
  1. Turn on the tool: Select ArcMap Options... in the Customize menu item. Then select the Sharing tab,
     and check the *Enable ArcGIS Runtime Tools*
  2. Assemble your map - set symbology, labeling, scale dependencies, etc. to your liking.
  3. Zoom to the full extents of the area you would like to have in the tile cache.
     To minimize file size you should make the area as small as necessary.
  4. Export the map by selecting File->Share As->Tile Package from the ArcMap menu
      1. Tile Package Tab<br>You will want to save the package to a file. Give it any name you want.
         When done, this file can be loaded into the app via iTunes.
      2. Tile Format Tab<br>You will want to leave the Tile scheme as
        *ArcGIS Online / Bing Maps / Google Maps * and Tile Format as *PNG*.
        You will want to leave this at 17 or lower, unless you have a very small survey are, and need a very
        high
        resolution of data. 5m resolution imagery will generally not look any better at more detail than level
        17.
        The higher the number, the longer the tile cache will take to generate, and the larger the tile package
        will be.
        Generating an entire park at level 17 may take several hours or more. I would experiment with small
        areas and
        low zoom levels to get a feel for how long it takes, and what zoom level gives you adequate resolution.
        Be aware each increase in zoom level will quadruple the size and time it take to generate the tile
        cache.
      3. Item Description Tab<br>As a minimum, you are required to provide a Summary and Tags.
  
  4. Load the tile cache you just created on to your device with iTunes.
     If you want the tile cache to appear in the list of basemaps available to all users,
     send a request to the contact below.
  
