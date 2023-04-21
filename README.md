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
## Part 4 - Visualising software
## Part 5 - Documenting software
## Part 6 - Software architecture in the development life cycle


