---
title: "Architecture"
date: 2020-09-08T11:00:00-04:00
hide_sidebar: true
seo_title: "Architecture"
keywords: ["openmdm", "architecture"]
---

openMDM® applications consist of a collection of components that can be distributed on different computers within a network. The communication between these components is done via defined interfaces.

Each component can be assigned exactly to one logical layer of the openMDM® architecture. The diagram provides an overview.

**ODS Services**  
This layer contains the basic features and specifications of the ODS standard. The functions are provided by a ODS server via OO API.

**Application Model**  
The application model is an openMDM®-specific implementation of the abstract ODS base model. It specifies the business objects that can be stored persistently in openMDM®. Although a large part of the generic constructs of ODS base model were dissolved, the storage structures for descriptive information (metadata) are designed to be very general and flexible. This layer can be extended with modular additions. In order to make the expansion of the application model accessible, an extension of the openMDM® API is required.

**Business Objects and Rules**  
In order to highlight the particular importance of the openMDM® API, it is assigned to a separate layer. Any access to ODS is done via the openMDM® API. It defines the business objects (e.g. MeaResult) and other business rules of openMDM®. It is described in IDL and be used by overlying building blocks. If the application model is expanded, it must be a building block in this layer, which implements the access to the extension of the model.

**Extended Business Services**  
This layer contains components which expand the openMDM® API by specific business objects (e.g. openMDM Entry) and functions (e.g. openMDM Syslog). They use the openMDM® API and are remote accessible for other blocks via their IDL interface. The layer can be extended to provide additional business objects, functions and rules.

**Platform interfaces**  
This layer contains the interfaces for platform-specific runtime environments. For the current reference implementations this are those of the Java VM (e.g. I/O API) and OSGi Containers (e.g. OSGi EventAdmin).

**Non-UI interfaces**  
Platform-specific interfaces that are not part of the user interface belong to this layer

**UI interfaces**  
Interfaces that belong to the user interface and serve the presentation of information (e.g. the composition of different views) are part of this layer.