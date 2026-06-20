Staff Ratings Application (Assignment 2)


Live Demo: https://staffratings-276.onrender.com


Features

Create staff ratings with validation

View all submitted ratings

Persistent PostgreSQL database storage

Server-side validation with error handling

Repository persistence (save, retrieve, delete)

Automated tests (validation + persistence)

Dockerized deployment

Cloud deployment on Render


Tech Stack

Java 17

Spring Boot 3

Spring MVC

Spring Data JPA

PostgreSQL

Thymeleaf

JUnit 5

Docker

Render



How to Run Locally

Prerequisites

Java 17+

PostgreSQL

Maven 

Steps to make it:

1. Create database
CREATE DATABASE staffratings;

2. Configure DB credentials

Set these environment variables before running (this keeps application.properties clean so the test suite can still use the in-memory H2 database):

SPRING_DATASOURCE_URL=jdbc:postgresql://localhost:5432/staffratings
SPRING_DATASOURCE_USERNAME=...
SPRING_DATASOURCE_PASSWORD=...

3. To run the app
./mvnw spring-boot:run

4. To open in browser
http://localhost:8080

Deployment (Render)

This app uses Docker + Render PostgreSQL.

Create Render PostgreSQL

4. Deploy

Render → Manual Deploy → Deploy latest commit

5. Open deployed app
https://staffratings-276.onrender.com


AI Declaration

used chat gpt on parts of the assignment to help with syntax.



