---
layout: archive
title: "Experience"
permalink: /experience/
author_profile: true
---
## Software Engineering Intern @ Autodesk
<p style="text-align:left;">
    <b>Atlanta, GA</b>
    <span style="float:right;">
        <i>may 2022 - Aug 2022</i>
    </span>
</p>

- Created ETL scripts to pull data from three key learning platforms into AWS Neptune, leveraging openCypher for querying – resulting in a highly connected knowledge graph consisting of over 30000 nodes and around 50000 relationships
- Developed a graph-based recommendation system utilizing AWS Neptune which increased monthly active users by 40% (estd)
- Implemented a GraphQL API for the recommendation engine consisting of Lambda functions (built using the Node.js Serverless framework) exposed over AWS AppSync to enable dynamic querying of the knowledge graph
- Provisioned and configured different AWS instances (EC2, Neptune, AppSync, Lambdas) and IAM roles using Cloudformation


## Head Teaching Assistant @ Georgia Tech
<p style="text-align:left;">
    <b>Atlanta, GA</b>
    <span style="float:right;">
        <i>Jan 2022 - Present</i>
    </span>
</p>

- Teaching assistant for the _CSE 6242 - Data and Visual Analytics_ course consisting of over 1200 students 
- Responsible for updating and creating autograder scripts, grading assignments, holding office hours and ensuring smooth collaboration between TAs

## Software Engineering Specialist @ General Electric
<p style="text-align:left;">
    <b>Hyderabad, India</b>
    <span style="float:right;">
        <i>Aug 2020 - Aug 2021</i>
    </span>
</p>

- Optimized GE’s Kubernetes based solution for creating microservices over AWS – used by over 150 teams globally
- Designed and developed REST-based microservices using Java and Spring Boot to add functionality to the platform (e.g., 
testing, storing preferences, data layer, etc.) – dockerized and deployed them as Kubernetes pods on the cluster as well as wrote Jenkins jobs for some of them
- Created & updated PDIs & Helm charts for automating the pod deployments; migrated build artifacts to JFrog Artifactory
- Visualized pod and system-level statistics for over 15 internal and default components using Grafana and Prometheus
- Configured Alertmanager to send out alerts to relevant stakeholders when user-defined thresholds were crossed
- Conducted performance tests on messaging queues (Artemis and Kafka) using Apache Camel to ensure that SLAs were being met

**Tech stack:** Java, Spring Boot, Kubernetes, Docker, PostgreSQL, Prometheus, Grafana, Alertmanager, Jenkins