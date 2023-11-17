<base target="_blank" />

# Relational Modeling

## A Brief and Simplified History

## Origins

The relational data model was first described in 1969 and [published by ACM in 1970 &#x1f855;](https://web.archive.org/web/20070612235326/http://www.acm.org/classics/nov95/toc.html).  

When I learned about relational algebra and calculus in an undergraduate course titled "Files and Databases" in the 1980s, we wrote our SQL with pen and paper because there was no affordable implementation available to us for classroom use.

Throughout the 1990s, vendors like Oracle, Sybase, IBM, and Microsoft released and popularized expensive implementations of SQL Relational Database Management Systems.  Toward the end of the decade, open-source projects like MySQL and PostgreSQL further democratized the use of SQL.

## Data Warehousing

The then-legacy vendors began moving their systems built on ISAM/VSAM, the various dBase-like 4GL platforms, and the Berkeley DB family of databases to use SQL storage engines as they came to market.  This opened their systems to reporting from offerings like Crystal Reports and offloaded the database and files management to the RDBMS vendors and the army of database administrators.

Data Warehousing took hold to meet the demand for reporting and analytics.  Though major ERP and business tool vendors moved their data into SQL RDBMS systems, it was years before the set-based paradigm of SQL took hold.  Many such systems&mdash;even today&mdash;contain tens of thousands of lines of code that treated RDBMS SQL tables as though they were indexed data files sitting in catalogs on refrigerator-sized DASD.

Data warehouse and SQL developers, driven by reporting and analytics needs, were the prime advancers of the arts of SQL and Relational Modeling.  As these SQL developers and data architects on the reporting side worked with Star Schemas, Snowflake Schemas, Data Vault, and too many failed competing concepts to list (EAV, anyone?), best practices emerged to deal with common scenarios like retention and archiving, evolution of master data over time, ETL/ELT, and data security and governance.

The vendors in the Data Warehousing space demanded and received astronomical licensing fees for their tools and technology.  Consultants demanded and received astronomical rates for working in and around these expensive systems.  This made perfect sense when the cost of compute, storage, and network bandwidth constrained the market.  That market grew as the cost of resources came down.

## Big Data and NoSQL

