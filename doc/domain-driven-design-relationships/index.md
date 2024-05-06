# Domain-driven design (DDD) - relationships to other ideas

**Object-oriented analysis and design**: In theory the general idea of DDD need not be restricted to object-oriented approaches, in practice DDD seeks to exploit the advantages that object-oriented techniques make possible. These include entities/aggregate roots as receivers of commands/method invocations and the encapsulation of state within foremost aggregate roots and on a higher architectural level, bounded contexts.

**Model-driven engineering (MDE) and Model-driven architecture (MDA)**: DDD is compatible with MDA/MDE. MDA is concerned more with the means of translating a model into code for different technology platforms than with the practice of defining better domain models. MDE is concerned wit techniques to model domains, to create DSLs to facilitate the communication between domain experts and developers. 

**POXOs**: These are technical implementation concepts, and reflect a growing view that, within the context of either of those technical platforms, domain objects should be defined purely to implement the business behaviour of the corresponding domain concept, rather than be defined by the requirements of a more specific technology framework.

**Naked objects pattern**: The premise that if you have a good enough domain model, the user interface can simply be a reflection of this domain model; and that if you require the user interface to be a direct reflection of the domain model then this will force the design of a better domain model.

**Domain-specific language (DSL) and Domain-specific modeling (DSM)**: DDD does not specifically require the use of a DSL, though it could be used to help define a DSL and support methods like domain-specific multimodeling. DSM is DDD applied through the use of Domain-specific languages.

**Aspect-oriented programming (AOP)**: AOP makes it easy to factor out technical concerns (such as security, transaction management, logging) from a domain model, and as such makes it easier to design and implement domain models that focus purely on the business logic.

**Command Query Responsibility Segregation (CQRS)**: CQRS is an architectural pattern for separation of reads from writes. While CQRS does not require DDD, domain-driven design makes the distinction between commands and queries, explicit, around the concept of an aggregate root. The idea is that a given aggregate root has a method that corresponds to a command and a command handler invokes the method on the aggregate root. The aggregate root is responsible for performing the logic of the operation and yielding either a number of events or a failure (exception or execution result enumeration/number) response OR (if Event Sourcing (ES) is not used) just mutating its state for a persister implementation such as an ORM to write to a data store, while the command handler is responsible for pulling in infrastructure concerns related to the saving of the aggregate root's state or events and creating the needed contexts (e.g. transactions).

**Event Sourcing (ES)**: ES is an architectural pattern which warrants that your entities do not track their internal state by reading and committing events to an event store, not by means of direct serialization or O/R mapping. When ES is combined with CQRS and DDD, aggregate roots are responsible for thoroughly validating and applying commands, and then publishing a single or a set of events which is also the foundation upon which the aggregate roots base their logic for dealing with method invocations. A significant benefit from this is that tooling such as axiomatic theorem provers (e.g. Microsoft Contracts or CHESS) are easier to apply. ES yields a domain model that synchronizes in distributed systems around the concept of optimistic concurrency.