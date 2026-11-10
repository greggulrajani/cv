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
A procurement platform for the biomedical industry, serving around 500 client organisations and 25,000 users. I report to the CTO and work across three Scrum teams (about 17 developers), moving between them to lead cross-team initiatives and to find and fix bottlenecks in delivery, working with team leads, QA and product managers.

- **Identity re-architecture:** led the redesign of identity and multi-tenancy on Keycloak, replacing a rushed migration from Microsoft Identity Server that was struggling under load. Phase one moved 500 client organisations to a new data model, cutting role operations from up to a minute to milliseconds and working-day memory use by 15%. Phase two, a new management UI and backend, is in development.
- Designed a hierarchical, multi-tenant organisation model on a single Keycloak realm, aligned with Keycloak's emerging built-in Organisations support so Amici can switch to it later without re-architecting.
- Assessed two options for TLS certificate handling across the microservices: keeping distributed resource servers or moving to a BFF/API gateway. Set out the cost and delivery trade-offs, which led to a decision to keep the existing architecture.
- **Search:** directed the overhaul of search across a 60-million-product catalogue. After trialling LLM approaches, replaced naive search-term splitting with lightweight rules and keyword lists, raising search-to-basket conversion by 18% with no significant extra compute.
- Directed the build of a chemical similarity index from PubChem, filtering 124 million compounds down to the 30 million relevant to customers. Chose Morgan fingerprints with Tanimoto scoring after Hugging Face chemistry models proved less consistent. Recommendations from the index lift conversion by 4% where shown.
- **Developer platform:** built on-demand environments on Azure Container Apps. Developers and AI agents can spin up a full stack from any combination of repositories and branches in 4–6 minutes, for testing, regression runs and security scans. This ended contention over a few shared integration environments.
- Prototyped a GDPR anonymisation pipeline so developers can work with realistic data. Used AI to audit the schema and list every table and column holding client or account personal data, including free-text memo fields. That list drove the data-seeding scripts, which I prototyped and the data team refined.
- **AI-assisted engineering:** led the adoption of agentic AI (GitHub Copilot and Claude Code) across all three teams. AI code review now runs before and after every commit, agentic workflows handle bug fixes, boilerplate and security scans, and frontend ticket velocity has improved by 7–8%.
- Introduced labelling for agent-written commits and size caps on agentic pull requests after early large AI-generated commits overloaded reviewers. Adopted across engineering, the labels let reviewers prioritise where human attention is needed.
- Shaped technical direction mainly through working proofs of concept, giving leads something concrete to weigh trade-offs against, backed by C4 diagrams and workshops tailored to technical and business audiences.
- **_Technologies used:_** Azure, Azure Container Apps, .NET, Java, Python, Keycloak, Lucene, Docker, GitHub, GitHub Copilot, Claude Code
  <br><br>

**[Nucleus Financial](https://www.nucleusfinancial.com/)** _(Jan 2013 - Dec 2024)_ <br>
A regulated wealth management platform with £17bn in assets and 200,000 customers. Over 12 years I grew from senior developer to principal engineer, reporting to the CTO from 2015. I built the development team from just me to 18 developers and took the platform from a Java monolith to cloud services on AWS.

- **Hiring and people:** hired around 30 engineers. I involved the whole team in interviews and made decisions by quorum. With the heads of other technical departments, I co-created a rotation programme that moved new hires through every technical department, which HR praised after launch. I also handled performance management, including two improvement plans: one person left, and the other moved to a role where they thrived.
- **Regulation and security:** shaped engineering practice around CASS, MiFID II reporting and audit requirements. I set up tiered review for critical components such as frontend APIs, organised security training and supported penetration testing.

**Principal Engineer** _(Jan 2022 - Dec 2024)_
- Led technical direction across four Scrum teams of 18 developers, line-managing three lead developers.
- Modernised the legacy reporting and analysis tools, built on a server-side rendering framework with limited UX options and a shrinking pool of developers. Instead of a big-bang rewrite, I reworked the server side in place to serve a new JavaScript frontend, improving performance and features, and moved clients over tool by tool.
- Led an evaluation of replacements for on-premises Jenkins: AWS CodePipeline versus Jenkins on a Fargate cluster. Chose Jenkins on Fargate as much cheaper, even including the DevOps time for upgrades.
- Designed the architecture to bring acquired wrap platforms behind a common front end. The integration was halted by legal issues with platform providers.
- Led integrations with third-party providers of reporting, analysis and research for customers.
- **_Technologies used:_** Java, JavaScript, AWS (Fargate, Lambda), Jenkins, Docker, [D2?]

**Software Architect** _(Jan 2017 - Dec 2021)_
- Designed the platform as a composable monolith of Maven modules that could be split into services when scaling or team ownership required it. Extracted four services to AWS Fargate and Lambda for scaling: change-data-capture batch processing, long-running reports, the iOS app backend and file storage.
- Proposed and won agreement for a GraphQL API to replace a granular HATEOAS API that internal frontend teams and third parties found hard to use. It cut bandwidth costs by 13%, improved developer productivity and morale, and drew positive feedback from third parties.
- Co-developed an integration test strategy that let the team deploy several times a day with confidence.
- Kept stakeholders updated on strategy and current projects, balancing developers' interests with the needs of the business during fierce competition for talent.
- **_Technologies used:_** AWS Lambda, Fargate, S3, ELB, DynamoDB, Docker, GraphQL, Java, Postgres, Oracle, React, JavaScript, Prometheus, Grafana

**Lead Developer** _(Jan 2015 - Dec 2016)_
- Took on line management of a team of 5 developers, reporting to the CTO.
- Introduced Docker into the CI/CD pipeline, and started the move from server-rendered web applications to React frontends.
- Introduced a hypermedia REST API.
- Built an offline cache for millions of rows that cut render times in client-facing apps and let Nucleus meet regulatory reporting requirements.
- Built a server-side PDF printing service that reused the existing React frontends.
- **_Technologies used:_** Docker, Maven, Jenkins, React, Java, Gerrit, Oracle

**Senior Developer** _(Jan 2013 - Dec 2014)_
- Designed a modular platform that adapts easily to new business requirements.
- Built an app store that lets third-party vendors integrate and sell applications to platform users.
- Built a SOAP bridge providing auditing, access control and billing, and a document store with search, bulk upload and auditing.
- **_Technologies used:_** Java, Spring, Wicket, CXF-SOAP, Oracle, Linux
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
