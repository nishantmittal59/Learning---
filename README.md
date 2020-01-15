# Learning :-)
This is made to learn &amp; explore new tech &amp; research.

## :point_right: Software Architecture
The presented architectures are designed based on three factors: 
#### > distributed or non-distributed
#### > front-end (server-side or client-side)
#### > monolithic or microservices

### Deployment Monolithics, Microservices, and DevOps
cloud computing can’t do much if systems are still designed in deployment monolithic approach where software applications are deployed as a single unit. Even though the monolithic approach is easy to understand by developers and has been adopted for decades, it has become a bottleneck with the new technology trends.
In the monolithic approach, software systems are developed most likely in the same technology stack, cluster-based replication as a scalability strategy.
Microservices architecture is based on developing software projects into modular services that are: small, self-contained, self-deployable, designed around business capabilities, manage its own data, and communicate with other services over a lightweight protocol (most likely HTTP).

In microservices, every service is designed, developed and operated by a dedicated team, which has almost a full decision on the design and technology of their service. This approach of team structure and management is called ***DevOps.***

:arrow_right: **Non-Distributed Monolithic With Server-Side Front-End**

In this architecture the application is developed using a 3-layer architecture which runs in a single process. In this approach, the front-end can be developed using Java EE( JSP or JSF), Spring MVC (FreeMarker, Thymeleaf, or JSP), and dynamic HTML rendering using server-side scripting languages such as PHP or Python.

Advantage is development simplicity and convenience. scalability, maintainability, and security are the main concerns. In addition, support for modern front-end technologies (such as smartphones apps) may be challenging as well.

:arrow_right: **Non-Distributed Monolithic With Client-Side Front-End**

This design is similar to the previous one, except that the frontend and the backend are separated into two subsystems. In this approach, the front-end will be fully running on the client side while the backend will run as a server-side process.

Potential technologies to be used in the front-end, in this case, could be
* Traditional web frontend technologies, including HTML, Bootstrap, CSS, and JavaScript.
* Javascript based client-side frameworks such as Angular or React.
* Native client applications such as Android, iOS, or desktop apps.
* Hybrid applications, such as Cordova, PhoneGap, or Xamarin.

This approach enables technology separation between the front-end and backend, where a new front-end can be supported easily without any modifications to the backend.

:arrow_right: **Distributed Monolithic With Client-Side Front-End**

The application is divided into 4-tiers (separate processes), where each tier communicates with the tier next to it over the network.
In this architecture, even though extra complexity is added to development, deployment, and operations, it enables more levels of modularity and reusability of every tier, where any tier can be easily replaced with another one. In addition, it is considered more secure than the one-tier architecture presented in the previous two approaches. Moreover, it allows more efficient scalability, especially if asynchronous communication is implemented (maybe by using event-driven reactive techniques or traditional messaging such as Java messaging service).

:arrow_right: **Non-Cloud Native Microservices**

This design utilizes the microservices architectural style. In particular, the application is modulized into self-contained services that can be deployed independently. In microservices architecture, every service shall be designed around business capabilities and manage its own database.

Microservices enables evolutionary approach of software development, where services and features can be developed and deployed incrementally without affecting other services. In addition, it enables more efficient scalability with its lightweight horizontal scalability on the microservice level (not the application level).

Potential technology for microservices implementation includes:
* Spring Boot.
* Drop Wizard.
* Java Micro profile.
* NodeJS.
* Python.

Theoretically, any technology talks HTTP can be used to develop microservices.

:arrow_right: **Cloud-Native Microservices**

In this approach, a microservices-based application will exploit the full benefits of cloud computing based on the 12-Factors concepts. 
This design might be sufficient for small-medium scale cloud-based applications. However, for more complex and larger scale applications, more infrastructure microservices should be considered, such as the components provided out of the box by Spring Cloud project.

In addition, other opensource projects may be useful to explore, such as Spring Boot Admin for real-time web-based application monitoring and JHipster project which provides a nice generator for cloud-based applications.

***JHipster*** is a fully Open Source, widely used application generator. Easily create high-quality Spring Boot + Angular/React projects!

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
