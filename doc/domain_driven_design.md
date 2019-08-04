# Domain-driven design (DDD)

Domain-driven design (DDD) is an approach to software development for complex needs by connecting the implementation to an evolving model.

Premise:

  * Place the project's primary focus on the core domain and domain logic.

  * Base complex designs on a model of the domain.

  * Collaborate among technical and domain experts to iteratively refine a conceptual model that addresses particular domain problems.

Concepts:

  * Context: the setting in which a word or statement appears that determines its meaning.

  * Domain: a sphere of knowledge (ontology), influence, or activity; a subject area.

  * Model: A system of abstractions that describes selected aspects of a domain and can be used to solve problems related to that domain;

  * Ubiquitous Language: a language structured around the domain model and used by all team members to connect all the activities of the team with the software.


## Strategic domain-driven design

Bounded context: explicitly set boundaries in terms of team organization, usage within specific parts of the application, and physical manifestations such as code bases and data schemas.

Continuous integration: institute a process of merging all code and other implementation artifacts frequently, with automated tests to flag fragmentation quickly.

Context map: explicity identify and name each model, bounded context, non-object-oriented subsystems; make names part of the ubiquitous language, and describe the points of contact, communication, and sharing.


## Cost and complexity

To help maintain the model as a pure and helpful language construct, the implementation team must typically create a great deal of isolation and encapsulation within the domain model. Consequently, a system based on domain-driven design can come at a relatively high cost. 

While domain-driven design provides many technical benefits, such as maintainability, some companies recommend that DDD be applied only to complex domains, where the model and the linguistic processes provide clear benefits in the communication of complex information, and in the formulation of a common understanding of the domain.

