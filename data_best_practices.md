# Data Best Practices

## Best Practices are Habits
Implement the below practices by setting policy and following through to form habits in your teams.  

In today's world we have screenshare calls/huddles, central code repositories, and free or open source tools to fulfill needs that used to require software packages that cost thousands of dollars per seat.

ONR Data is happy to provide your teams coaching on these practices.

## Define and Maintain Your Data Model

### Model Your Data

* The Third Normal Form (3NF) should be kept top-of-mind
* Denormalization is acceptable to meet reporting tools part way, but:
  * Understand and document the tradeoffs
  * Denormalize at the last possible step in the pipeline
* If your team pushes back, then find out why

### Implement Integrity Constraints

* Every table needs a Primary Key (PK)
* Add `not null` and `unique` constraints
* Define Foreign Key (FK) constraints
* Use Check constraints as needed
* It is always better to troubleshoot a failed data load than to go searching for data anomalies identified by your end users

### Generate Documentation from Your RDBMS Catalog

* Create your baseline data dictionary 
* Create generated Entity Relationship Diagrams (ERD) 
* Monitor completeness and currency with scripts

## Automate Your Data Flow

### Treat Data Movement as Pipelines

* Settle on an orchestration policy and stick to it
* Available methodologies span from products like Databricks down to scripts run under `cron`
* Expose your data operations to operations staff 
  * Ensure observability
  * Tie into ticketing systems
  * Create runbooks for problem resolution

### Accommodate Manual Steps

* Manual intervention is sometimes unavoidable
* Hands-on operations invite problems
  * Missed steps
  * File format changes
  * 

## Validate Wherever Possible

### Testing

### Budget for Interim Quality Reporting

### Bookend Every Manual Step

## Use Source Code Control

### Git

### Avoid Binary or Opaque Code Formats

## Control the Software Development Lifecycle

### Data Movement Policy

### Code Change Control