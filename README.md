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
* Becoming a software architect isn’t something that simply happens overnight or with a
  promotion. It’s a role, not a rank. It’s the result of an evolutionary process where you’ll gradually
  gain the experience and confidence that you need to undertake the role. While the term “software
  developer” is fairly well understood, “software architect” isn’t
* !!      Notice that I said “role” here; it’s something that can be performed by a single person or shared amongst the team.
* Here are the things that I consider to make up the software architecture role:
* 1. Architectural Drivers - The first part of the role is about understanding the business goals and managing the architectural drivers,
       which includes the requirements (both functional and non-functional) and the
       constraints of the environment. Software projects often get caught up on asking users what
       features they want, but rarely ask them what non-functional requirements (or quality attributes)
       that they need.
       Non-functional requirements and constraints often have a huge influence on
       the software architecture, so explicitly including them as a part of the software architecture role
       helps to ensure that they are considered and taken into account.
* 2. Designing Software -  A key part of designing software is technology selection, which is typically a fun exercise but
     it does have its fair set of challenges. For example, some organisations have a list of approved
     technologies that you are forced to choose from, while others have rules in place that don’t allow
     open source technology with a specific licence to be used. Then you have all of the other factors
     such as cost, licensing, vendor relationships, technology strategy, compatibility, interoperability,
     support, deployment, upgrade policies, end-user environments and so on.
*  3. Technical Risks - What we’ve looked at so far will help you focus on building a good solution, but it doesn’t
      guarantee success. Simply throwing together the best designs and the best technologies doesn’t
      necessary mean that the overall architecture will be successful.  Furthermore, I don’t 
      always trust myself to get it (architecture) right first time. Your mileage may vary though!
      Throughout the software development life cycle, we undertake a number of different types of
      testing in order to give us confidence that the system we are building will work when delivered.
      So why don’t we do the same for our architecture? If we can test our architecture, we can prove
      that it works. And if we can do this as early as possible, we can reduce the overall risk of project
      failure. Like good chefs, architects should taste what they are producing.
*  4. Architecture Evolution - More often than not, software is designed and then the baton is passed over to a development
      team, effectively treating software development as a relay sport. This is counterproductive
      because the resulting software architecture needs to be taken care of.
      If an architect has created an architecture, why shouldn’t they own and evolve
      that architecture throughout the rest of the delivery too? This is about continuous technical
      leadership rather than simply being involved at the start of the life cycle and hoping for the best
* 5. Coding - Many software architects are master builders, so it makes sense to keep those skills up to
     date. In addition, coding provides a way for the architect(s) to share the software development
     experience with the rest of the team, which in turn helps them better understand how the
     architecture is viewed from a development perspective.
* Although the need for thinking about software architecture is usually acknowledged, the
  responsibilities of the software architecture role often aren’t clear.
* Regardless of what you call it (e.g. Architect, Tech Lead, Principal Designer, etc), my advice is
  simple. If you don’t have something that you can point at and say, “this is what we expect of our
  software architects”, take some time to create something.
* If this is the case, building prototypes and proof of concepts related to the software system in
  question is a great way to be involved. Again, this allows you to build some rapport with the
  team and it’s a great way to evaluate that your architecture will work.
* In essence, the traditional architect role has diverged into two roles. One is the structural
  engineer, who ensures that the building doesn’t fall over. And the other is the architect, who
  interacts with the client to gather their requirements and design the building from an aesthetic perspective.
* Performing a software architecture role across a number of teams is not an effective way to work
  though. Typically this situation occurs when there is a centralised group of architects (e.g. in an
  “Enterprise Architecture Group”) who are treated as shared resources. From what I’ve read, the
  master masons were dedicated to a single building site at any one point in time and this is exactly
  the approach that we should adopt within our software development teams.
* A mason would have an apprentice working for him. When the mason moved on
  to a new job, the apprentice would move with him. When a mason felt that his
  apprentice had learned enough about the trade, he would be examined at a Mason’s Lodge.
* Breadth of knowledge - it’s important for software architects to have a breadth of technology knowledge too. Sure, they may be
  specialists in Java or Oracle, but the role demands more. For example, the people in the software architecture
  role should be able to answer the following types of questions too:
* * Is the technology that we’ve chosen the most appropriate given the other options available?
* * What are the other options for the design and build of this system?
* * Is there a common architectural pattern that we should be using?
* * Do we understand the trade-offs of the decisions that we’re making?
* * Have we catered for the desired quality attributes?
* * How can we prove that this architecture will work?
* Does this mean that the software architect should be an expert in all of the technologies that are in use on
  any give software system? No.
* Pair programming has benefits, so why not pair architecting?
* My advice would be to start with some control and listen to the feedback in order to fine-tune
  it as you progress. If the team are asking lots of “why?” and “how?” questions, then perhaps
  more guidance is needed. If it feels like the team are fighting against you all of the time, perhaps
  you’ve pushed that lever too far. There’s no universally correct answer, but some control is a
  good thing and it’s therefore worth spending a few minutes looking at how much is right for
  your own team.
* If you’re a software developer:
* * Understand the big picture: Taking some time out to understand the big picture will
  help you understand the context in which the architectural decisions are being made and
  enhance your understanding of the system as a whole.
* * Challenge architectural decisions: With an understanding of the big picture, you now
  have the opportunity to challenge the architectural decisions being made. Architecture
  should be a collaborative process and not dictated by people that aren’t engaged in the
  project day-to-day. If you see something that you don’t understand or don’t like, challenge it.
* * Ask to be involved: Many projects have an architect who is responsible for the architecture and it’s
  this person who usually undertakes all of the “architecture work”. If you’re a
  developer and you want to get more involved, just ask. You might be doing the architect a favour!
* Let’s face it, most software developers don’t get to take a blank sheet of paper and design software
  from scratch all that frequently, regardless of whether that design is up front or evolutionary and
  whether it’s a solo or collaborative exercise.
## Part 3 - Designing software
* Regardless of the process that you follow (traditional and plan-driven vs lightweight and
  adaptive), there’s a set of common things that really drive, influence and shape the resulting
  software architecture:
* * Functional requirements
    In order to design software, you need to know something about the goals that it needs to satisfy.
    If this sounds obvious, it’s because it is. Having said that, I have seen teams designing software
    (and even building it) without a high-level understanding of the features that the software should
    provide to the end-users. Some might call this being agile, but I call it foolish. Even a rough, short
    list of features or user stories (e.g. a Scrum product backlog¹) is essential. Requirements drive
    architecture.
* * Quality Attributes
    Quality attributes are represented by the non-functional requirements and reflect levels of
    service such as performance, scalability, availability, security, etc. These are mostly technical
    in nature and can have a huge influence over the resulting architecture, particularly if you’re
    building “high performance” systems or you have desires to operate at “Google scale”.
    Retrofitting high performance, scalability, security, availability, etc into an existing codebase is
    usually incredibly difficult and time-consuming.
* * Constraints
    We live in the real world and the real world has constraints. For example, the organisation that
    you work for probably has a raft of constraints detailing what you can and can’t do with respect
    to technology choice, deployment platform, etc.
* * Principles
    Where constraints are typically imposed upon you, principles are the things that you want to
    adopt in order to introduce consistency and clarity into the resulting codebase. These may be
    development principles (e.g. code conventions, use of automated testing, etc) or architecture
    principles (e.g. layering strategies, architecture patterns, etc).
* Quality Attributes (non-functional requirements)
  Alternative, arguably better yet less commonly used names for non-functional requirements include
  “system characteristics” or “quality attributes”. A non-exhaustive list of the common quality attributes is as follows:
* * Performance
* * Scalability
* * Availability
* * Security
* * Disaster Recovery
* * Accessibility
* * Monitoring
* * Management
* * Audit
* * Flexibility
* * Extensibility
* * Maintainability
* * Legal, Regulatory and Compliance
* * Internationalisation
* * Localisation
* A web-based system in the
  finance industry will likely have a different set of quality attributes to an internal system used
  within the telco industry. My advice is to learn about the quality attributes common within your
  domain and focus on those first when you start building a new system or modifying an existing system.
* Working with non-functional requirements
  Regardless of what you call them, you’ll often need to put some effort into getting the list of
  non-functional requirements applicable to the software system that you’re building.
* *  1.Capture  (Dan: ask the stakeholders what they want concerning the non-functional requirements)
     If you ask a business sponsor what level of system availability they
     want, you’ll probably get an answer similar to “100%”, “24 by 7 by 365” or “yes please, we want all of it”.
* *  2.Refine
     Once you’ve started asking those tricky questions related to non-functional requirements, or
     you’ve been fortunate enough to receive some information about them, you’ll probably need to
     refine them. Rather than asking how much availability is needed and getting the inevitable “24 by 7” answer, you
     can vary the questions depending on who you are talking to. For example:
* * * “How much system downtime can you tolerate?”
* * * “What happens if the core of the system fails during our normal working hours of 9am until 6pm?”
* * * “What happens if the core of the system fails outside of normal working hours?”
* * *  Why does the system need to be available?
* * *  When we talk about “high security”, what is it that we’re protecting?
* * * How many concurrent users should the system support on average? What about peak times?
* * * What response time is deemed as acceptable? Is this the same across all parts of the system
       or just specific features?
* * * How exactly do we need to secure the system? Do we really need to encrypt the data or
       is restricted access sufficient?
* * 3.Challenge
       With this in mind, we all know what response we’ll get if we ask people whether they need
       something. They’ll undoubtedly say, “yes”. This is why prioritising functional requirements, user
       stories, etc is hard. Regardless of the prioritisation scale that you use (MoSCoW¹, High/Medium/Low, etc),
       everything will end up as a “must have” on the first attempt at prioritisation. You
       could create a “super-must have” category, but we know that everything will just migrate there.
       A different approach is needed and presenting the cost implications can help focus the mind.
       Anything is possible but everything has a trade-off. Explaining those trade-offs can help find the
       best solution for the given context. (example in the notes...by introducing cost in question, client 
       might change his mind about what is important and what is not)
* Principles
  While constraints are imposed upon you, principles are the things that you want to adopt in
  order to introduce standard approaches, and therefore consistency, into the way that you build
  software. There are a number of common principles, some related to development and others
  related to architecture.
* * Development principles
* * * Coding standards and conventions: “We will adopt our in-house coding conventions for
    [Java|C#|etc], which can be found on our corporate wiki.”
* * * Automated unit testing: “Our goal is to achieve 80% code coverage for automated unit
    tests across the core library, regardless of whether that code is developed using a test-first or test-last approach.”
* * * Static analysis tools: “All production and test code must pass the rules defined in
    [Checkstyle|FxCop|etc] before being committed to source code control.”
* * Architecture principles
* * * Layering strategy: A layered architecture usually results in a software system that has a
      high degree of flexibility because each layer is isolated from those around it. For example,
      you may decompose your software system into a UI layer, a business layer and a data access
      layer. Making the business layer completely independent of the data access layer means
      that you can (typically) switch out the data access implementation without affecting the
      business or UI layers. You can do this because the data access layer presents an abstraction
      to the business layer rather than the business layer directly dealing with the data storage
      mechanism itself. If you want to structure your software this way, you should ensure that
      everybody on the development team understands the principle. “No data access logic in
      the UI components or domain objects” is a concrete example of this principle in action
* * * Placement of business logic: Sometimes you want to ensure that business logic always
      resides in a single place for reasons related to performance or maintainability. In the case
      of Internet-connected mobile apps, you might want to ensure that as much processing as
      possible happens on the server. Or if you’re integrating with a legacy back-end system that
      already contains a large amount of business logic, you might want to ensure that nobody
      on the team attempts to duplicate it.
* * * High cohesion, low coupling, SOLID¹, etc: There are many principles related to the
      separation of concerns, focussing on building small highly cohesive building blocks that
      don’t require too many dependencies in order to do their job.
* * * Stateless components: If you’re building software that needs to be very scalable, then
      designing components to be as stateless as possible is one way to ensure that you can
      horizontally scale-out your system by replicating components to share the load. If this is
      your scalability strategy, everybody needs to understand that they must build components
      using the same pattern. This will help to avoid any nasty surprises and scalability
      bottlenecks in the future.
* * * Stored procedures: you either love them or you hate them. There are advantages and disadvantages to using or
      not using stored procedures, but I do prefer it when teams just pick one approach for data
      access and stick to it. There are exceptions to every principle though.
* * * Domain model - rich vs anaemic: Some teams like having a very rich domain model
      in their code, building systems that are very object-oriented in nature. Others prefer a
      more anaemic domain model where objects are simply data structures that are used by
      coarse-grained components and services. Again, consistency of approach goes a long way.
* * * Use of the HTTP session: If you’re building a website, you may or may not want to
      use the HTTP session for storing temporary information between requests. This can often
      depend on a number of things including what your scaling strategy is, where session backed objects are
      actually stored, what happens in the event of a server failure, whether
      you’re using sticky sessions, the overhead of session replication, etc. Again, everybody on
      the development team should understand the desired approach and stick to it.
* * * Always consistent vs eventually consistent: Many teams have discovered that they
      often need to make trade-offs in order to meet complex non-functional requirements.
      For example, some teams trade-off data consistency for increased performance and/or
      scalability. Provided that we do see all Facebook status updates, does it really matter if we
      all don’t see them immediately? Your context will dictate whether immediate or delayed
      consistency is appropriate, but a consistent approach is important.
* If you don’t understand the trade-offs that you’re making by choosing technology X over Y,
  you shouldn’t be making those decisions. It’s crucial that the people designing software systems
  understand technology. This is why software architects should be master builders.
* Experience influences software design
  Our own knowledge, experience and preferences tend to influence how we design software,
  particularly if it’s being done as a solo activity. In the absence of communication, we tend to
  make assumptions about where components will sit and how features will work based upon our
  own mental model of how the sofware should be designed. Getting these assumptions out into
  the open as early as possible can really help you avoid some nasty surprises before it’s too late.
  One of the key reasons I prefer using a whiteboard to design software is because it encourages
  a more collaborative approach than somebody sitting on their own in front of their favourite
  modelling tool on a laptop. If you’re collaborating, you’re also communicating and challenging each other
## Part 4 - Visualising software
* This part of the book is about visualising software architecture using a collection of lightweight,
  yet effective, sketches.
* I’m very much a visual person myself and fall into latter camp. I like being able to visualise a
  problem before trying to find a solution. Describe a business process to me and I’ll sketch up a
  summary of it. Talk to me about a business problem and I’m likely to draw a high-level domain
  model. Visualising the problem is a way for me to ask questions and figure out whether I’ve
  understood what you’re saying. I also like sketching out solutions to problems, again because
  it’s a great way to get everything out into the open in a way that other people can understand
  quickly
* Context, containers and components diagrams are usually sufficient. (see examples in the bookPics folder)
* Software architecture is about structure, which is about things (boxes) and how they interact (lines).
  This diagram has one, but not the other. It’s telling a story, but not the whole story.
* Granted there are many options and often teams don’t like committing early without putting
  together some prototypes. No problem, just annotate those lines on the diagram with the list of
  potential options instead so we can at least have a better conversation.
*  C4: context, containers, components and classes
   When describing software through pictures, we have a tendency to create a single uber-diagram that includes as
   much detail as possible at every level of abstraction simultaneously. This may be because we’re anticipating
   questions or because we’re a little too focussed on the specifics of how the system works at a code level.
   Such diagrams are typically cluttered, complex and confusing. Picking up a tool such
   as Microsoft Visio, Rational Software Architect or Sparx Enterprise Architect usually adds to the
   complexity rather than making life easier.
*  A better approach is to create a number of diagrams at varying levels of abstraction. A number
   of simpler diagrams can describe software in a much more effective way than a single complex
   diagram that tries to describe everything
* With this set of abstractions in mind, I tend to draw the following types of diagrams when
  summarising the static view of my software:
  1. Context: A high-level diagram that sets the scene; including key system dependencies and actors.
  2. Container: A container diagram shows the high-level technology choices, how responsibilities are distributed across them and how the containers communicate.
  3. Component: For each container, a component diagram lets you see the key logical
  components and their relationships.
  4. Classes: This is an optional level of detail and I will draw a small number of high-level
  UML class diagrams if I want to explain how a particular pattern or component will be (or
  has been) implemented. The factors that prompt me to draw class diagrams for parts of the
  software system include the complexity of the software plus the size and experience of the
  team. Any UML diagrams that I do draw tend to be sketches rather than comprehensive
  models.
* Context diagram - see book notes and bookPics about what how etc
* Container diagram - see book notes and bookPics about what how etc
* Component diagram - see book notes and bookPics about what how etc
* The thing is though, you don’t need a UML tool in order to architect and design software. I’ve
  conducted a number of informal polls during my conference talks over the past few years and
  only 10-20% of the audience said that they regularly used UML in their day to day work. Often
  a blank sheet of paper, flip chart or whiteboard together with a set of sticky notes or index cards
  is all you need, particularly when you have a group of people who want to undertake the design
  process in a collaborative way. Have you ever tried to get three or four people collaborating
  around a laptop screen?
* Effective sketches          (things to consider when doing NO UML diagrams..aka basic sketches on a whiteboard)
  If you are going to use “NoUML” diagrams (i.e. anything that isn’t UML), here are some things to
  think about, both when you’re drawing sketches on a whiteboard and if you decide to formalise
  them in something like Microsoft Visio afterwards.
* * Titles
    The first thing that can really help people to understand a diagram is including a title. If you’re
    using UML, the diagram elements will provide some information as to what the context of the
    diagram is, but that doesn’t really help if you have a collection of diagrams that are all just boxes
    and lines. Try to make the titles short and meaningful. If the diagrams should be read in a specific
    order, make sure this is clear by numbering them
* * Labels
    You’re likely to have a number of labels on your diagrams; including names of software systems,
    components, etc. Where possible, avoid using acronyms and if you do need to use acronyms
    for brevity, ensure that they are documented in a project glossary or with a key somewhere on
    the diagram
    The exceptions here are acronyms used to describe technology choices, particularly if they
    are used widely across the industry. Examples include things like JMS (Java Message Service),
    POJO (plain old Java object)
* * Shapes
    Most boxes and lines style sketches that I’ve seen aren’t just boxes and lines, with teams using
    a variety of shapes to represent elements within their software architecture. For example, you’ll
    often see cylinders on a diagram and many people will interpret them to be a database of some
    description. Make sure that you include an explanation to confirm whether this is the case or
    not.
* * Responsibilities
    If naming is one of the hardest things in software development, resist the temptation to have a
    diagram full of boxes that only contain names. A really simple way to add an additional layer of
    information to, and remove any ambiguity from, an architecture diagram is to annotate things
    like systems and components with a very short statement of what their responsibilities are. A
    bulleted list (7 ± 2 items¹) or a short sentence work well.
    (see "6 - Responsabilities remove ambiguity.png" for example)  
* * Lines
    Lines are an important part of most architecture sketches, acting as the glue that holds all of the
    boxes (systems, containers, components, etc) together. The big problem with lines is exactly this
    though, they tend to be thought of as the things that hold the other, more significant elements
    of the diagram together and don’t get much focus themselves. Whenever you’re drawing lines
    on sketches, ensure you use them consistently and that they have a clear purpose. For example:
* * * Line style (solid, dotted, dashed, etc): Is the line style relevant and, if so, what does it mean?
* * * Arrows: Do arrows point in the direction of dependencies (e.g. like UML “uses” relationships) or do
      they indicate the direction in which data normally flows?
    Often annotations on the lines (e.g. “uses”, “sends data to”, “downloads report from”, etc) can
    help to clarify the direction in which arrows are pointing, but watch out for any lines that have
    arrows on both ends!
* * Borders
    Adding borders (e.g. double lines, coloured lines, dashed lines, etc) around diagram elements
    can be a great way to add emphasis or to group related elements together. If you do this, make
    sure that it’s obvious what the border means, either by labelling the border or by including an
    explanation in the diagram key
* Diagram review checklist
  The software architecture process is about introducing structure and vision into software
  projects, so when reviewing architecture diagrams, here are a number of things that you might
  want to assert to ensure that this is the case. This checklist is applicable for diagrams produced
  during the initial architecture process, as well as those produced to retrospectively document an
  existing software system.
  1. I can see and understand the solution from multiple levels of abstraction.
  2. I understand the big picture; including who is going to use the system (e.g. roles, personas,
  etc) and what the dependencies are on the existing IT environment (e.g. existing systems).
  3. I understand the logical containers and the high-level technology choices that have been
  made (e.g. web servers, databases, etc).
  4. I understand what the major components are and how they are used to satisfy the
  important user stories/use cases/features/etc.
  5. I understand what all of the components are, what their responsibilities are and can see
  that all components have a home.
  6. I understand the notation, conventions, colour coding, etc used on the diagrams.
  7. I can see the traceability between diagrams and diagramming elements have been used consistently.
  8. I understand what the business domain is and can see a high-level view of the functionality
  that the software system provides.
  9. I understand the implementation strategy (frameworks, libraries, APIs, etc) and can almost
  visualise how the system will be or has been implemented.
## Part 5 - Documenting software
## Part 6 - Software architecture in the development life cycle


