# Domain-specific language (DSL)

A domain-specific language (DSL) is a computer language specialized to a particular application domain. This is in contrast to a general-purpose language (GPL), which is broadly applicable across domains. 

There are a wide variety of DSLs, ranging from widely used languages for common domains, such as HTML for web pages, down to languages used by only one piece of software. 

DSLs can be subdivided by the kind of language, and include domain-specific markup languages, domain-specific modeling languages (more generally, specification languages), and domain-specific programming languages. Special-purpose computer languages have always existed in the computer age, but the term "domain-specific language" has become popular due to the rise of domain-specific modeling. 


## Use

The design and use of appropriate DSLs is a key part of domain engineering, by using a language suitable to the domain at hand – this may consist of using an existing DSL or GPL, or developing a new DSL. Language-oriented programming considers the creation of special-purpose languages for expressing problems as standard part of the problem-solving process. 

Creating a DSL (with software to support it), rather than reusing an existing language, can be worthwhile if the language allows a particular type of problem or solution to be expressed more clearly than an existing language would allow and the type of problem in question reappears sufficiently often. Pragmatically, a DSL may be specialized to a particular problem domain, a particular problem representation technique, a particular solution technique, or other aspects of a domain.


## Example: Gherkin for behavior driven design

Gherkin is a language designed to define test cases to check the behavior of software, without specifying how that behavior is implemented. It is meant to be read and used by non-technical users using a natural language syntax and a line-oriented design. The tests defined with Gherkin cant then be implemented in a general programming language.


## Example: Rules engines for policy automation

Various business rules engines have been developed for automating policy and business rules used in both government and private industry. ILOG, Oracle Policy Automation, DTRules, Drools and others provide support for DSLs aimed to support various problem domains. DTRules goes so far as to define an interface for the use of multiple DSLs within a Rule Set.

The purpose of business rules engines is to define a representation of business logic in as human-readable fashion as possible. This enables both subject matter experts and developers to work with and understand the same representation of the business logic. Most rules engines provide both an approach to simplifying the control structures for business logic (for example, using Declarative Rules or Decision Tables) coupled with alternatives to programming syntax in favor of DSLs.
