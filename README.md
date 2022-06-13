# How to publish open data: a list of advice and tools

<p align="center"><img src="./open_data_illustration.png" alt="i typed open data in to one of those AI image generation things and got this" width="500"/></p>

This is a curated list of links which we, at the  [Open Data Institute](https://theodi.org/), think are most helpful in publishing open data. It includes useful links and advice about platforms, licences, metadata and standards.

If you would like to expand or adapt this list yourself, please feel free to fork the project. If you would like to recommend some resources for this guide, please create a  [GitHub Issue](https://docs.github.com/en/issues), and we’ll consider them. 

## Contents
*  [About open data](#about-open-data) – the key concepts behind open data
*  [Data publishing platforms](#data-publishing-platforms) – some tools which can help put data on the web
*  [Dataset metadata](#dataset-metadata)  – standards and advice for data that describes datasets
*  [Tabular Data and CSVs](#tabular-data-and-csvs) – tools and advice 
*  [Application programming interfaces (APIs)](#application-programming-interfaces-apis) – best practices for machine-readable APIs
*  [Naming data files and datasets](#naming-data-files-and-datasets)  – how to name datasets for easy finding and use 
*  [Accessibility](#accessibility) – how to be inclusive of all people’s needs when publishing data
*  [Data licences](#data-licences) – what licences are for and how to pick the right one
*  [Data standards](#data-standards) – why standards are important and how to develop one

## About open data
Before getting to the tools and techniques of publishing, it’s important to know the core definitions and principles of open data.

**[The Open Definition](https://opendefinition.org/)  | Open Knowledge Foundation**

* ‘Open means anyone can freely access, use, modify, and share for any purpose (subject, at most, to requirements that preserve provenance and openness)’*

* The definition is available in many languages
* The Open Knowledge Foundation is a non-profit, international organisation and behind a number of the resources linked to here

**[What is Open Data?](https://opendatahandbook.org/guide/en/what-is-open-data/)  |  Open Data Handbook**
* This takes the open definition and expands on it, explaining what open means for data and why it’s so valuable.
* The handbook was also made by the Open Knowledge Foundation

**[Some open data publishing principles](https://digitalblog.ons.gov.uk/2017/01/06/some-open-data-publishing-principles/)  | ONS Digital**
* Principles can be very useful to refer to when making decisions – and to ask: ‘if I do this, will it adhere to our principles?’ 
* These seven principles are an excellent, concise review of what to aim for when publishing open data

**[The Annotated 8 Principles of Open Government Data](https://opengovdata.org/)  | Opendata.gov**
* These principles were formed by a committee open government specialists
* They contain some important points which weren’t mentioned in the previous link

**[The Data Spectrum](https://theodi.org/about-the-odi/the-data-spectrum/)  | Open Data Institute**

* Data exists on a spectrum from closed to shared to open
* Data should be as open as responsibly possible, while protecting people’s privacy, commercial confidentiality and national security.


## Data publishing platforms
**[Data Portals](https://tech.datopian.com/data-portals/#summary-data-portals-make-data-discoverable-and-accessible-and-provide-a-foundation-for-integration)   | Datopian Tech**
* Comprehensive overview on data portals. What are they, why they would be needed 
* This can help you decide what your data publishing needs actually are before choosing any tool
* Note: the portals it reviews are very centred on the CKAN platform


**[CKAN](https://ckan.org/)  | Comprehensive Knowledge Archive Network**
* *‘CKAN is an open-source DMS (data management system) for powering data hubs and data portals. CKAN makes it easy to publish, share and use data.’*
* The biggest and most widely used data platform by large public organisations. 
* Features include APIs, visualisations, search and analytics 
* Over [250 user-generated extensions](https://extensions.ckan.org/) available 

 **[Datasette](https://datasette.io/)** 
* ‘*Datasette is a tool for exploring and publishing data. It helps people take data of any shape or size, analyze and explore it, and publish it as an interactive website and accompanying API*
* Straightforward to set up and provides a simple interface * Can run SQL queries on the datastore
* Search and API functionality
* Not as many features as platforms like CKAN

**[DataDock](https://datadock.io/info/about)  | Networked Planet**
* ‘*DataDock is an online service which creates navigable data portals for individuals and organisations to publish open data free of charge’*
* Helps with adding dataset metadata, licences, and search

**[OpenDataSoft](https://www.opendatasoft.com/)** 
* Large, many-featured, software service share and visualise open datasets
* Holds a large share of the open data publishing market across public and private organisations
* Runs a [Data Hub](https://data.opendatasoft.com/pages/home/) which gives access to nearly 27,000 open datasets. 

**[Open Data Platform (powered by Socrata)](https://www.tylertech.com/products/data-insights/open-data-platform) | Tyler Technologies** 
* Socrata is a software service for data insights that was acquired Tyler Technologies in 2018
* Popular product in the open data publishing space
* Connected to the [Open Data Network](http://www.opendatanetwork.com/) to browse and access open dataset, with a [discovery API](https://socratadiscovery.docs.apiary.io/#).


## Dataset metadata
Dataset metadata is data that describes and provides information about data. Adding good metadata to a dataset helps the users understand what a dataset contains and how it is structured. Also, search engines use metadata to index datasets, making them easier to find. 

**[Data and Datasets](https://schema.org/docs/data-and-datasets.html) | schema.org**
* Schema.org is a community that agrees on data standards to add to structured data when publishing to the web
* It’s used by several big search engines to find and index datasets on the web
* Schema.org also provides overviews of the [Dataset](https://schema.org/Dataset) and [DataCatalog](https://schema.org/DataCatalog) types (*DataCatalog*s can contain multiple *Dataset*s) 

**[Dataset | Documentation](https://developers.google.com/search/docs/advanced/structured-data/dataset)  | Google Developers**
* Guidance on how to add structured data (like that from Schema.org) to a dataset
* Essential properties required for Google Dataset Search – such as *description* and *name* – are listed in the [properties](https://developers.google.com/search/docs/advanced/structured-data/dataset#dataset) section.
* Other recommended properties are useful for metadata, such as *creator*, *licence* and *url*. 

**[Marking up your dataset with DCAT](https://theodi.org/article/marking-up-your-dataset-with-dcat/)  | Open Data Institute**
* *‘The Data Catalog Vocabulary (DCAT) defines a standard way to publish machine-readable metadata about a dataset’*
* Simple guide from 2014 by the ODI on adding DCAT metadata 

**[Data Catalog Vocabulary (DCAT) format](https://www.w3.org/TR/vocab-dcat/)  | W3C**
* The full documentation on DCAT* DCAT v2 now has support for documenting APIs 

**[Sample Dataset Metadata](https://centerforgov.gitbooks.io/open-data-metadata-guide/content/appendix-a.html)  | Centre for Gov (USA)**
* Part of a guide on dataset metadata as used by the USA federal government
* Useful as it provides a list of properties and then clearly explains what each of those metadata properties represent

**[Metadata best practice for data publishers](https://www.gov.uk/government/publications/making-your-geospatial-data-easy-to-fin%5B%E2%80%A6%5Da-easy-to-find-metadata-best-practice-guide-for-data-publishers)  | Geospatial Commission**
* An introduction to metadata and practical guidance for data publishers  
* Outlines the importance of good metadata in ensuring published data can be discovered and used effectively
* Provides guidance and examples in describing the key characteristics of data

**[Search Engine Optimisation best practice for data publishers](https://www.gov.uk/government/publications/search-engine-optimisation-for-publishers-best-practice-guide)  | Geospatial Commission**
* Guidance to maximise the discoverability of your data in search engines and portals  


## Tabular data and CSVs
**[Creators of tools for open data? Steal this](https://theodi.org/article/creators-of-tools-for-open-data-steal-this/)  | Open Data Institute**
* Blogpost from the ODI summarising user research on data publishing tools, along with accompanying report
* The research highlights key needs of people publishing data:
	* *tools that are easier to use*
	* *better tools for checking and ensuring quality of the published data*
	* *better integration between tools in the publishing workflow*
* Includes a link to a [register of open source tools](https://docs.google.com/spreadsheets/d/11yyev1MyDZqR7iS0FgLqwgCe_D3XkS--97x0b6cNeF0/edit#gid=2015018097) 

**[Using CSV file format](https://www.gov.uk/guidance/using-csv-file-format)  | UK Government Digital Service**
* Aimed at people working in the UK government, but contains lots of good points
* ‘[Setting up your CSV file](https://www.gov.uk/guidance/using-csv-file-format#setting-up-your-csv-file)’ describes the basics of well-formatted CSVs
* Includes useful advice on when and when not to use CSV files. 

**[Tidy data](https://cran.r-project.org/web/packages/tidyr/vignettes/tidy-data.html)  | Hadley Wickham**
* Advice, adapted from a paper, on how to structure clean, easy-to-analyse, tabular datasets
* ‘*Tidy datasets are easy to manipulate, model and visualize, and have a specific structure: each variable is a column, each observation is a row, and each type of observational unit is a table’*

**[Frictionless Framework](https://framework.frictionlessdata.io/docs/guides/introduction/)  | Frictionless Data**
* Frictionless Framework is a *‘data management framework for Python to describe, extract, validate, and transform tabular data’ *
* Part of  [Frictionless Data](https://frictionlessdata.io/) , an open source toolkit of software and standards for the use of data. Part-funded by the Open Knowledge Foundation.* Available as command-line tool, Python library and in Javascript

**[CSV Lint](https://csvlint.io/)  | Open Data Institute**
* Online tool to validate CSV files
* *CSVLint helps you to check that your CSV file is readable. And you can use it to check whether it contains the columns and types of values that it should*

**[An Introduction to VisiData](https://jsvine.github.io/intro-to-visidata/)**
* Impressive open source command line tool for interacting with tabular data
* ‘A*free, open-source tool that lets you quickly open, explore, summarize, and analyze datasets in your computer’s terminal*’


## Naming data files and datasets
Good names for datasets make the contents clear and save time for data users. 

**[Datasets](https://style.ons.gov.uk/category/data-visualisation/datasets/)  | Office of National Statistics UK**
* *‘How to structure and format your datasets and write effective dataset titles, summaries and information notes’*
* Simple and to-the-point advice
* Developed by the ONS for internal use, but acts as a useful template for other data stewards to guide naming practices and standards. 

**[Best Practices for File Naming – Records Express](https://records-express.blogs.archives.gov/2017/08/22/best-practices-for-file-naming/)  | USA National Archives**
* Short blogpost on things to consider when naming files

**[File naming and structure](https://libguides.princeton.edu/c.php?g=102546&p=930626)  | Princeton University Library**
* A useful guide around the importance of descriptive file names for organising, sharing, and monitoring data files. 
* The most important piece of advice: ‘*Write down naming convention in data management plan*’. Data stewards and data users should be able to easily understand the naming conventions.


## Application programming interfaces (APIs)
**[What is an Application Programming Interface (API)](https://www.ibm.com/cloud/learn/api)  | IBM**
* Good introduction article to the topic of APIs, explaining some of the fundamental concepts: what are APIs; why we need them; types of APIs etc.
* A useful resource to help make the business case for APIs

**[Open standards and open APIs](https://theodi.org/topic/open-standards-and-open-apis/)  | Open Data Institute**
* A collection of projects from different sectors which use and apply APIs   

**[Web API design best practices](https://docs.microsoft.com/en-us/azure/architecture/best-practices/api-design)  | Microsoft Azure**
* Comprehensive and detailed high-quality, technical introduction to good API development
* We recommend the first section on ‘RESTful web API design

 **[API technical and data standards](https://www.gov.uk/guidance/gds-api-technical-and-data-standards) | UK Government Digital Service**
* ‘*The following web-based application programming interface (API) standards guidance will help your organisation deliver the best possible services to users.’*
* This is a comprehensive guide with useful sections, from publishing bulk data through to testing performance and scalability 


## Accessibility
**[Accessibility](https://www.w3.org/standards/webdesign/accessibility)  | W3C**
* A good, short overview on why accessibility for websites and data is so important
* ‘*The power of the Web is in its universality. Access by everyone regardless of disability is an essential aspect.’ – Tim Berners-Lee*
* The dataset you publish is very likely to be on a web page. This page should be accessible to people with a diverse range of hearing, movement, sight, and cognitive ability. 

**[Releasing Statistics in Spreadsheets](https://gss.civilservice.gov.uk/policy-store/releasing-statistics-in-spreadsheets/#section-3) | UK Government Statistical Service**
* *Guide ‘to help improve the usability, accessibility and machine readability of statistical spreadsheets.’*
* Good examples of accessible spreadsheets
* Advice on naming spreadsheet tables, columns, cells so that they are accessible and machine-readable

**[The 6 Simplest Web Accessibility Tests Anyone Can Do](https://karlgroves.com/2013/09/05/the-6-simplest-web-accessibility-tests-anyone-can-do)  | Karl Groves**
* Before going in to automated testing tools, check the basics of the page’s accessibility
* Tests include simply turning off the mouse, images and/or CSS

**[Creating Accessible Tables - Data Tables](https://webaim.org/techniques/tables/data) | Web Accessibility In Mind**
* Discusses which HTML tags to add to make data tables more accessible 
* WebAIM is a long running organisation that provides training and services in web accessibility, and has a good library of  [useful articles](https://webaim.org/articles/) .

**[WAVE](https://wave.webaim.org/)** 
* Free web accessibility tool from WebAIM
* ‘*WAVE can identify many accessibility and Web Content Accessibility Guideline (WCAG) errors, but also facilitates human evaluation of web content.*’
* Enter a website address to get a diagnosis of accessibility issues 


## Data licences
Licences define what others can and can not do with the data you publish. 

**[Publisher’s Guide to Open Data Licensing ](https://theodi.org/article/publishers-guide-to-open-data-licensing/) | Open Data Institute**
* Introduction to licensing for open data
* This can help you understand what data you are allowed to store, and what you are allowed to openly publish
* *‘If you have ownership of a work, and someone else wants to use it, they have to ask your permission. Licences are how you explicitly give someone else permission to use that work.’*

**[How to choose an open data license](https://koordinates.com/guides/how-choose-open-data-license/)  |  Koordinates**
* Includes a clear description of creative commons licences and the difference between the four licence elements of *Attribution*, *ShareAlike*, *No-Derivatives* and *Non-Commercial*

**[Choose a License](https://creativecommons.org/choose/)  | Creative Commons**
* Useful step-through to help you choose which CC licence is best for you 
* Includes the option of an icon to use on your website along the data

**[Conformant Licenses](https://opendefinition.org/licenses/)  | Open Definition from the Open Knowledge Foundation**
* List of all the licences that conform to the Open Knowledge Foundation’s definition of an open licence. 
* Also includes an API to pull structured information about each of these licences
* This can useful if you encounter a licence elsewhere and are unsure whether its suitable or not 

**[Using geospatial data: a guide to licences](https://theodi.org/projects-services/projects/using-geospatial-data-a-guide-to-licences/)  | Open Data Institute**
* The ODI published this guide to help people understand different types of licences 
* It has 17 example use cases of geospatial data, and discusses what licence is most suitable and why


## Data standards
**[Data standards: What are they and why do they matter?](https://transparencee.org/analysis/data-standards-what-are-they-and-why-do-they-matter/)  | Transparencee**
* Nice approachable description on data standards. Articles on this topic can often be quite dry, and this article is refreshingly clear. 
* *‘The power of the standard comes from the power of all the stakeholders using it. If it’s not really common then it isn’t really a standard.’*

**[What are open standards for data?](https://standards.theodi.org/introduction/what-are-open-standards-for-data/)   | ODI, Open Standards Guidebook**
* *‘Standards are documented, reusable agreements that solve a specific set of problems or meet clearly defined needs. Standards detail the language, concepts, rules, guidance or results that have been agreed.’*
* Part of a guidebook the ODI released on open data standards. It explains many aspects of data standards including how to find them, choose and create them.  

**[Data standards](https://resources.data.gov/standards/concepts/)   | Data.gov**
* Overview of the definitions and terms used around data standards
* *‘An anatomical unit of a data standard is referred to as a data standard “component.” The documentation for a more holistic data standard specification then assembles multiple components together to form a data standards “package.’*
* Especially useful is the breakdown of different types of components in a data standard package – identifiers, vocabulary, formats, APIs etc

**[Data Standards](https://www.ons.gov.uk/aboutus/transparencyandgovernance/datastrategy/datastandards) | UK Office of National Statistics** 
* Useful as a reference list of some example data standards
* They range from simple standards on naming conventions, such as how dates should be represented through to metadata schemas such as Dublin Core or Schema.org 

**[OpenStand Principles](https://open-stand.org/)   | OpenStand**
* Five clear criteria (cooperation; adherence to principles; collective empowerment; availability; voluntary adoption) for the development of open standards
* Developed jointly by a range of authoritative international bodies, including the Institute of Electrical and Electronics Engineers (IEEE) and the World Wide Web Consortium (W3C)
* While there are many definitions of what constitutes an ‘open standard’, the OpenStand criteria are influential and widely accepted
