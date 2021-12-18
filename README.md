# Full Stack Development By Example Code

This is a set of sample applications covering various scenarios that can be extended or borrowed from for your own application. The code is entirely free and located at github/sktxdev/


### Applications
- Patient Management System (Humans)	https://github.com/sktxdev/FullStackDevByExampleBookCode/pmsapp
- Vet Portal				https://github.com/sktxdev/FullStackDevByExampleBookCode/vetapp
- Lost Pet Finder			https://github.com/sktxdev/FullStackDevByExampleBookCode/petapp
- Student Enrollment Portal		https://github.com/sktxdev/FullStackDevByExampleBookCode/studentapp
- Generic CRM				https://github.com/sktxdev/FullStackDevByExampleBookCode/crmapp
- Simple DMS				https://github.com/sktxdev/FullStackDevByExampleBookCode/dmsapp

### Technologies
- Front End: Angular 9, Typescript, scss, html etc
- Middle tier(api): Dotnet Core 3.1 (3.1.22), C#, DB Code is dapper or linq
- Databse: SQL Server (some use of stored procedures)

### Rationale:
I'm using Microsoft technologies because thats what I used on a day to day basic. I may convert this to use other databases, but the UI and API are generic enough that they can be pointed at a different database with little trouble.

### Code Structure
Within each repository, the code is segmented into 3 folders: UI, API and DB
- DB contains all database code including db creation scripts, store procs, sql snippets etc (SQL)
- API contains the API (dotnet core/C#)
- UI contains the UI (Angular)

### Other Stuff
- The section on the DB queries will also cover how to generate data dictionaries, perform query performance analysis and more
