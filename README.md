# Full Stack Development By Example

## Volume 1 - Student / Teacher Portal

This is the first volume in a set of hands on tutorials on how to build a web application.

This volume is designed to  takes a novice developer through the steps needed to develop a student / teacher portal for tracking classes, class schedules, courses and much more.
This will include an angular front end, a C# middle tier, and a SQL Server backend and deploy everything in docker containers managed in a kubernetes cluster. If you want to interface to other systems, there is a chapter and example code that will show how to do that. You should be able to follow this tutorial on Windows, Mac or Linux. All the code was written on a base level mac mini m1.

### The full series of Full Stack Development By Example Volumes are

| Volume   | Description | URL |
| -------- | ----------- | --- |
| 1 | Student Enrollments - an application to track student enrollments in classes | <https://github.com/sktxdev/FSDevVolume1> |
| 2 | Patient Scheduler - a patient appointment organizer for a doctors office | <https://github.com/sktxdev/FSDevVolume2> |
| 3 | A simple CRM for tracking sales leads | <https://github.com/sktxdev/FSDevVolume3> |
| 4 | A simple document management system | <https://github.com/sktxdev/FSDevVolume4> |
| 5 | Vet Portal - an application for vets to track pets they have treated | <https://github.com/sktxdev/FSDevVolume5> |
| 6 | Lost Pet Portal - a portal for tracking lost pets | <https://github.com/sktxdev/FSDevVolume6> |

### My Environment

- Hardware: A base level Mac Mini M1
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

### Other Stuff

- The section on the DB queries will also cover how to generate data dictionaries, perform query performance analysis and more

### Documentation

[Requirements](Requirements/Requirements.md)<br>
[Database](Documentation/Database%20Design/Databsse%20Design.md)<br>
[API](Documentation/API%20Design/API%20Design.md)<br>
[UI](Documentation/API%20Design/Controllers/Controllers.md)<br>
