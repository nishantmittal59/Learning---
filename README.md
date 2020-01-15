# Learning :-)
This is made to learn &amp; explore new tech &amp; research.

## ->> Software Architecture
The presented architectures are designed based on three factors: 
#### > distributed or non-distributed
#### > front-end (server-side or client-side)
#### > monolithic or microservices

### Deployment Monolithics, Microservices, and DevOps
cloud computing can’t do much if systems are still designed in deployment monolithic approach where software applications are deployed as a single unit. Even though the monolithic approach is easy to understand by developers and has been adopted for decades, it has become a bottleneck with the new technology trends.
In the monolithic approach, software systems are developed most likely in the same technology stack, cluster-based replication as a scalability strategy.
Microservices architecture is based on developing software projects into modular services that are: small, self-contained, self-deployable, designed around business capabilities, manage its own data, and communicate with other services over a lightweight protocol (most likely HTTP).

In microservices, every service is designed, developed and operated by a dedicated team, which has almost a full decision on the design and technology of their service. This approach of team structure and management is called ***DevOps.***

### Why Software Architecture ?
The purpose of software development processes is to deliver primary functionality expected by the end users and external stakeholders ,this category of functionality is known as ***functional requirements***

Most of the time, functional requirements can be achieved without following best practices or having a good architecture. For example, implementing a full-featured wire-transfer functionality (including security, validation, integration, and auditing), can be implemented in a single file (maybe tens of hundreds of lines of code).

However, in the last example, the application will not survive for a long time. Problems will start to be visible in many stages, starting with the internal testing, user acceptance testing, to the going-live. Main concerns will be reliability (achieving the required functionality as expected all the time) and maintainability (the ability to maintain and apply changes to this functionality). Also, other potential issues include scalability and security. This leads to a different type of requirements: non-functional requirement (i.e. quality attributes).

### Service Oriented Architecture (SOA) vs Microservices
SOA services communicate over heavyweight smart-pipes (ESB), microservices communicate over dump pipes with smart-end points.
SOA aims to integrate enterprise large complex monolithic applications into enterprise-wide processes, while microservices aims to integrate small microservices into a single project.
SOA is enterprise-wide based, microservices is project based.
In SOA, a business process is created as orchestration and managed by the platform, in microservices, a business process is written as another microservice on the application level, which can be replaced by another service if the process changed.

An ***enterprise service bus(ESB)*** is a middleware tool used to distribute work among connected components of an application. ESBs are designed to provide a uniform means of moving work, offering applications the ability to connect to the bus and subscribe to messages based on simple structural and business policy rules.

***Orchestration*** is the automated configuration, coordination, and management of computer systems and software.
