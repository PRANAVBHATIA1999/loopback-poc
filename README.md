# Generated REST API using LoopBack 4

## Part 1 – Automatic API Generator Used

**Tool Used:** **LoopBack 4 CLI** (`@loopback/cli`)

For this assignment, I used LoopBack 4, an automatic API generator that scaffolds a complete REST API project with minimal manual coding. LoopBack automatically generates the project structure, models, datasources, repositories, and controllers.


---

## Steps Followed to Auto-Generate the API

### 1. Install LoopBack CLI
```bash
npm install -g @loopback/cli

Create the LoopBack app:

lb4 app


Project name: books-api

Description: Trying LoopBack for Quiz 14

Left all other options as default.

Generate the Book model:

lb4 model


Model name: Book

Base: Entity

Properties:

id (number, id, required)

title (string, required)

author (string, required)

year (number, optional)

Create an in-memory datasource:

lb4 datasource


Datasource name: memdb

Connector: In-memory db

Generate repository:

lb4 repository


Datasource: MemdbDatasource

Model: Book

Repository: BookRepository

Generate CRUD REST controller:

lb4 controller


Type: REST CRUD controller

Model: Book

Repository: BookRepository

Base path: /books

This automatically created CRUD endpoints such as:

POST /books

GET /books

GET /books/{id}

PATCH /books/{id}

PUT /books/{id}

DELETE /books/{id}

How to Run
npm install
npm start


Then open:

API: http://127.0.0.1:3000

API Explorer: http://127.0.0.1:3000/explorer