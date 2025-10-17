---
title: User Guideline LSC Hubs
date: 2023-11-20
author: Paul van Genuchten, Thaïsa van der Woude
---


This document is a guideline for usage of the Land Soil Crop hub. A [glossary](../glossary.md) is available in case terms are unclear.

## What is a Land Soil Crop hub?

Decision support tools in agronomy heavily depend on acurate environmental and crop data. 
Many data are available, but often disperse and hard to locate. Land Soil Crop hubs aim to faciliate findability 
and accessibility of relevant data. Hubs facilitate data and knowledge to be shared, processed and visualized.

The hubs describe a number of different resources relevant to the Land Soil Cop community.

- **Datasets** are either a source for predictions, as well as can be the result of a prediction.
- **Services** are offered by organizations to facilitate access to data and knowlegde. Services can vary from web services (APIs), SMS services, brochures, up to on site visits.
- Predictions on distribution of environmental parameters in time and space, as well as yield predictions, are calculated using statistical, rule based, and/or machine learning **models**. Commonly available models are described as resources in the hub. 
- In the hub various **software** components are described which enable visualisation and/or analysis of relevant data and knowledge sources
- **Approaches** describe commonly known mechanisms to improve land management to overcome challenges such as erosion, limited fertility, salinisation, and climate change.
- The hub describes relevant **policies** to the Land Soil Crop community. Policy drives the collection of data, but data can also support policy development. 

The hub does not store data or documents directly, but acts as a facility to easily discover and access information. Following the FAIR principles, the hub encourages information providers to store their works in presistent repositories, such as the
[Open Science Foundation](https://osf.io), [Datadryad](https://datadryad.org/) or [Zenodo](https://zenodo.org) and reference the publication from the hub. With every publication to a repository, the work can be identified using a persistent
identifier (typically [doi](https://doi.org), [handle.net](https://handle.net) or [ePic](https://www.pidconsortium.net/)). These identifiers are added to the hub, after which the hub will be able to present the work.

---

## User stories

The content in the hub is clustered around user stories. A user story aims to collect information and provide guidance about an actual agronomic operational challenge. Example use cases are **Soil fertility management** and **Soil water conservation**.

---

## Find data

Search for data and knowledge in the hub in various ways:

- Search by keyword or organisation
- When you click on submit, the available records will appear.
- On a search result, further limit the results by filters in the sidebar

::: {layout-ncol=2}
![Hub catalogue overview](./img/cataloguerecords.PNG){.shadow}
:::

The catalogue allows the filtering of keywords. The 3 main keywords are: 

1. category ( _such as soil, crop, etc._),
2. spatial scope (_such as Global, National, district, etc._),
3. the type (_such as dataset, software, etc_).

Second, any other keyword linked to the resource can be used to search in the catalogue, for example, _land use_ or _crop yield_. This depends on which keywords are given to the resources.

::: {.callout-tip}
Try the keywords. Type in the search bar various keywords, such as _soil or Land use_ or click on the keywords on the side.
:::

::: {layout-ncol=2}
![Filter by keyword](./img/cataloguesearch.png){.shadow}
:::

For each record, a number of metadata properties are provided, such as abstract, used datasets, keywords, usage constraints, and contact information.

Some records link directly to the [map viewer](#map-viewer) component. Under the image, it will say: Open _record_ in the LSC map and you will be directed to the map viewer.

::: {.callout-tip} 
Explore the records. Click, after searching on keywords, on one of the appeared records and explore the provided information. Click on the links in the records
:::

::: {layout-ncol=2}
![Hub catalogue record](./img/cataloguepHrecord.PNG){.shadow} 
:::

If a mapping link is available on the record, a button will appear under the map to preview the data in a map viewer.

### Contribute your data

Contact the LSC-hub team in case you want to share data via the hub. Data can best be uploaded in a persistent repository, such as [Zenodo](https://zenodo.org), the [Open Science Foundation](https://osf.io), [Harvard dataverse](http://dataverse.harvard.edu) or others. A reference to the data can then easily be added to the hub.

---

## Map viewer

Spatial data can be viewed and compared in a web-based map viewer. The map viewer can be
accessed on the homepage of the LSC hub, under _DATA_ and then click on _Go the map viewer_.
This manual provides an overview of the functionality, a full manual of the TerriaJS library
is available at [https://userguide.terria.io](https://userguide.terria.io/).

![Hub map vizualisation](./img/map.png){.w-50 .border .shadow}

The map viewer can used for the visualisation of existing maps listed in the LSC catalogue, your data and web data. In this guideline, we will take you through the available functionalities of the map viewer.

### Top menu

![mapviewer top bar](./img/mapviewer_topbar.PNG){.w-50 .border .shadow}

1. Get more information `about` the map viewer. The introduction, disclaimer and data attributes are described.
2. the `related maps` show other available maps, such as GAEZ and WAPOR. If you click on one of these maps, it will make that data available in the Table of Contents.

![mapviewer related maps](./img/mapviewer_relatedmaps.PNG){.w-50 .border .shadow}

3. `Map settings` allows you to select a different base map, such as natural earth maps or aerial maps. This depends on which base map you prefer to work with.

![mapviewer map settings](./img/mapviewer_mapsettings.PNG){.w-50 .border .shadow}

4. `Help` gives useful tips on how to use the map viewer. It provides a tour through the map viewer and a step-by-step guide. This is an interactive guideline and shows the main functionalities.

![mapviewer help](./img/mapviewer_help.PNG){.w-50 .border .shadow}
 
5. A `Story` is a function that allows you to create and share interactive stories directly from your map. It contains a video with an explanation of how to create them.

![mapviewer story](./img/mapviewer_story.PNG){.w-50 .border .shadow}

6. `Share/Print` generates a link to your created map, which you can share with colleagues. Anything you have added to the map viewer will be shown in the shareable link. You can also use this button to download your created map as an image.   

![mapviewer share](./img/mapviewer_share.PNG){.w-50 .border .shadow} 


### Vertical toolbar on the top right

The vertical toolbar allows you to zoom on the map or location, compare maps, measure distance and provide feedback. Each of the buttons will be explained below.

![mapviewer rightbar](./img/mapviewer_rightbar.png){.w-50 .border .shadow}  

1. Zoom in and out, and back to a full world zoom
2. Zoom to your current location
3. Compare two map data side-by-side. In the next section on _explore map data_, we go into more detail on this function.

![mapviewer compare](./img/mapviewer_compare.png){.w-50 .border .shadow} 

4. Measure the distance on the map between two locations.

![mapviewer measure](./img/mapviewer_measure.png){.w-50 .border .shadow} 
  
::: {.callout-tip}
Explore the basic settings of the mapviewer. Change the map settings, take the tour at the help button, download your current map, measure distances and go to your location.
:::

### The Sidebar

The sidebar is the main location for adding maps to the map viewer and visualising your data or any other web data.

   - `Search for locations` allows you to search for a specific location and go to your area of interest.
  
   ![mapviewer location](./img/mapviewer_location.png){.w-50 .border .shadow} 
     
   - `Explore map data` shows a listing of datasets that can be added to the map via a catalogue search or directly from available maps. If the panel is empty, select an alternative map from `related maps`.

  
   ![mapviewer explore](./img/mapviewer_explore.png){.w-50 .border .shadow} 

   Under the available maps, you can click on a property map to which you would like to add the viewer. It shows, for example, for the property pH, 4 maps: the 5% prediction value, the 95% prediction value, the median of predictions and the pH map.

   The values are given for pH*10 for better visualisation. Under the data preview, the metadata of the map is given. You can add the map to the map viewer by clicking on `Add to the map`.

   ![mapviewer add](./img/mapviewer_add.png){.w-50 .border .shadow} 

   You can add as many maps to the Mapviewer as you want. For example, you add another map of Organic Carbon.

   ![mapviewer add2](./img/mapviewer_add2.png){.w-50 .border .shadow} 

   If you now click on the `compare` button as described in the previous section, and put one layer to the left and the other to the right, you can compare the layers side-by-side.

   ![mapviewer compare2](./img/mapviewer_compare2.png){.w-50 .border .shadow} 

   `About data` brings you back to the Explore map Data, and shows you the metadata describing the map. The description gives in addition which datasets are used to generate the maps.
   
   - `Upload` provides the option to open a dataset from the local computer. Note that this data is not uploaded to a server, so this data is not shared with anyone else. You can also add `web data` from this panel to the map viewer.
     
   ![mapviewer localweb](./img/mapviewer_localweb.png){.w-50 .border .shadow} 

   For local files, you first need to select a file type. The file should have a spatial component and/or coordinates to add it to the map viewer. In step 2, you browse your file on your local computer.
     
   ![mapviewer local](./img/mapviewer_local.PNG){.w-50 .border .shadow} 

   For web data, you first need to select the file or web service type. In step 2, you will add the URL to add the web data. For example, you can add the ESA land cover map as a WMS layer. The URL is: <https://worldcover2020.esa.int/geoserver/gwc/service/wms?SERVICE=WMS&VERSION=1.1.1>

   ![mapviewer web](./img/mapviewer_web.png){.w-50 .border .shadow}   


   You can compare these maps with other added maps, through the compare button.
     
   ![mapviewer compare2](./img/mapviewer_compare2.png){.w-50 .border .shadow}   

    
   - As soon as layers are loaded on the map, you can set the order of the layers, view a legend of the layer, zoom to its extent, set its opacity and view the metadata of the data. 


::: {.callout-tip}  
The steps of this exercise are written down under the `help` button. By clicking on `Take the tour`, it will guide you through the steps.
:::

1. Search for a location to quickly find an area of interest
2. Use 'Explore map data' to view the catalogue of available data sets and add at least two to the map
3. Interact with the data layer, including opacity and toggling on and off on the left in your workbench, compare the maps by using the compare button
4. Click on the data on the map to view more detailed data, including the raw data
5. Change your base map using options in 'Map Settings' to help make some data sets more visible
6. Zoom and change your view, including tilting the view angle using the controls on the right-hand side of the screen

### Download data as files or from web services

Data is made available in various formats by the providers of the data. Common are file downloads in Excel, Esri Shape or GeoTiff format. Some organisations provide data access via web services. Web services enable partial downloads of a dataset, filtered by attribute, temporal or spatial extent. Common web service types are:

- **OGC:WMS** visualizes spatial data in map viewers
- **OGC:WFS** downloads a part of a vector dataset
- **OGC:WCS** downloads a part of a grid dataset

Various software is available to interect with these data formats and data services. In [this article](./ows-in-qgis.md) we explain how you can use [QGIS Desktop](https://www.qgis.org) to interact with web services for spatial data.

---

## Hub community

We welcome you to contribute to the development of the hub. The contents of the hub is maintained via a co-creation platform called [github.com](https://github.com/lsc-hubs/hub-core/). You can either directly contribute via the github platform, but a feed back mechanism is also provided on each of the hub resources. 

Providing your feedback is crucial for several reasons: 

1. Firstly, incorporating diverse perspectives from stakeholders involved in working with and benefiting from land, soil, and crop information ensures that the LSC hub caters to the actual needs and demands of its users (Data providers/Users). This feedback allows for the fine-tuning of the hub's functionalities, making it more user-friendly and effective in serving the specific requirements of different user groups.
  
2. Secondly, gathering feedback facilitates continuous improvement. It provides an opportunity to identify potential shortcomings or areas needing enhancement within the LSC hubs. Insights from stakeholders enable the developers and administrators of the hub to address any challenges faced by users, thereby refining the system to better align with the expectations and requirements of its intended beneficiaries.
  
3. Moreover, involving stakeholders in providing feedback fosters a sense of ownership and collaboration. When users feel heard and their inputs valued, it encourages their active participation and engagement with the LSC hub. This collaborative approach promotes a sense of ownership among stakeholders, leading to increased utilization and sustained support for the system in the long term.
  
4. Ultimately, the feedback obtained from diverse stakeholders during the workshop plays a pivotal role in ensuring that the LSC hub evolves as a valuable, user-centric platform, effectively supporting decision-making processes related to land, soil, and crop information in the agricultural landscape.

Every page or resource on the hub provides an option to provide feedback and/or ask a question related to the content. In these sections, you can provide feedback about the page and what you would like to be adjusted.



