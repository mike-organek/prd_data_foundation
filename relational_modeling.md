<base target="_blank" />

# Relational Modeling

## A Brief and Simplified History

## Origins of SQL and Relational Databases

The relational data model was first described in 1969 and [published by ACM in 1970 &#x1f855;](https://web.archive.org/web/20070612235326/http://www.acm.org/classics/nov95/toc.html).  

When I learned about relational algebra and calculus in an undergraduate course titled "Files and Databases" in the 1980s, we wrote our SQL with pen and paper because there was no affordable implementation available to us for classroom use.

Throughout the 1990s, vendors like Oracle, Sybase, IBM, and Microsoft released and popularized expensive implementations of SQL Relational Database Management Systems.  Toward the end of the decade, open-source projects like MySQL and PostgreSQL further democratized the use of SQL.

## Data Warehousing

The then-legacy vendors began moving their systems built on ISAM/VSAM, the various dBase-like 4GL platforms, and the Berkeley DB family of databases to use SQL storage engines as they came to market.  This opened their systems to reporting from offerings like Crystal Reports and offloaded the database and files management to the RDBMS vendors and an army of database administrators.

Data Warehousing took hold to meet the demand for reporting and analytics.  Though major ERP and business tool vendors moved their data into SQL RDBMS systems, it was years before the set-based paradigm of SQL took hold.  Many such systems&mdash;even today&mdash;contain tens of thousands of lines of code that treated RDBMS SQL tables as though they were indexed data files sitting in catalogs on refrigerator-sized DASD.

Data warehouse and SQL developers, driven by reporting and analytics needs, were the prime advancers of the arts of SQL and Relational Modeling.  As these SQL developers and data architects on the reporting side refined the virtues of Star Schemas, Snowflake Schemas, Data Vault while rejecting too many failed concepts to list (EAV, anyone?), best practices emerged to deal with concerns like performance, retention and archiving, evolution of master data over time, ETL/ELT, and data security and governance.

The vendors in the Data Warehousing space demanded and received astronomical licensing fees for their tools and technology.  Consultants demanded and received astronomical rates for working in and around these expensive systems.  This made perfect sense when the cost of compute, storage, and network bandwidth constrained the market.

## Big Data

As the world got comfortable with social media and e-commerce, the advertising companies funding the orgy of excess stretched their ambitions toward achieving omniscience.  

Companies started tracking every time an email was opened or a shopper clicked a link on their websites.  They did what they could to match these activities to known customers and their purchase history.  They starte paying handsomely to enrich their customer databases with demographic information about individuals, households, and the neighborhoods they lived in.  Social media giants selling advertising sweetened the pot by providing data on impressions, click-throughs, and whatever could be gleaned by intrusive cookie tracking.

Thousands of companies each sprouted dozens of eyes to be like Argus Panoptes.  It was a towering achievement.  All this knowledge let them know where, when, and to whom to send coupons and flyers.

All of this data needed crunching, but the volumes overwhelmed the SQL RDBMS offerings available at the time.  Specialized hardware like Netezza made it possible, but the licensing, implementation, and hardware costs were prohibitive for all but organizations with the deepest pockets.

About the same time that 

