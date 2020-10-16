---
title: "How it works"
date: 2020-09-08T11:00:00-04:00
hide_sidebar: true
seo_title: "How it works"
keywords: ["openmdm", "how does it work"]
---

## User components
The user components of openMDM® support the user in carrying out different steps in the measurement process and allow the standardization and automation of repetitive workflows. Alongside the storage of the measurement data, the recording of descriptive data (metadata) is a central aspect in each process step. Metadata are important for the usability of any data management system since they are used for navigation, exploration, searches and for the ability to compare the measurement data.

The diagram illustrates the openMDM® standard process.

{{< figure src="/overview/images/how-does-it-work.jpg" alt="openMDM standard process" >}}

&nbsp;

Measurement systems and analysis tools from different vendors can be integrated into the workflow in a flexible way via open interfaces. Some process steps generate business objects which are intended for the user to see. These can include test orders, test results, reports, evaluations or references to data objects located in the ODS storage.

## Administration components
The administration components of openMDM® allow that applications can be easily tailored and adapted to specific use cases. The following topics can be administrated by selected users:

Data structures in which all descriptive information of a test (metadata) can be unambiguously stored. These include information describing the context of a test (e.g. unit under test, test equipment and test set up) as well as information describing the measurement result (e.g. measured quantities, units and channels).
Templates for the description of test procedures.
Specific application components to support the user in the test description and commissioning or automatic processing of data objects (e.g. automatic generation of test and test step names, transferring data from external systems, execution of actions when entering data and commissioning tests or mapping of attributes for assignment of measured data).
User roles, groups and permissions to ensure the confidentiality of test data.
Those tasks do not require ASAM ODS or database expert knowledge.