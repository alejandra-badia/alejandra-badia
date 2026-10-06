# Alejandra Badia

Data Analyst | Business Intelligence | Technical Project Manager

Data Analyst & Technical Project Manager backed by 11 years of Technical Project Management experience in the oil & gas industry and a Master’s in International Business, with technical qualifications across Kimball dimensional modeling, advanced Power Query/DAX analytics, Azure cloud data flows, and full-stack API/dashboard programming.

## What I Do

* **Data Modeling & Analytics** – Designing robust data structures utilizing Kimball frameworks, star/galaxy schemas, and clean data preparation.
* **Business Intelligence & Dashboards** – Building custom, interactive visualization platforms and advanced Power Query/DAX reporting solutions.
* **Requirements & Functional Analytics** – Translating high-level project scopes and user stories into structured BI measurement blueprints to deliver actionable business metrics.
* **Full-Stack & Cloud Integration** – Integrating APIs, full-stack application logic (OOP/PHP), and Azure cloud data flows.
* **Business & Domain Analytics** – Applying quantitative analysis to marketing performance, operational workflows, and healthcare data to identify trends, inefficiencies, and actionable recommendations.

## Technical Skills

* **BI & Analytics:** Power BI · DAX · Power Query · Excel · SQL
* **Data & Modeling:** Kimball Dimensional Modeling · Star/Galaxy Schemas · Data Transformation · Data Quality
* **Programming & Integration:** Python (ML) · PHP · APIs · OOP
* **Cloud:** Azure Data Flows · Azure Data Lake / Bicep
* **Analytical Methods:** KPI Analysis · Trend Analysis · Variance Analysis · Root-Cause Analysis · Performance Analysis · Cohort Analysis

  
## Featured Projects

### E-Commerce Marketing BI Engine

**Business Problem:** Did a significant increase in marketing investment translate into profitable, sustainable revenue growth?

**What I Built:** An end-to-end Power BI analytics solution combining sales, marketing performance, and web-traffic data to evaluate the relationship between increased marketing investment, revenue growth, marketing efficiency, and profitability. The project began with stakeholder requirements and a BI measurement plan, translating the business question into defined KPIs, reporting requirements, data-grain specifications, and a Kimball-style dimensional model before implementation.

**Skills Demonstrated:** Business Requirements & KPI Definition · BI Measurement Planning · Dimensional Modeling · Data Transformation & Data Quality · DAX Analytics · Marketing Performance Analysis · Profitability Analysis · Executive Reporting · Data Visualization

**Tech Stack:** Power BI · DAX · Power Query · Kimball Dimensional Modeling · Fact Constellation / Galaxy Schema

**Key Findings & Recommendation:** Marketing investment increased 253% while Net Sales increased only 23%. Over the same periods, MER declined from 4.62x to 1.62x, blended ROAS from 4.37x to 1.69x, and Marketing Profit by 89%. The results indicate that marketing spend was scaled faster than revenue, reducing overall marketing efficiency and profitability. The recommendation is to reassess further budget increases, diagnose campaign-level performance and attribution, and validate incremental revenue before rescaling investment.

→ **[View Project](https://github.com/alejandra-badia/ecommerce-marketing-bi-engine)**


### BI Measurement Planner (Kimball Spec Engine)

**Business Problem:** How can BI teams eliminate scope creep, ambiguous metrics, and downstream modeling errors before writing code?

**What I Built:** A full-stack web application based on Ralph Kimball’s dimensional modeling framework to standardize BI project scoping and planning. The tool guides users step-by-step through business charter definition, KPI and DAX mathematical modeling, data-grain alignment, field-level ETL mapping, and dashboard design. It auto-populates dependencies across sections to ensure architectural integrity and exports production-ready specification files (`measurement_spec.json` and a Markdown `data_dictionary.md`).

**Skills Demonstrated:** BI Project Scoping & Governance · Kimball Dimensional Modeling (Star/Galaxy) · Data Grain Specification · Metric & DAX Formula Architecture · Field-Level ETL Mapping · Full-Stack Web Development · State Management & App Security

**Tech Stack:** PHP · JavaScript · HTML5/CSS3 · JSON · Markdown

**Key Findings / Impact:** Upfront planning and structured documentation can prevent project rework and avoid potentially broken data models. Enforcing early alignment on business objectives, user stories, and target metrics ensures the resulting data model, DAX measures, and dashboard layouts reflect stakeholder expectations before development begins. Standardizing this phase with auto-generated spec documents (`measurement_spec.json`) provides a clear, shared contract between business stakeholders, data analysts, and data engineers.

→ **[View Project](https://github.com/alejandra-badia/bi-measurement-planner)**


### Clinical Laboratory Operations & Interoperability Diagnostic Dashboard

**Business Problem:** Are hospital turnaround time (TAT) delays caused by IT/HL7 network interface drops, mechanical instrument bottlenecks, or clinical sample exception workflows?

**What I Built:** An interactive diagnostic dashboard in Microsoft Excel built to conduct root-cause analysis on clinical laboratory throughput and EHR data transmission. Ingested and cleaned 1,000 specimen records using Power Query ETL, structured a relational schema in Power Pivot connecting transactional lab runs to manufacturer SLA targets, and engineered dynamic DAX measures to audit data sync exceptions, latency thresholds, and mechanical processing variances.

**Skills Demonstrated:** Diagnostic Root-Cause Analysis · Power Query (ETL & Sanitization) · Power Pivot Relational Modeling · DAX Measure Engineering · Health Informatics (HL7 / EHR Interoperability) · Interactive Dashboard Design

**Tech Stack:** Microsoft Excel · Power Query · Power Pivot · DAX

### Summary of Results
* **Zero Patient Safety Leaks:** 0.0% invalid or errored results reached the patient's EHR chart, confirming robust LIS middleware rules and pre-analytical validation filters.
* **100% IT Interface Uptime:** Integration latency for valid samples averaged **1.4 minutes** (well within the <5-minute SLA threshold), confirming zero infrastructure or HL7 server transmission drops.
* **Manual Bottleneck Identified:** High latency (averaging **24.3 minutes**) was strictly confined to `Critical_Error` samples, representing human-driven verification and cancellation workflows rather than network drag.
* The recommendation is to implement automated 15-minute LIS hold alerts to accelerate review, schedule preventative maintenance on analyzers exceeding baseline cycle times, and collaborate with clinical supervisors to audit pre-analytical sample collection protocols.

→ **[View Project](https://github.com/alejandra-badia/clinical-laboratory-operations-dashboard)**


### Healthcare Analytics Cloud Foundation

**Business Problem:** How can clinical laboratory data be ingested and staged across a governed cloud pipeline so analysts can access clean data for reporting without exposing sensitive healthcare records or running up idle compute costs?

**What I Built:** Designed and deployed an enterprise Azure cloud foundation following the Cloud Adoption Framework (CAF) and Well-Architected Framework (WAF). Implemented an isolated Virtual Network with private endpoints and a "Deny-by-Default" firewall posture for serverless Azure Data Lake Storage Gen2 (ADLS Gen2). Structured a Medallion Architecture (`/1-bronze`, `/2-silver`, `/3-gold`) with Hierarchical Namespace enabled for downstream Microsoft Fabric integration, automated CI/CD validation via passwordless GitHub Actions (OIDC/WIF), and parameterized the deployment into reusable Bicep Infrastructure-as-Code templates.

**Skills Demonstrated:** Cloud Architecture & Governance · Azure Infrastructure as Code (Bicep / ARM) · Network Isolation & Security (VNet, Private Endpoints, DNS) · Identity & Access Management (Microsoft Entra ID, OIDC, RBAC) · Data Lakehouse Architecture (Medallion Layout, ADLS Gen2) · Cloud Cost Optimization & Total Cost of Ownership (TCO) Analysis

**Tech Stack:** Microsoft Azure · Azure Bicep · ADLS Gen2 · Microsoft Entra ID · GitHub Actions (OIDC) · Virtual Networks

**Key Findings & Strategic Recommendations:** Shifting from legacy compute to a decoupled, serverless data lakehouse structure eliminates data duplication bottlenecks, enabling Power BI to read optimized Delta-Parquet tables directly from curated storage via OneLake shortcuts. Isolating data stores behind private endpoints and scoping RBAC tightly to the resource group level ensures sensitive clinical telemetry remains fully protected from public exposure. The recommendation is to enforce Medallion data tiering as the ingestion standard for downstream Fabric pipelines, automate deployment repeatability using the parameterized Bicep templates, and maintain passwordless OIDC authentication across all analytics repos.

→ **[View Project](https://github.com/alejandra-badia/healthcare-analytics-cloud-foundation)**


### VitalSync Healthcare Interoperability Platform

**Business Problem:** How can clinical and operations teams maintain visibility over data movement, message delays, and integration failures across fragmented healthcare systems?

**What I Built:** A full-stack healthcare observability and dashboard platform simulating data flows across Hospital Information Systems (HIS), HL7 v2 messaging logs, and external FHIR R4 REST APIs. Designed a MySQL relational database separating transactional tables, event logs, and denormalized reporting summary tables for fast dashboard lookups. Built an MVC web interface (PHP, HTML/CSS) featuring role-based analytical views (Clinical, PM Oversight, Integration Health, Research Metrics) with dynamic KPI threshold indicators (Healthy, Warning, Critical).

**Skills Demonstrated:** Relational Database Design & SQL Querying · REST API Integration & Ingestion (FHIR R4) · Multi-Tier Data Modeling (Normalized vs. Denormalized) · Health Informatics (HL7 / FHIR Concepts) · Full-Stack Dashboard Engineering (MVC / PHP) · System Observability & SLA Threshold Monitoring

**Tech Stack:** PHP · MySQL · SQL · REST APIs (FHIR R4) · HL7 Simulation · JSON · HTML5/CSS3 · Figma

**Key Takeaways & Technical Insights:**
* **Multi-Tier Modeling & Reporting Abstraction:** Separated normalized transactional tables (HIS), structured audit logs (HL7 status/retries), and denormalized summary tables (`patient_sync_summary`) to keep analytical dashboard queries performant.
* **Hybrid Ingestion for Semi-Structured Data:** Ingested external FHIR R4 API data by retaining raw JSON payloads for traceability while extracting and materializing key observation metrics into SQL tables for trend analysis.
* **Built-in Governance & Observability:** Implemented schema validation tracking, retry monitoring, and threshold-based status indicators (Healthy, Warning, Critical) to surface interface latency and bottlenecks across operational domains.

→ **[View Project](https://github.com/alejandra-badia/vitalsync-interoperability-dashboard)** · **[Live Demo](https://vitalsync.smarterspec.tech/)**

## Education

* **Master’s in International Business**
* **B.S. in Chemical Engineering**

## Technical Training

* **Power BI**
* **Python for Machine Learning**
* **Full-Stack Web Development, SQL, APIs**

## Professional Background

11 years of technical project engineering and management in the oil & gas industry, a BS in Chemical Engineering, and a Master’s in International Business. My engineering foundation centers on process flows, root-cause diagnostics, and capital project delivery. Having managed complex technical scopes and cross-functional stakeholders, I approach analytics not as isolated charts, but as end-to-end business systems: translating operational requirements into structured data models, auditing metric integrity, and delivering decision-ready reporting

## Resume

→ **[View Resume](YOUR-RESUME-LINK)**

## Currently Developing

Healthcare Analytics & ML Engine
Python • Machine Learning • Healthcare Operations

## Connect

[LinkedIn](www.linkedin.com/in/alejandra-badia-544910371)
