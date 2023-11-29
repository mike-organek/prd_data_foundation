# Data Best Practices

## Best Practices are Habits
Adopt these practices by setting policy and then following through to make them habits in your teams.  

In today's world we have screenshare calls/huddles, central code repositories, and free or open source tools to fulfill needs that used to be inadequately filled by software packages that cost thousands of dollars per seat.  It has never been easier to create a constant feedback loop with minimal impact on productivity.

[ONRData &#x1f4e7;](mailto:morganek@onrdata.com) is happy to provide coaching for your teams on these practices as we work to resolve your data problems.

## Define and Maintain Your Data Model

### Model Your Data

* Keep the Third Normal Form (3NF) at top of mind
* Denormalization is acceptable to meet reporting tools part way, but:
  * Understand and document the tradeoffs
  * Denormalize at the last possible step in the pipeline
* If your team pushes back, then find out why

### Implement Integrity Constraints

* Every table needs a Primary Key (PK)
* Add `not null` and `unique` constraints
* Define Foreign Key (FK) constraints
* Use Check constraints as needed
* It is always easier to troubleshoot a failed data load than to diagnose data anomalies identified by end users

### Generate Documentation from Your RDBMS Catalog

* Get the baseline data dictionary from the database catalog
* FK constraints simplify Entity Relationship Diagram (ERD) production
* Monitor completeness and currency with scripts

## Automate Your Data Flow

### Treat Data Movement as Pipelines

* Settle on an orchestration methodology and stick to it
* Available methodologies span from products like Databricks down to scripts run under `cron`
* Expose your data operations to operations staff 
  * Ensure observability
  * Tie into ticketing systems
  * Create runbooks for problem resolution

### Accommodate Manual Steps

* Manual intervention is sometimes unavoidable
* Hands-on operations invite problems
  * Missed steps
  * Duplicate loads
  * File format changes
* Wrap manual steps with validation before and after (see below)

## Validate, Validate, Validate

### Automate Validation

* Adopt software testing tools and methods to help
* Clearly define pipeline error handling, including notifications to outside teams
* Treat process logs as data and put dashboards on them
* Bookend automated validation around problematic (*e.g.* manual) steps

### Quality is the Product

* Budget for interactive validation&mdash;including incremental visualizations that look nothing like the final product&mdash;during development
* Earliest project milestones and deliverables must require customer sign-off
* Remember the parable of the blind men and the elephant
  * Involve customers and SMEs in requirements sessions
  * There is no better icebreaker for requirements clarification than a visualization that end users can pick apart

## Apply Software Development Principles

### Source Code Control

* Manage source code and configuration artifacts with `git`
* If your existing development does not fit in `git`, then you are doing it wrong
* Reap the benefits:
  * Change history as a side effect
  * Code review as habit, leading to rapid improvements in quality and professional development
  * Foundation for adopting DevOps and DevSecOps tools and methodologies

### Data Movement Policy

* Implement a convention for naming objects
* Define guidelines for transformations and data quality at each stage
* Enforce data integrity early
* Automate compliance checks

### Software Development Lifecycle

* Separate development from QA and production environments
* Take advantage of new cloud paradigms to create non-production environments on demand
* Treat support operations as product
  * Automate cloning
  * Adopt a test-first approach to maintenance
* Build Change Control fences around non-development environments

## Have We Struck a Chord?

Please contact [ONRData &#x1f4e7;](mailto:morganek@onrdata.com) to schedule a call to discuss what ONRData can do for your organization to get onto the right track of doing data the right way.