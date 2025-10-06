---
title: Towards FAIR Data and Knowledge in Land Soil Crop hubs
Authors: Tomas Pavelka  & Paul van Genuchten  
Date: June 2025   
Version: 0.1   
---
 
Land Soil Crop-related data and knowledge are essential for understanding and improving soil health, guiding sustainable land management, informing policy, and enabling scientific progress. Yet, these resources are often scattered, poorly documented, hard to access, or locked in incompatible formats. This fragmentation hampers their reuse, reduces their impact, and creates inefficiencies across projects and disciplines. 

This strategy, developed within the Land Soil Cropa and SoilWise projects, provides guidance to data and knowledge providers to ensure that all data and knowledge generated, collected, or reused are managed according to the [FAIR principles](https://go-fair.org) – Findable, Accessible, Interoperable, and Reusable. Data and knowledge assets which are archived using the FAIR principles will automatically be integrated in Land Soil Crop hubs.

This document has two parts. The first part provides an overview of a stepwise approach to adopt FAIR practices in data and knowledge management. The second part introduces some specific use cases, and how FAIR strategy can be implemented in those cases.


#  Approach: How to FAIRify Data and Knowledge 

By applying the FAIR principles, we can increase the visibility and value of land, soil, crop-related data and knowledge. FAIRness enables: 

- Transparency – allowing others to understand how data were produced and under what conditions.   
- Collaboration – making it easier to combine datasets across projects, regions, and domains.   
- Efficiency – reducing duplication of efforts and enabling the reuse of existing data.   
- Impact – enhancing the potential for innovation, decision support, and long-term use of project outputs. 
  
Metadata play a central role in this process: without clear and rich metadata, data and knowledge can not be truly findable or reusable. Metadata describe the context, origin, structure, and conditions of use of the data or knowledge asset, acting as the bridge between producers and users — whether human or machine. 

We recommend the following stepwise process for implementing FAIR principles in the scope of a research project or field campaign: 

## Step 1: Inventory & Typology 

* Identify what data and knowledge will be used as source and created.   
* Classify them by type, format, origin, and reuse potential.   
* Remember that the goal is to sustain the results after the end of the project.     

## Step 2: Metadata Design and Management 

* Define what metadata are needed to describe the content, origin, context, quality, and terms of use of your data or knowledge assets.    
* Use community standards to ensure consistency and interoperability — e.g., [Dublin Core](https://dublincore.org/), [ISO 19115](https://www.iso.org/standard/53798.html), [DataCite](https://datacite.org/), or discipline-specific schemas.    
* Ensure metadata are machine-readable and structured to support automated indexing and discovery.   
* Assign persistent identifiers (PIDs) to data objects, documents, and authors whenever possible — e.g. [DOIs](https://www.doi.org/) for datasets, [ORCIDs](https://orcid.org/) for researchers.    
* Use metadata to interlink related resources — e.g., link datasets to the methods used to generate them, to derived visualizations, or to policy reports where they are cited.   
* Document metadata using common formats such as XML, JSON-LD, or RDF to support integration with data catalogues and search engines.   
* Note that, in most cases, you can create metadata directly in the trustworthy repository during the resource upload.    
   

## Step 3: Choose Trustworthy Repositories 

* Use trusted platforms for archiving and sharing, such as: [Harvard dataverse](https://dataverse.harvard.edu/), [Open Science foundation](https://osf.io), [Zenodo](https://zenodo.org/).   
* Prefer repositories that support persistent identifiers (e.g., DOI), machine-readable metadata, and open licenses.   
* Remember that FAIR doesn’t necessarily mean open. In most repositories, you can also safely store resources with restricted access.   
   

## Step 4: Choose Open and Standardized Formats 

* Use non-proprietary, open formats whenever possible (e.g., CSV instead of Excel, GeoJSON instead of shapefile, PDF instead of DOCX, SQLITE over MS Access).   
* Ensure that data formats are machine-readable and suitable for long-term access.   
* If needed, add a readme.txt to the zip file with the data, providing clear documentation, definitions and relevant software compatibility notes.   
   

## Step 5: Use Controlled Vocabularies and Ontologies 

* Apply standardized vocabularies or code lists (e.g., [AGROVOC](https://agrovoc.fao.org/browse/agrovoc/en/), [GEMET](https://www.eionet.europa.eu/gemet/en/about/)) to describe data content and context.     
* If possible, avoid creating new vocabularies and ontologies. When local or project-specific terms are used, provide crosswalks or mappings to widely used vocabularies.    
   

## Step 6: Define Licensing and Access Conditions 

* Clearly specify the terms under which data and knowledge can be reused (e.g., [Creative Commons licenses](https://creativecommons.org/licenses/)). Always use already existing, standardised licences.   
* Choose the most open license possible, while respecting privacy, ethical and legal constraints.   
* Provide machine-readable licensing information in metadata (e.g., [cc-by-4.0](https://creativecommons.org/licenses/), [cc0](https://creativecommons.org/public-domain/cc0/)).   
   

## Further reading.

For more information on FAIR principles, you can visit guides at e.g. [OpenAIRE](https://www.openaire.eu/how-to-make-your-data-fair) or  [go-fair.org](https://www.go-fair.org/fair-principles/), or you can test your resource FAIRness at [FAIR Data Self-Assessment](https://ardc.edu.au/resource/fair-data-self-assessment-tool/) or [FAIRsFAIR](https://www.fairsfair.eu/tools-software) tools. See also the related official Horizon 2020 documents, [Guidelines on FAIR Data Management in Horizon 2020](https://ec.europa.eu/research/participants/data/ref/h2020/grants_manual/hi/oa_pilot/h2020-hi-oa-data-mgt_en.pdf), and [Guidelines to the Rules on Open Access to Scientific Publications and Open Access to Research Data in Horizon 2020](https://ec.europa.eu/research/participants/data/ref/h2020/grants_manual/hi/oa_pilot/h2020-hi-oa-pilot-guide_en.pdf). 

 
# Use cases FAIR data and knowledge management

## Store reports in a knowledge repository

There are various reasons why relevant reports are incidentally not deposited in a library. It is relevant to identify
and prevent these reasons, so all relevant information is carefully archived. [Read more](./reports-in-repos.md).

## Enrich (legacy) soil data with column level metadata  

Many soil data is stored in tabular form, where each column represents an observed property (Texture, Bulk density, Organic matter) for a soil sample. The exact property, its unit of measure and observation procedure are often described in related reports. This use case proposes to store that metadata close to the data, so this information is easily accessible for both humans and machines. [Read more](./tabular-data.md).

## Glossary alignment in multi disciplinary teams

The effective use of vocabularies and glossaries is critical in multi disciplinary teams to ensure interoperability, clarity, and reuse of data and knowledge. This use case outlines best practices for the creation, adoption, and maintenance of vocabularies. [Read more](./vocabularies.md).

## Knowledge hubs and websites

Project websites and especially knowledge hubs developed in (funded) projects have a tendency to contain unique information which is not available elsewhere on the web. Due to the limited project timeline, the websites and hubs tend to be unmaintained after the project, handed over to a second party, abandoned or discontinued. If not carefully archived this unique information has a high risk of being lost. A progress report typically aims to reference a specific state of the deliverable, which is difficult if the content of the system is dynamic. For both scenario's, it is of interest to persist the state of the system at intervals, but at least at project finalisation, to facilitate consistent access to the content and accurate citation.  

[Read more](./knowledge-hubs-and-websites.md).