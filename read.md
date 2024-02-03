<!-----



Conversion time: 0.849 seconds.


Using this Markdown file:

1. Paste this output into your source file.
2. See the notes and action items below regarding this conversion run.
3. Check the rendered output (headings, lists, code blocks, tables) for proper
   formatting and use a linkchecker before you publish this page.

Conversion notes:

* Docs to Markdown version 1.0β35
* Fri Feb 02 2024 21:50:18 GMT-0800 (PST)
* Source doc: Requirements Specification - 1st Iteration
* Tables are currently converted to HTML tables.

WARNING:
You have 14 H1 headings. You may want to use the "H1 -> H2" option to demote all headings by one level.

----->


<p style="color: red; font-weight: bold">>>>>>  gd2md-html alert:  ERRORs: 0; WARNINGs: 1; ALERTS: 0.</p>
<ul style="color: red; font-weight: bold"><li>See top comment block for details on ERRORs and WARNINGs. <li>In the converted Markdown or HTML, search for inline alerts that start with >>>>>  gd2md-html alert:  for specific instances that need correction.</ul>

<p style="color: red; font-weight: bold">Links to alert messages:</p>
<p style="color: red; font-weight: bold">>>>>> PLEASE check and correct alert issues and delete this message and the inline alerts.<hr></p>



# Requirements Specification


## Business Analytics Upgrade (Project Octopus)

 


# **Document Overview**


## **Document Summary**

This document represents the top-level requirements and scope specification for the Business Analytics Upgrade project (hereafter, the Project), as negotiated between Flytographer and the development team. 

This document begins by specifying the necessary background and justification for the project, and goes on to state the project’s overall requirements. Following this, technical scope and further context is provided. Implementation details, success metrics, external interface requirements, and other necessary criteria conclude the document.

This is a living document, and represents the current state of the negotiated terms.


# **Version History**


<table>
  <tr>
   <td><strong>Name</strong>
   </td>
   <td><strong>Date</strong>
   </td>
   <td><strong>Comments</strong>
   </td>
   <td><strong>Version</strong>
   </td>
  </tr>
  <tr>
   <td><strong> </strong>
   </td>
   <td><strong> </strong>
   </td>
   <td><strong> </strong>
   </td>
   <td><strong> </strong>
   </td>
  </tr>
</table>



## Table of Contents


# Table of Contents

1. [Document Overview](#document-overview)  
2. [Document Summary](#document-summary)  
3. [Version History](#version-history)  
4. [Table of Contents](#table-of-contents)  
5. [Business Requirements](#business-requirements)  
    5.1. [Background](#background)  
    5.2. [Business Opportunity](#business-opportunity)  
    5.3. [Business Objectives](#business-objectives)  
        5.3.1. [Concrete Objectives](#concrete-objectives)  
        5.3.2. [Abstract Objectives](#abstract-objectives)  
    5.4. [Success Metrics](#success-metrics)  
6. [Vision Statement](#vision-statement)  
7. [Scope and Limitations](#scope-and-limitations)  
    7.1. [Principle Features](#principle-features)  
    7.2. [Scope](#scope)  
    7.3. [Initial Release](#initial-release)  
    7.4. [Second Release](#second-release)  
    7.5. [Subsequent Releases](#subsequent-releases)  
    7.6. [Limitations](#limitations)  
8. [Budget and Schedule](#budget-and-schedule)  
9. [Language, Architecture, and Other API](#language-architecture-and-other-api)  
10. [Accessibility](#accessibility)  
11. [Exclusions](#exclusions)  
12. [Context Description](#context-description)  
13. [User Classes and Characteristics](#user-classes-and-characteristics)  
14. [Operating Environment](#operating-environment)  
15. [Design and Implementation Constraints](#design-and-implementation-constraints)  
16. [Assumptions and Dependencies](#assumptions-and-dependencies)  
17. [Glossary of Terms](#glossary-of-terms)  
18. [References](#references)  
19. [System Features](#system-features)  
20. [Data Requirements](#data-requirements)  
21. [External Interface Requirements](#external-interface-requirements)  
22. [Software Quality Attributes](#software-quality-attributes)  
23. [Analysis Models](#analysis-models)  
24. [Appendix](#appendix)



# **Business Requirements**


## **Background**

Real Time Networks is a small, British Columbia based enterprise which manufactures and administrates physical asset lockers, marketed to other businesses. Real Time Networks (henceforth The Client) comprises numerous departments: Marketing, Manufacturing, Accounting, and others; and each such department manages its own data footprint independently. While one department might use QuickBooks to track sales, another may be using Excel to track inventory. This decentralization of the Client’s data footprint has made it difficult for their Executive Management team to make decisions, and oversee the running of the business.

The Project aims to implement a centralized, real time, functionally empowered data analytics tools so as to correct these limitations.

The software resulting from the Project shall hereafter be referred to as the System.


## **Business Opportunity**

The Client’s current infrastructure, or lack thereof, demands the careful assembly of reports from each department by key employees (henceforth, Administrators). Each report is phrased according to its progenating software’s syntax, resulting in confusingly mixed data formats. Report generation is also time consuming, error prone, and quickly becomes outdated.

Consequences of this lack of infrastructure are typically more subtle than can be easily measured – the quality of “decision making” manifests indirectly. However, certain concrete opportunities and other more abstract opportunities can be specified.


## **Business Objectives**


### **Concrete Objectives**



*  The number of systems needed to view the Client’s data footprint can be reduced to one
*  Report generation can be made faster and more flexible
*  The Client’s data footprint can be made viewable in real time
* Advanced analytics tools can be implemented which further enhance the system’s usefulness


### **Abstract Objectives**



* Decision making by the executive team can be made easier and more informed
* Errors due to inaccurate or outdated data can be minimized
* Sales can be increased and costs decreased
* Day to day operations can be made cheaper and more efficient
* Overall frustration can be eased


## **Success Metrics**

As previously stated, numeric metrics are difficult to apply when the goal is “improved decision making.” Perhaps more important than numeric metrics is simple Boolean success or failure: some component of infrastructure is measured as successful if it is implemented, otherwise it fails.

Based on this, the following concrete metrics are proposed:



* The number of systems required to view all data from all departments is reduced to one
    * All data currently accessible remains accessible
    * All such data is updated in real time
* All existing categories of audit or report can be generated from within the new system
    * Modification of report content, formatting, and other details can be customized
    * New report templates can be built easily
* A standard (if minimal) suite of data analytics tools is established
    * Charts and other visualizations can be easily generated
    * Other analytics tools, negotiated as needed, are implemented
* Different user classes are presented different views (contexts) according to their needs

These objectives represent the measurable success markers for the Project. Needless to say, other more generalized goals are the true motivation behind the Project. These include:



* Time between customer inquiry and product installation is reduced to 60 days
* Locker sales are increased
* Business operations are made cheaper and more efficient
* Research, marketing, and new product development is streamlined


## **Vision Statement**

**For** the Client’s Executive Management team, department directors, and assorted Administrators **who** are required to facilitate business operations, **the** Flytographer Business Analytics Upgrade **will** provide a centralized and empowered interface for better decision making through data analytics. Via this system: the Client’s entire data footprint will be accessible in real time; new and existing audits or reports will be accessible and easily customizable; assorted data analytics tools including charts may be generated; and a robust system of permissions and view customization will tailor the system on a user by user basis. **Unlike **the Client’s current lack of infrastructure**, the Project** will enable faster and better decision making, reduce cost and improve efficiency, increase sales, and streamline new product development.


# 


# **Scope and Limitations**


## **Principle Features**

The Project’s central features can be divided into three categories:



* A** Visual Interface **should provide real time access to the Client’s entire data footprint. This interface should also support various data visualization and analytics tools, including charts and infographics. Customizable views and assignment of permission should ensure that a user sees the data they need, when they need it, without unhelpful noise.This interface should be modern, visually appealing, and easy to use.
    * **Visualization Tools** such as tables, charts, simple infographics, and others should provide dynamic and real time access to data for Executive Managers, business analysts, and others. These visualizations should be printable for inclusion in audits and reports as needed.
    * **Prebuilt Views **should ensure that users with cross-departmental access (such as Executive Managers) can view data department by department, or context by context.
    * **View Customization **should ensure that a user sees only the data they need and have permission to access. Additionally, customization should allow for some degree of personalization for those who use the system regularly.
    * **Permission Management **should ensure data security and integrity. Maintenance of permission should be straightforward, likely delegated to the Client’s Administrators.
* **Real Time Data Maintenance** should ensure the Client’s entire data footprint is centralized and current. These systems should include the database itself, some means of saving snapshots of the current state of affairs, and the software to harvest data from various sources in real time.
    * **Data Harvesting** should run in the background on all workstations, harvesting and transmitting to the database any changes as they occur. Data harvesting software must be able to translate from the following systems:
        * QuickBooks
        * Hubspot
        * Excel
        * Access Database
        * Jira
        * TeamSupport
        * ServiceNow
    * A **Snapshot System **should ensure regular backups of Client’s data footprint are maintained, for data integrity and security purposes.
* **Report Generation **should initially enable all existing audits and reports to be accessible through the system, and should ultimately enable for easy creation of new report templates or modification of existing templates.

**Scope**


### **Initial Release**

The initial release should consist of the database’s creation, the completion of data harvesting software, and a first round of report generation protocols. This bare minimum of functionality should enable users of the System to access everything they can currently access but with improved efficiency.

Omitted from this release should be any data visualization software or views, the snapshot system, and report customization.


### **Second Release**

The second release should focus on establishing a general framework for the dashboard view and data visualization systems. Infrastructure for defining a view (or context) and embedding within it a layout should be developed. An initial round of data visualization tools should be implemented – primarily tables, as that is most likely the common data format. At this stage, permission setting should be implemented.


### **Subsequent Releases**

Subsequent releases should take an Agile or Scrum approach to the addition of more features. Audit- and report-template customization, more and more-advanced data visualizations, and view context customization should all proceed in balance according to ease of implementation and usefulness. The snapshot system should proceed as needed, though as a background priority.


## **Limitations**


### **Budget and Schedule**

The Project’s monetary budget is $100, 000, and its initial temporal budget is six months to initial release, with subsequent releases proceeding on an as-yet negotiated schedule.


### **Language, Architecture and Other API**

As a web application, the System’s front-end (user interface) will be built using HTML5 graphics and the JavaScript scripting language. As a backend, the Client has not specified a preferred language or architecture. These will be decided upon in future phases. The Client has specified the use of RestAPI where applicable.


### **Accessibility**

As a Canadian company, the Client feels it is appropriate to support both English and French interfaces. Other accessibility concerns such as supports for the visually impaired should be implemented on an industry-best-practice basis.


## **Exclusions**

No support for artificially intelligent analytics software has been requested by the Client.

 


# 


# **Context Description**


## **User Classes and Characteristics**

The Project anticipates the existence of three distinct user classes. These classes are…



* **C-Suite Executives **are the Client’s highest authority – the Executive Management team as it might be stated. This user class is responsible for the Client's company’s overall direction: which investments to make, which products to research, and other key decisions fall upon these users. This user class is also responsible for the running of the business’ day-to-day operations, albeit from a macro perspective. \
 \
 These users will consume the System in two ways. Firstly, these users will consume reports provided to them by Administrators in order to make decisions on behalf of the company. Here, the importance of_ accurate and_ _current _data is key. Secondly, these users will employ the System’s real time visualization tools to direct day-to-day operations, and to stay abreast of the state of the company. \
 \
 This class of user will likely have moderate technical skills, and a positive attitude towards the Project’s goals. These users will have total access to all views and all data. \

* **Managers and Directors **are either department heads or else chiefs of key operations. These users are essentially middle management and are in charge of day-to-operations from an \
 on-the-ground perspective. These users will make use of real-time visualization tools in order to stay abreast of the state of their operations. These users are unlikely to make use of formal audits and reports, though they may employ them from time to time. \
 \
These users should have access only to their own department’s data. Each department should be given its own context view and suite of visualizations to suit their needs. \

* **Administrators **are not technically a _position _so much as a _role _that any of the Client’s employees might take on. Administrators are those entrusted by the Client to maintain their data footprint. Their duties include the assembly of audits and reports for use by the executive team, manual data entry, and the maintenance of permission and context views. \
 \
These users will make use of all the system’s features, from audit and report generation to advanced data visualization, and from manual data entry to the maintenance of permissions and context views. \
 \


** **

**Operating Environment**

On a technical level, the system’s operating environment is a web browser on the frontend and a server running in the backend. The Client expects consistent behavior across all major browsers, as well as support for mobile devices. As such, responsive design will be required. On the backend, a server will facilitate communication between users on the frontend and the system’s core software.

Physically speaking, users will likely make use of the system in an office setting, though across a wide range of departments with (potentially) differing conditions.


## **Design and Implementation Constraints**

The system must support automatic data harvesting from the following sources:



* QuickBooks
* Hubspot
* Excel
* Access Database
* Jira
* TeamSupport
* ServiceNow

Data harvested from these sources must be placed in a central database, and then vended to users of the System with consistent syntax and formatting. The System should harvest data from all sources in real time, transmitting changes as they occur to the central database.

The Client has specified the use of RestAPI where appropriate. The primary backend language should support modular, future-friendly, object-oriented design.


## **Assumptions and Dependencies**

The development team makes the following assumptions:



* All software from which the system harvests will remain updated at all times
* All browsers will remain updated
* Export formats from source software will be standard


## **Glossary of Terms**

**The Client **refers to Flytographer as a whole, the entity commissioning the Project.

**The Team** refers to the development team which is designing and implementing the Project.

**The Project **refers to the endeavor by the Team to implement the System, and encompasses all documents, procedures, assumptions, and code therein.

**The System **refers to the end result of the development process, the actual software being developed, and the software which users will actually use.

**Executive Management **refers to those employed by The Client to make business altering decisions, as well as to oversee the running of the company.

**Administrator **refers to those employed by The Client to maintain their data footprint and its integrity as well as the System itself.


## **References**

No references have been identified.

 

 


# 


# **System Features**

 


# **Data Requirements**


# **External Interface Requirements**


# **Software Quality Attributes**


# **Analysis Models**


# **Appendix**

 
