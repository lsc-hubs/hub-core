---
title: Implementation Guidance
date: 2023-11-13
author: Paul van Genuchten
---

This document describes a number of aspects to be considered when implementing or maintaining a Land Soil Crop system.

## Github

The software and content of the LSC hub are maintained in a [Github](https://github.com/lsc-hubs). Github is a service provider offering GIT services plus a number of add-ons to facilitate co-creation. Alternative GIT providers can be considered, such as [gitlab](https://gitlab.com) or [bitbucket](https://bitbucket.org/). 

As an LSC hub administrator it is relevant to familiarise yourself with Github. Notice that some tools exist to facilitate the use of Git, such as [Github desktop](https://desktop.github.com/), [Smartgit](https://www.syntevo.com/smartgit/), [Git Kraken](https://www.gitkraken.com/), or the [Github plugin](https://marketplace.visualstudio.com/items?itemName=GitHub.GitHubExtensionforVisualStudio) of [Visual Studio](https://visualstudio.microsoft.com/).

## LSC Hub content pages

Content pages are maintained as markdown in github and rendered by [Quarto](https://quarto.org). These pages are maintained in [github](https://github.com/lsc-hubs/hub-core). Editing of quarto documents is further facilitated by a [quarto plugin](https://quarto.org/docs/tools/vscode.html) in [visual studio](https://visualstudio.microsoft.com/).

The quarto tool is configured as a [ci-cd](https://en.wikipedia.org/wiki/CI/CD) action in github. You can follow the progress of an action in the actions tab. In some cases an action may fail and human interaction is needed to fix the problem and/or restart the action. 

## Discussions

Discussions are managed within [github](https://github.com/lsc-hubs/{{< var country >}}-hub/discussions). A [giscus widget](https://giscus.app/) is added to every resource page, so users can provide feedback or ask questions about the resource. These questions are stored as github discussions. Discussions can be answered from the resource page (a github login is required) or from github discussions. Users should be invited to the github project to be able to administer github discussions.

## Maps

The TerriaJS framework enables users to share maps and map stories with stakeholders (share button top-right). Notice that you can also use this functionality to link from a description of a resource to a map, which displays some data in a certain context.

```markdown
[A nice map](https://maps.lsc-hubs.org/#start=%7B%22version%22%...)
```

Another option is to store the map definition (urldecoded) on a folder of TerriaJS. The map is then available by its filename. You can now add a link to this map for example in the `related maps` section of TerriaJS (config.json). 

## Map services

Map services on source data are configured using [mapserver mapfiles](https://mapserver.org/mapfile/). The configuration is generated from the metadata of the source data using the [geodatacrawler](https://pypi.org/project/geodatacrawler/) tool. Mapfiles are stored on a NFS (accessible via webdav) or in the mapserver  (docker) container. Source of the mapfiles is preferably stored on Git.

Every new mapfile is registered in the mapserver config file as an [alias](https://mapserver.org/mapfile/config.html)

## Catalogue 

The catalogue can be linked to various information sources, without the data being stored on the LSC hub. Therefore, if you know existing information sources that are missing and should be added. Proving metadata is essential for findability and to avoid ambiguity. 

Source of catalogue records is maintained at [github](https://github.com/lsc-hubs/{{< var country >}}-catalogue). Records are organised in Global, Continental, and country. Within country they are organised by portal/initiative.

Metadata records are stored in the [mcf](https://geopython.github.io/pygeometa/reference/mcf/) format, a subset of iso19115 in a conveniant yaml encoding. But you can also add them as iso19115 xml format.

A number of mechanisms is available to load records into the catalogue.

- Import records from external sources, such as data portals (zenodo, dataverse, CSW, STAC, OSF)
- Mcf records can be created using [mdme](https://osgeo.github.io/mdme)
- A [Excel template](https://github.com/lsc-hubs/{{< var country >}}-catalogue/blob/main/portals/KE/LSC/index.csv) is available, on which resources can be described. A single resource per record.


