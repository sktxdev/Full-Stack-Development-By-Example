# Full Stack Development By Example

## Introduction and Setup

This is a series of tutorials to help new or entry level developers get up to speed quickly on Web Application Development.

Each volume will show how to setup an angular front end, a C# middle tier, and a SQL Server backend and deploy everything in docker containers managed in a kubernetes cluster. If you want to interface to other systems, one of the tutorials that will show how to do that. You should be able to follow this tutorial on Windows, Mac or Linux. All the code was written on a base level mac mini m1.

### The full series of Full Stack Development By Example Volumes are

| Volume   | Description | URL |
| -------- | ----------- | --- |
| 1 | Student Enrollments - an application to track student enrollments in classes | <https://github.com/sktxdev/FSDevStudentPortal> |
| 2 | Patient Scheduler - a patient appointment organizer for a doctors office | <https://github.com/sktxdev/FSDeVPatientScheduler> |
| 3 | A simple CRM for tracking sales leads | <https://github.com/sktxdev/FSDevCRM> |
| 4 | A simple document management system | <https://github.com/sktxdev/FSDevDMS> |
| 5 | Vet Portal - an application for vets to track pets they have treated | <https://github.com/sktxdev/FSDevVetPortal> |
| 6 | Lost Pet Portal - a portal for tracking lost pets | <https://github.com/sktxdev/FSDevLostPets> |
| 7 | Property Manager - a portal for property maangement | <https://github.com/sktxdev/FSDevPropman> |

### My Environment

- Hardware: A base level Mac Mini M1, I'm also testing this on a Surface Pro 6 i5
- Front End: Angular 13, Material UI, Typescript, scss, html etc
- Middle tier(api/services): Dotnet Core 3.1 (3.1.22), C#, DB Code uses dapper or linq
- Databse: SQL Server running in a Docker Container

### Rationale

I'm using Microsoft technologies because thats what I used on a day to day basic. I may convert this to use other databases, but the UI and API are generic enough that they can be pointed at a different database with little trouble.

### Code Structure

Within each repository, the code is segmented into 3 folders: UI, API and DB

- DB contains all database code including db creation scripts, store procs, sql snippets etc (SQL)
- API contains the API (dotnet core/C#)
- UI contains the UI (Angular)
- Doc contains all the documentation
- Exercises contains the exercises
