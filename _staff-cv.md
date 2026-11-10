<!--
DRAFT — Staff / Principal Engineer version.
Placeholders in [square brackets] need real facts before this goes anywhere.
The leading underscore in the filename stops Jekyll/GitHub Pages publishing this file.
-->
# Gregory Gulrajani

_Staff / Principal Engineer · platform architecture, identity, search and AI-assisted engineering · Edinburgh, Scotland_ <br>

[E-Mail](mailto:greg@gulrajani.org) | [Mobile](tel:+447939068324) | [LinkedIn](https://www.linkedin.com/in/greg-gulrajani-091771/) | [Github](https://github.com/greggulrajani/)

Staff engineer with over 20 years' experience, including 12 years at Nucleus Financial growing from senior developer to principal engineer on a £17bn regulated wealth platform. I modernise legacy platforms without stopping delivery, design identity, search and cloud architecture, and lead teams through change, most recently bringing agentic AI development to three teams at Amici Procurement. I lead through working prototypes and clear trade-offs, so decisions rest on evidence.

## Skills

- **Architecture:** distributed systems, modular monoliths and microservices, multi-tenancy, identity (OIDC, SSO, Keycloak), API design (GraphQL, REST), search (Lucene, chemical similarity)
- **Cloud and delivery:** AWS (Fargate, Lambda, S3, DynamoDB), Azure Container Apps, Docker, CI/CD (Jenkins, GitHub), on-demand environments
- **Languages:** Java, Python, JavaScript, React, SQL
- **AI-assisted engineering:** GitHub Copilot, Claude Code, agentic workflows, AI code review and governance
- **Leadership:** technical strategy, cross-team influence, hiring and mentoring, regulated environments (CASS, MiFID II, GDPR)

## Experience

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
A regulated wealth management platform with £17bn in assets under administration (AUA) and 200,000 customers. Over 12 years I grew from senior developer to principal engineer, reporting to the CTO from 2015. I built the development team from just me to 18 developers and took the platform from a Java monolith to cloud services on AWS.

- **Hiring and people:** hired around 30 engineers. I involved the whole team in interviews and made decisions by quorum. With the heads of other technical departments, I co-created a rotation programme that moved new hires through every technical department, which HR praised after launch. I also handled performance management, including two improvement plans: one person left, and the other moved to a role where they thrived.
- **Regulation and security:** shaped engineering practice around CASS, MiFID II reporting and audit requirements. I set up tiered review for critical components such as frontend APIs, organised security training and supported penetration testing.

**Principal Engineer** _(Jan 2022 - Dec 2024)_

- Led technical direction across four Scrum teams of 18 developers, line-managing three lead developers.
- Modernised the legacy reporting and analysis tools, built on a server-side rendering framework with limited UX options and a shrinking pool of developers. Instead of a big-bang rewrite, I reworked the server side in place to serve a new JavaScript frontend, improving performance and features. Clients moved over tool by tool, and 30% of users had switched by the time I left.
- Led an evaluation of replacements for on-premises Jenkins: AWS CodePipeline versus Jenkins on a Fargate cluster. Chose Jenkins on Fargate as much cheaper, even including the DevOps time for upgrades.
- Designed the architecture to bring acquired wrap platforms behind a common front end. The integration was halted by legal issues with platform providers.
- Led integrations with around 30 third-party providers of reporting, analysis and research for customers.
- **_Technologies used:_** Java, JavaScript, React, AWS (Fargate, Lambda), Jenkins, Docker

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

## Earlier career

- **Contract Developer**, Royal London _(Aug 2012 - Dec 2012)_: improved calculation efficiency by 20%, removing the need for two production servers.
- **Contract Team Lead**, Vebnet / Standard Life _(Jan 2010 - Jul 2012)_: led a team of 3 to 7 developers, fixed major Hibernate performance bottlenecks in batch processing, and owned UAT and production support for batch.
- **Application Designer**, BSkyB _(Jan 2009 - Dec 2009)_: designed a rule-driven product selection application combining product, pricing and promotion data, and migrated a billing application from JAX-RPC to Spring-WS.
- **Contract Developer**, Allianz _(Oct 2007 - Jan 2009)_: built JSF and Seam user interfaces, including a replacement for a Lotus Notes application, with SOAP and JMS integration.
- **Contract Developer**, NCR _(Mar 2007 - Oct 2007)_: built NFC payment prototypes for Nokia handsets and NCR ATM and point-of-sale equipment.
- **Developer**, German Research Center for Artificial Intelligence (DFKI) _(Aug 2004 - Mar 2007)_: built semantic web (OWL) data integration in Python, and mentored new staff.
- **Developer**, Max Planck Institute for Psycholinguistics _(Aug 2002 - Mar 2004)_: designed XML and multimedia search frameworks in Java.

## Personal

- Avid hill runner: [Strava](https://www.strava.com/athletes/6909/)
- Photography: [Instagram](https://www.instagram.com/gulrajanigregory/) | [Blipfoto](https://www.blipfoto.com/gwak)
  <br><br>
