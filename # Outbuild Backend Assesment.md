# Outbuild Backend Assesment

  

## Overview

  

To join our team at Outbuild, you should be capable of developing scalable and secure APIs. During development, we primarily use **Express and PostgreSQL** (though our projects sometimes extend beyond this stack).

A key part of your role will involve efficiently managing **large datasets**.

The objective of this test is to assess your understanding of **essential backend principles**, including but not limited to software design principles, test-driven development, error handling, logging, security, and architectural design.

  

## Problem statement

  
 At Outbuild,  construction **schedules** are the core entity for our **users**. For this test, assume that each user can access multiple schedules, with each schedule associated with a single user. A schedule can contain many **activities**—some may have thousands—and each activity is associated with a single schedule. 

Each schedule has a name and an URL of an image with the construction objective (e.g., a building). Each activity has a name, a start date, and an end date.

Your task is to develop a backend system that effectively implements these domain entities. You have the autonomy to decide on the storage system, API details, pagination, and other architectural choices. If you progress to the next stage of the hiring process, you may be asked to **explain your decisions**.

The following section outlines the base requirements for the system implementation.
  

## Requirements

  

###  API Requirements:

The API must include **at least** the following endpoints:

1.  Create an empty schedule (with no activities) in the system.
2.  Retrieve a schedule along with its activities.
3.  Add an activity to a schedule.
4.  Add multiple activities to a schedule.

 > ��**Note** :  Your API should be documented, and you are free to choose the format and any tools you deem appropriate for this.



###  Security and Performance Requirements:
Your implementation should include a mechanism to prevent users from accessing schedules that do not belong to them. Use techniques that enhance security and speed, such as avoiding the exposure of database entities during data transfers and optimizing the number of requests.

###  Error handling:
Your implementation should include a mechanism to effectively catch and handle most errors. 

###  Observability:
Your implementation should include a mechanism to log the system transactions.
  
###  Tests:
Your implementation should include any necessary tests that you deem appropriate.


  

## Deliverables:

 An expected deliverable is a repository containing the source code of your project, along with instructions on how to run tests and start the project. 

  >  �� **Important**: Ensure that we can run your implementation on our machines. Please provide any necessary configurations to run your project (e.g., Dockerfile, etc.). Additionally, describe **any relevant decisions  regarding the problem or code structure** in the README file.


## Technology Stack

-   Express
    
-   Node.js
    
-   PostgreSQL (you may use neon.tech or a similar DBaaS)
    
-   Any additional tools or libraries you deem necessary for the system


## Evaluation Criteria:

This section contains a list of basic questions that will be part of our evaluation criteria. These may help guide you during the development process:

-   **✅ Correctness:** Does the API behave as expected?
    
-   **��Testing:** Are there sufficient and effective tests for each feature?
    
-   **⚡Performance:** Is the API performant, especially when handling large datasets?
    
-   **��️ Security:** Are there measures in place to secure the API?
    
-   **�� Scalability:** Is the API structured to accommodate future growth and increased data load?
    
-   **�� Code Quality:** Is the codebase well-architected, clean, modular, and maintainable, following best practices and software principles?
