---
title: "Related Eclipse Projects"
date: 2020-09-08T11:00:00-04:00
hide_sidebar: true
seo_title: "Related Eclipse Projects"
keywords: ["openmdm", "Related Eclipse Projects"]
---

The following Eclipse projects are related to the openMDM Working Group:

## 1. [MDM|BL](https://projects.eclipse.org/projects/technology.mdmbl)
The MDM|BL project comprises a bottom to top architecture view of three parts:

The first one is a specific openMDM application model definition for the ASAM ODS data storage. The standardization provides a structured representation for common use case related data in all openMDM application. The data model is split into the base model, which covers the most common use cases, and extensions for additional use cases.

The base model and every extension has an associated API interface. These interfaces are used by higher level components to work with openMDM business objects. In addition there are a set of business interfaces, which represent non data based enterprise use cases.

At the top of the layer there are the implementations of the business interfaces. In consideration of the API  there normally will be an  ODS server implementation but in some use cases the data storage is implemented otherwise. Virtual objects or the storage in an ODS ATFX file are examples.

Concerning the runtime view the business layer project defines a core application structure, which every openMDM application is based on. This structure is composed of services and rules how these services should be used and be executed at runtime.

Status: Incubation  
Link: https://projects.eclipse.org/projects/technology.mdmbl

## 2. [MDM|WEB](https://projects.eclipse.org/projects/technology.mdmweb)
PLEASE NOTE THAT THIS PROJECT HAS BEEN ARCHIVED. IMPORTANT CONTENT HAS BEEN TRANSFERRED TO MDMBL

The MDM@WEB project includes multiple components for handling measured data. These components are structured to allow for high re-usability of core components like the communication with the ODS server or the import and export of data. In addition to these core components the project includes a web-based front-end.

The list of components includes:

* Navigator.
* Search (Meta-Data).
* Search (Full-Text).
* Export.
* Reporting.
* Shopping Cart (for interaction with local tools).
* Localization.
* User Documentation.
* Administration.
* Data Sharing.
* Archiving.  

Status: Incubation  
Link: https://projects.eclipse.org/projects/technology.mdmweb