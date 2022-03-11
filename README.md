# SidelineSwap Java Coding Exercise (sls-mettle)

## Description

In this coding exercise you will create a simple Spring Boot application that hosts a REST web service and persists data in a database.

## Required Tasks

1. Create a spring boot application named sls-mettle.
2. Create a REST webservice that manages items. (Create, Read, Update, Delete)
    ```
    {
      "id": "26937741-15a2-435b-82b0-39cd0539ed5e",  :uuid
      "name": "Item Name",                           :string (0-20)
      "description": "Item description",             :string (0-200)
      "type": "hockey_pads"                          :enum["hockey_pads","hockey_skates","hockey_stick"]
      "cost": 20.00,                                 :double (>0.00)
      "created_at": "2022-03-10T14:46:55.372283Z",   :timestamp (iso8601)
      "updated_at": "2022-03-10T14:46:55.372283Z",   :timestamp (iso8601)
      "deleted_at": null                             :timestamp (iso8601)
    }
    ```
3. Instantiate the database schema for storing this information using FlywayDB. Use PostgreSQL or MySQL for the database.
4. Add appropriate logging statements and error handling.
5. Feel free to show off any architectural patterns you prefer.

## Submitting
1. Please commit your resulting code to a repository on your personal GitHub account. 
2. Share the link to the repository to your contact on the SidelineSwap team.

## Requirements

- Java 14+
- Use Gradle for dependency management
- Use Log4J2 for logging instead of SLF4J
- Use Spring Data JPA for data layer
- Use PostgreSQL or MySQL for persistence
- Flyway for schema creation
- Use of spring initializer is fine.

## Optional Tasks for Fun

1. Create a request filter that logs the IP address of each incoming request.
2. Create a search endpoint that returns a list of matching items.
3. Broadcast messages when items are modified to a RabbitMQ topic.
