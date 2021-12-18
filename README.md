# Full Stack Development By Example Code

This is a set of sample applications covering various scenarios that can be extended or borrowed from for your own application. The code is entirely free and located at https://github.com/sktxdev/

The code is a part of the book series "Full Stack Development by Example". Each book covers one of the applications below, it takes the developer from beginning to end in the steps to build a functioning web application, this includes an angular front end, C# middle tier, and SQL Server backend. If you need to interface to other systems, there is a chapter on doing that with each application.

### Books
Full Stack Development By Example - Volume 1 - The basics
Full Stack Development By Example - Volume 2 - Student Enrollments - an application to track student enrollments in classes
Full Stack Development By Example - Volume 3 - Patient Scheduler - a patient appointment organizer for a doctors office
Full Stack Development By Example - Volume 4 - A simple CRM for tracking sales leads
Full Stack Development By Example - Volume 5 - A simple document management system
Full Stack Development By Example - Volume 6 - Vet Portal - an application for vets to track pets they have treated
Full Stack Development By Example - Volume 7 - Lost Pet Portal - a portal for tracking lost pets


### Applications
- Patient Management System (Humans)	https://github.com/sktxdev/FullStackDevByExampleBookCode/pmsapp
- Vet Portal				https://github.com/sktxdev/FullStackDevByExampleBookCode/vetapp
- Lost Pet Finder			https://github.com/sktxdev/FullStackDevByExampleBookCode/petapp
- Student Enrollment Portal		https://github.com/sktxdev/FullStackDevByExampleBookCode/studentapp
- Generic CRM				https://github.com/sktxdev/FullStackDevByExampleBookCode/crmapp
- Simple DMS				https://github.com/sktxdev/FullStackDevByExampleBookCode/dmsapp

### Technologies
- Front End: Angular 13, Typescript, scss, html etc
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
