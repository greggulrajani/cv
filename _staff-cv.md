<!--
DRAFT — Staff / Principal Engineer version.
Placeholders in [square brackets] need real facts before this goes anywhere.
The leading underscore in the filename stops Jekyll/GitHub Pages publishing this file.
-->
# Gregory Gulrajani

_Software engineer, architect and leader based in Edinburgh, Scotland_ <br>

[E-Mail](mailto:greg@gulrajani.org) | [Mobile](tel:+447939068324) | [LinkedIn](https://www.linkedin.com/in/greg-gulrajani-091771/) | [Github](https://github.com/greggulrajani/)

Staff engineer with over 20 years' experience designing, building and scaling platforms across procurement, wealth management, insurance and research. I specialise in modernising legacy systems, cloud and identity architecture, and helping teams adopt better ways of working, most recently LLM-assisted development.

## 💻 Technical Experience

**Staff Engineer** @ [Amici Procurement](https://www.amiciprocurement.com/) _(Jan 2025 - present)_ <br>
A procurement platform for the biomedical industry, serving around 500 client organisations and 25,000 users. I report to the CTO and work across three Scrum teams (about 17 developers), moving between them to lead cross-team initiatives with team leads, QA and product managers.

- **Identity re-architecture:** led the redesign of identity and multi-tenancy on Keycloak, replacing a rushed migration from Microsoft Identity Server that was struggling under load. Phase one moved 500 client organisations to a new data model, cutting role operations from up to a minute to milliseconds and working-day memory use by 15%. Phase two, a new management UI and backend, is in development.
- Designed a hierarchical, multi-tenant organisation model on a single Keycloak realm, aligned with Keycloak's emerging built-in Organisations support so Amici can switch to it later without re-architecting.
- Assessed two options for TLS certificate handling across the microservices: keeping distributed resource servers or moving to a BFF/API gateway. Set out the cost and delivery trade-offs, which led to a decision to keep the existing architecture.
- **Search:** directed the overhaul of search across a 60-million-product catalogue. After trialling LLM approaches, replaced naive search-term splitting with lightweight rules and keyword lists, raising search-to-basket conversion by 18% with no significant extra compute.
- Directed the build of a chemical similarity index from PubChem, filtering 124 million compounds down to the 30 million relevant to customers. Chose Morgan fingerprints with Tanimoto scoring after Hugging Face chemistry models proved less consistent. Recommendations from the index lift conversion by 4% where shown.
- **Developer platform:** built on-demand environments on Azure Container Apps. Developers and AI agents can spin up a full stack from any combination of repositories and branches in 4–6 minutes, for testing, regression runs and security scans. This ended contention over a few shared integration environments.
- Spearheaded a GDPR-compliant anonymisation pipeline for client and account data, including personal data hidden in free-text memo fields, so developers can work with realistic data.
- [Branching and merging: what you changed and the result.]
- **AI-assisted engineering:** led the adoption of agentic AI (GitHub Copilot and Claude Code) across all three teams. AI code review now runs before and after every commit, agentic workflows handle bug fixes, boilerplate and security scans, and frontend ticket velocity has improved by 7–8%.
- Introduced labelling for agent-written commits and size caps on agentic pull requests after early large AI-generated commits overloaded reviewers. Adopted across engineering, the labels let reviewers prioritise where human attention is needed.
- Got architecture decisions agreed through prototypes, C4 diagrams and workshops, tailored to technical and business audiences.
- **_Technologies used:_** Azure, Azure Container Apps, .NET, Java, Python, Keycloak, Lucene, Docker, GitHub, GitHub Copilot, Claude Code
  <br><br>

**Principal Engineer** @ [Nucleus Financial](https://www.nucleusfinancial.com/) _(Jan 2022 - Dec 2024)_ <br>
A platform for managing wealth.

- Led development across four Scrum teams, driving collaboration and timely delivery of high-quality features.
- Prototyped and implemented scalable solutions that shortened development cycles and improved team productivity.
- Worked with cross-functional stakeholders to refine requirements, align business goals with technical solutions and report progress clearly.
- Reviewed and approved critical patchsets, maintaining code quality and system reliability.
- Modernised a legacy application with a lightweight architecture that preserved core functionality while improving the user experience and feature set.
- Led the migration of the CI/CD stack to AWS, using cloud-native services to speed up deployments and improve operational efficiency.
- Developed and standardised a data-driven interview process, improving the accuracy of technical hiring decisions across engineering teams.
- Aligned security practices across development teams to meet best practice and regulatory standards.
- Defined and executed the technology roadmap for integrating multiple wrap platforms, positioning the company for scalable growth.
- **_Technologies used:_** Java, D2, AWS Services
  <br><br>

**Software Architect** @ [Nucleus Financial](https://www.nucleusfinancial.com/) _(Jan 2017 - Jan 2022)_ <br>

- Directed internal development and gave stakeholders strategic updates on current and upcoming projects, keeping work aligned with business objectives.
- Grew the development team by defining hiring criteria and processes to meet increasing demand.
- Designed and prototyped a microservices architecture, breaking a monolithic Java application into AWS Fargate and Lambda services for better scalability and flexibility.
- Developed a GraphQL API to replace the existing Hypermedia API, cutting bandwidth costs by 13%.
- Co-developed an integration test strategy that let the team deploy multiple times per day with confidence and less downtime.
- Took part in Scrum ceremonies, code reviews and planning across four teams.
- **_Technologies used:_** AWS Lambda, Fargate, S3, ELB, DynamoDB, Docker, GraphQL, Java, Postgres, Oracle, React, JavaScript, Prometheus, Grafana
  <br><br>

**Lead Developer** @ [Nucleus Financial](https://www.nucleusfinancial.com/) _(Jan 2015 - Jan 2017)_ <br>

- Introduced, designed and co-developed Docker infrastructure for the CI/CD pipeline.
- Introduced and began the migration from server-rendered web applications to client-side React frontends.
- Introduced and developed a Hypermedia RESTful API.
- Developed a browser-agnostic, server-side printing solution that reused existing React frontends to produce PDF output.
- Developed an offline caching mechanism for millions of rows that reduced render times in client-facing apps and allowed Nucleus to meet regulatory reporting requirements.
- Mentored and managed a team of 5 developers.
- Took part in code reviews and planning sessions.
- **_Technologies used:_** Docker, Maven, Jenkins, React, Java, Jira, Gerrit, Oracle
  <br><br>

**Senior Developer** @ [Nucleus Financial](https://www.nucleusfinancial.com/) _(Jan 2013 - Jan 2015)_ <br>

- Designed a modular platform that adapts easily to new business requirements.
- Developed an app store that lets third-party vendors integrate and sell applications to platform users.
- Developed a SOAP bridge providing auditing, ACLs and billing.
- Developed a document store with search, bulk upload and auditing.
- Designed and maintained development and production servers.
- **_Technologies used:_** Java, Spring, Wicket, CXF-SOAP, Oracle, Unix (Linux)
  <br><br>

**Contract Developer** @ [Royal London](http://royallondon.com/) _(Aug 2012 - Dec 2012)_ <br>

- Moved all SQL queries out of inline Java code.
- Improved calculation efficiency by 20%, removing the need for two production app servers.
- Found and fixed a major date and time handling bug.
- Helped with the migration to JSF.
- **_Technologies used:_** Java, JSF, Spring
  <br><br>

**Contract Team Lead** @ [Vebnet / Standard Life](https://www.standardlife.com/) _(Jan 2010 - July 2012)_ <br>

- Led a team of 3 to 7 people: ran daily stand-ups, tracked progress, and reviewed every developer's uncommitted diffs daily. Assigned stronger developers to sensitive areas and had them peer review others' code.
- Identified major Hibernate performance bottlenecks and improved batch processing performance; fixed many subtle mapping issues and critical Hibernate exceptions.
- Debugged class loader issues across multiple development and production containers.
- Profiled UAT and production servers to find performance bottlenecks.
- Ported and refactored legacy code from an earlier version of the application, adding unit tests as it was ported.
- Developed a user-facing JavaScript module that reduced client requests for bespoke developer and analyst work.
- Owned UAT and production support for batch processing, managing, assigning and tracking all bugs in that component.
- **_Technologies used:_** Java, Rhino JSR-223, Wicket
  <br><br>

**Application Designer** @ [BSkyB](https://www.sky.com/) _(Jan 2009 - Dec 2009)_ <br>

- Refactored a project of many tightly coupled components into a few components with clear scope and intent, using Agile and refactoring techniques.
- Replaced or augmented in-house MVC add-ons, unit test frameworks and RPC patterns with third-party libraries, simplifying the codebase and increasing developer productivity.
- Designed and began development of a rule-driven product selection application combining product, pricing, promotion and discount data. Chose Wicket after evaluating GWT and JSF, and used iterative development to handle shifting requirements.
- Migrated a billing application from IBM's JAX-RPC SOAP stack to Spring-WS using JAXB, Axiom and JMS, speeding up binding generation, configuration and debugging.
- **_Technologies used:_** Java, Spring, WebSphere, Unix (Linux), jQuery, JMS, SOAP
  <br><br>

**Contract Developer** @ [Allianz](https://www.allianz.com/) _(Oct 2007 - Jan 2009)_ <br>

- Developed a Seam user interface for a message-based batch processing application with external developers.
- Developed JSF UI components to replace a Lotus Notes application.
- Extended the Hibernate reverse engineering script to add JAXB annotations to POJOs and detect cyclic dependencies.
- Implemented SOAP-based interfaces.
- Integrated associated projects into the Spring framework.
- **_Technologies used:_** Java, Seam, SOAP, JMS, Hibernate-JPA, DB2, AS400
  <br><br>

**Contract Developer** @ [NCR Corporation](https://www.ncr.com/) _(Mar 2007 - Oct 2007)_ <br>

- Developed UML use-case scenarios using Nokia NFC handsets and NCR ATM and point-of-sale equipment.
- Developed a six-month project plan for two developers.
- Developed NFC Java MIDlets for Nokia NFC mobile phones.
- Developed a REST/SOAP API for server operations and mobile phone targets.
- Wrote an OPOS NFC/RFID reader service object for the NCR FastLane platform.
- **_Technologies used:_** J2ME, NFC, RFID, C++
  <br><br>

**Developer** @ [German Research Center for Artificial Intelligence](https://www.dfki.de/) _(Aug 2004 - Mar 2007)_ <br>

- Developed a Plone/Zope database driver for the Sesame OWL database.
- Wrote an application to synchronise the relational and OWL databases.
- Developed Plone archetypes providing ACL-controlled CRUD access to OWL data.
- Managed and mentored new employees on a range of programming tasks.
- **_Technologies used:_** Python, Unix, Plone, OWL, Sesame
  <br><br>

**Developer** @ [Max Planck Institute](https://www.mpi.nl/) _(Aug 2002 - Mar 2004)_ <br>

- Designed and developed an XML search framework, including an XML Schema parser for the search engine.
- Developed double-buffered visualisation components for a multimedia linguistic annotation tool.
- Integrated the JNLP launch protocol into all applications developed at the institute.
- Designed and developed multimedia search framework software.
- **_Technologies used:_** Java, JNI, Swing/AWT, Oracle

## 📌 Personal

- Father
- Avid hill runner: [Strava](https://www.strava.com/athletes/6909/)
- Photography: [Instagram](https://www.instagram.com/gulrajanigregory/) | [Blipfoto](https://www.blipfoto.com/gwak)
  <br><br>
