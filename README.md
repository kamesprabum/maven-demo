# Week 11 Jenkins webhook test

A simple Java project created to understand the basics of **Apache Maven** and its integration with **Jenkins**.

## Project Overview

This project demonstrates how Maven can be used to:

- Compile Java code
- Run unit tests
- Package the application into a JAR file
- Manage project dependencies
- Prepare a project for Jenkins CI/CD

# Maven Demo

A simple Java project created to understand the basics of **Apache Maven** and its integration with **Jenkins**.

## Project Overview

This project demonstrates how Maven can be used to:

- Compile Java code
- Run unit tests
- Package the application into a JAR file
- Manage project dependencies
- Prepare a project for Jenkins CI/CD

## Tech Stack

- Java 17
- Apache Maven
- JUnit 5
- Git & GitHub
- Jenkins

## Project Structure

```text
maven-demo/
├── pom.xml
├── .gitignore
├── README.md
└── src/
    ├── main/
    │   └── java/
    │       └── com/
    │           └── demo/
    │               └── App.java
    └── test/
        └── java/
            └── com/
                └── demo/
                    └── AppTest.java
```

## Maven Commands

Build the project:

```bash
mvn clean package
```

Run tests:

```bash
mvn test
```

Compile the project:

```bash
mvn compile
```

Package the application:

```bash
mvn package
```

## Run the Application

After building the project:

```bash
java -cp target/classes com.demo.App
```

Expected output:

```text
Maven Demo
10 + 20 = 30
```

## Maven Build Flow

```text
mvn clean package
       │
       ▼
     Clean
       │
       ▼
    Compile
       │
       ▼
      Test
       │
       ▼
    Package
       │
       ▼
      JAR
```

## Jenkins Integration

The project is designed to be used as a simple Jenkins CI exercise.

Jenkins can pull this repository from GitHub and execute:

```bash
mvn clean package
```

Maven reads the project's `pom.xml`, builds the application, runs the tests, and creates the JAR file.

## Learning Goal

The goal of this project is to understand the basic relationship between:

**GitHub → Jenkins → Maven → Java Build**

This is a small hands-on project for learning Maven before moving into larger DevOps pipelines.
