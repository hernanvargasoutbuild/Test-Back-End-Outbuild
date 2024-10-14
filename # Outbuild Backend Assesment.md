# Outbuild Backend Assesment

## Objective

In order to work in Outbuild, you need to develop scalable and secure APIs by using (but not limited to) Express and PostgreSQL, and handling large datasets in a efficient way. It's required to demostrate a good understanding of key backend principles, like application of software principles, TDD, error handling, logging and security and architecture design.

## Problem

Outbuild uses schedules as the principal entity for our users, an user has multiple schedules and one schedule is related to only one user, a schedule has multiple activities (some schedules has thousands of them) and one activity is related to only one schedule. We need you to develop a backend system that implements this domain entities and let us work with them in a efficient way. A schedule has a unique name and a image url representing the building, in the other hand, an activity has a name, a start date and an end date. Is up to you decide wheter the storage system, the API details, pagination, etc... if you pass to the next step in the hiring process, you could be asked why you take those decisions. In the next section, we'll give you the base requirements, in order to evaluate what decisions you take while the developing of this assesment.

## Requirements

* **API Requirements**:
  The API needs to comply with at least, this endpoints:

  1. Creates an empty schedule (with no activities) in the system 
  2. Returns a schedule with their activities 
  3. Adds an activity to a schedule
  4. Adds multiple activities to a schedule

* **API Documentation**
  Document the implemented endpoints

* **Security**
  Implement a security measure that prevent non-authorized users access to schedules that don't belong to them. Also, don't expose database entities, make usage of DTOs

* **Error Handling**
  Implement some method to handle most of the errors that can be on the system

* **Observability**
  Implement logs for each transaction in the system

* **Testing**
  Implement tests for the 4 usecases

## Deliverables:

A repository containing the source code of your project, instructions on how to run tests and run the project, Dockerfile and docker-compose if necessary, and everything that we need in order to run your project. Also, each decision that you think is relevant, or asumptions regarding the problem, must be described in the README.md file.

## Technology Stack
* Express
* NodeJS
* PostgreSQL (you can use neon.tech or related DBaaS, local implementations of the database requires a Dockerfile for us in order to run the project)
* Anything that you consider necessary for the system

## Evaluation Criteria:
* Correctness: Does the API behave as expected ?
* Testing: Are there sufficient and effective tests for each feature?
* Performance: Is the API performant, especially when handling large datasets?
* Security: Are there measures in place to secure the API?
* Scalability: Is the API structured in a way that can handle future growth and data load?
* Code Quality: Is the codebase well-architected, clean, modular, and maintainable following best practices and software principles?
