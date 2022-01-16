# Full Stack Development By Example

## Introduction and Setup

This is a series of tutorials to help new or entry level developers get up to speed quickly on Web Application Development.

Each volume will show how to setup an angular front end, a C# middle tier, and a SQL Server backend and deploy everything in docker containers managed in a kubernetes cluster. If you want to interface to other systems, one of the tutorials that will show how to do that. You should be able to follow this tutorial on Windows, Mac or Linux. All the code was written on a base level mac mini m1.

### The full series of Full Stack Development By Example Volumes are

| Volume   | Description | URL |
| -------- | ----------- | --- |
| 1 | A simple document management system | <https://github.com/sktxdev/FSDevDMS> |
| 2 | Property Manager - a portal for property maangement | <https://github.com/sktxdev/FSDevPropman> |
| 3 | A simple CRM for tracking sales leads | <https://github.com/sktxdev/FSDevCRM> |
| 4 | Student Enrollments - an application to track student enrollments in classes | <https://github.com/sktxdev/FSDevStudentPortal> |
| 5 | Patient Scheduler - a patient appointment organizer for a doctors office | <https://github.com/sktxdev/FSDeVPatientScheduler> |

| 6 | Lost Pet Portal - a portal for tracking lost pets | <https://github.com/sktxdev/FSDevLostPets> |
| 7 | Vet Portal - an application for vets to track pets they have treated | <https://github.com/sktxdev/FSDevVetPortal> |

### My Environment

- Hardware: A base level Mac Mini M1, I'm also testing this on a Surface Pro 6 i5
- Front End: Angular 13, Material UI, Typescript, scss, html etc
- Middle tier(api/services): Dotnet Core 3.1 (3.1.22), C#, DB Code uses dapper or linq◊
- Databse: SQL Server running in a Docker Container

### Rationale

I'm using Microsoft technologies because thats what I used on a day to day basic. I may convert this to use other databases, but the UI and API are generic enough that they can be pointed at a different database with little trouble.

### Code Structure

Within each example repository, the code is segmented into folders: UI, API, DB, Doc and Exercises

- DB contains all database code including db creation scripts, store procs, sql snippets etc (SQL)
- API contains the API (dotnet core/C#)
- UI contains the UI (Angular)
- Doc contains all the documentation
- Exercises contains the exercises

### Database Fundamentals

From an application developers perspective, a database is a convenient way to store relational data. A database is more than that, but for the purposes of these tutorials, that is how we will approach things.

Within a database there is a collection of tables that may or may not be related to each other. Each table is a collection of records.

Records may be related to other records, for example if we have a collection of Products, each of which has detail information and also category information, then Product is related to Product Category, and Product Detail is related to Product.

In order to formulate a relationship between 2 or more tables, we use what is called a foreign key reference.

Visually this can be seen as:

        ProductCategory  <---- Product <---- ProductDetail

- ProductDetail will have 2 keys, ProductDetailId (the primary key) and ProductId (this is a reference to the associated record in the Product table, i.e., a Foreign Key).
- Product will have 2 keys also, ProductId (the primary key) and ProductCategoryId (a reference to a record in the ProductCategory table)
- ProductCategory has one key, ProductCategoryId (this primary key)

A given record in any table represents an single entity. Every entity may have properties. For example, Product has a name, a description, and some properties, it also has a category, but we dont want to spell out that category on every row in the product table, therefore we move this to another table, ProductCategory and simply provide a reference to that record from the product table. This is called normalization.

If you want to know more, head over to my [SqlTutorial](https://github.com/sktxdev/SQLTutorial)
