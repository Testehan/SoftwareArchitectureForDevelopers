## Part 1 - What is software architecture?
*  As a noun = architecture can be summarised as being about structure. It’s about the
   decomposition of a product into a collection of components/modules and interactions. This needs
   to take into account the whole of the product, including the foundations and infrastructure
   services that deal with cross-cutting concerns such as power/water/air conditioning (for a
   building) or security/configuration/error handling (for a piece of software)
* As a verb = architecture (i.e. the process, architecting) is about understanding what you need to
  build, creating a vision for building it and making the appropriate design decisions. All of this
  needs to be based upon requirements because requirements drive architecture. Crucially, it’s
  also about communicating that vision and introducing technical leadership so that everybody
  involved with the construction of the product understands the vision and is able to contribute in
  a positive way to its success.
* Application architecture is what we as software developers are probably most familiar with,
  especially if you think of an “application” as typically being written in a single technology
  (e.g. a Java web application, a desktop application on Windows, etc). It puts the application
  in focus and normally includes things such as decomposing the application into its constituent
  classes and components, making sure design patterns are used in the right way, building or
  using frameworks, etc. In essence, application architecture is inherently about the lower-level
  aspects of software design and is usually only concerned with a single technology stack (e.g.
  Java, Microsoft .NET, etc).
  The building blocks are predominantly software based and include things like programming
  languages and constructs, libraries, frameworks, APIs, etc. It’s described in terms of classes,
  components, modules, functions, design patterns, etc. Application architecture is predominantly
  about software and the organisation of the code.
* System architecture
  I like to think of system architecture as one step up in scale from application architecture. If
  you look at most software systems, they’re actually composed of multiple applications across a
  number of different tiers and technologies. As an example, you might have a software system
  comprised of a .NET Silverlight client accessing web services on a Java EE middle-tier, which
  itself consumes data from an Oracle database. Each of these will have their own application
  architecture.
* Software architecture
  Unlike application and system architecture, which are relatively well understood, the term
  “software architecture” has many different meanings to many different people. Rather than
  getting tied up in the complexities and nuances of the many definitions of software architecture,
  I like to keep the definition as simple as possible.
  For me, software architecture is simply the combination of application and system architecture
* there’s a growing trend of software
  systems being made up of tiny micro-services⁵, where each service only does one thing but does
  that thing very well. A micro-service may typically be less than one hundred lines of code. If
  change is needed, services can be rewritten from scratch, potentially in a different programming
  language. This style of architecture provides agility in a number of ways. Small, loosely coupled
  components/services can be built, modified and tested in isolation, or even ripped out and
  replaced depending on how requirements change. This style of architecture also lends itself well
  to a very flexible and adaptable deployment model, since new components/services can be added
  and scaled if needed.
* Architecture vs design
  Grady Booch has a well cited definition of the difference between architecture and design that
  really helps to answer this question. In On Design¹, he says that
  As a noun, design is the named (although sometimes unnameable) structure or
  behavior of an system whose presence resolves or contributes to the resolution of
  a force or forces on that system. A design thus represents one point in a potential
  decision space.
* Part of the process of architecting a software system is about understanding what is significant and why.
* The benefits of software architecture
  What benefits can thinking about software architecture provide then? In summary:
* * A clear vision and roadmap for the team to follow, regardless of whether that vision is
  owned by a single person or collectively by the whole team.
* *  Technical leadership and better coordination.
* *  A stimulus to talk to people in order to answer questions relating to significant decisions,
  non-functional requirements, constraints and other cross-cutting concerns.
* * A framework for identifying and mitigating risk.
* * Consistency of approach and standards, leading to a well structured codebase.
* *  A set of firm foundations for the product being built.
* * A structure with which to communicate the solution at different levels of abstraction to
  different audiences.

## Part 2 - The software architecture role
## Part 3 - Designing software
## Part 4 - Visualising software
## Part 5 - Documenting software
## Part 6 - Software architecture in the development life cycle


