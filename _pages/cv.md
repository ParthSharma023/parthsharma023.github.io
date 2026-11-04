---
layout: archive
title: "CV"
permalink: /cv/
author_profile: true
redirect_from:
  - /resume
---

{% include base_path %}

Experience
======
* **Software Team Lead, Ardurra** - Houston, TX - Jan 2026 to present
  * Lead software delivery for internal teams and municipal clients, including the City of Houston's water utilities; hands-on in architecture and implementation.
  * Embedded with the City of Houston's water utilities: shipped 40 operational dashboards in five months, replacing vendor Power BI with self-hosted HTML/JS apps backed by Python, DuckDB, and Parquet pipelines on S3.
  * Reverse-engineered a 104-page, 12.5-million-row Power BI compliance model (5.5 GB of exports) into a DuckDB/Parquet pipeline (196 MB) powering a 58-page static web app, and validated the migration plant-by-plant against 12,000+ regulatory violation counts.
  * Consolidated three vendors' sensor BI platforms (about 72 tables across three semantic models) into a single canonical data model with automated, lock-protected incremental publishing.

* **Founder & Lead Engineer, Basil Health** - 2025 to present
  * Built and operate a clinical reporting platform that turns DEXA body-composition scans into personalized patient reports: in production at three paying clinics, 300 patients processed.
  * Sole engineer across the stack: reverse-engineered the scanner's Access database, wrote the Postgres ingestion pipeline, and ship guardrailed LLM-generated reports; re-platforming onto FHIR/Medplum with byte-parity tests between the Python and TypeScript insight engines.
  * Shipped a full-stack patient portal verified by 58 API tests and 19 Playwright end-to-end specs.

* **Researcher, The Robotic Global Surgical Society (TROGSS)** - Sep 2026 to present
  * AI engineering lead on a study of video models that detect robotic suturing errors across surgical platforms (in development).

* **Software Engineer, Ardurra** - Houston, TX - Mar 2024 to Dec 2025
  * Led a two-engineer team delivering about 10 access-controlled RAG deployments (Azure OpenAI, AI Search, CosmosDB, Bicep IaC) for internal departments and external clients - adding multi-tenancy, MSAL auth, usage telemetry, and CI/CD on top of Microsoft's open-source azure-search-openai-demo base.
  * Delivered a crash-countermeasure benefit-cost tool over 9,777 FHWA studies across three platforms: a web app, a Power BI report, and a Tableau dashboard with a custom Extensions-API widget.
  * Built the cloud side of a patent-pending IoT condition-monitoring system for stormwater trash interceptors: Azure IoT Hub ingestion, time-series data model, threshold alerting, and monitoring dashboard.

Selected projects
======
* **[Daycase](/portfolio/daycase/)** - charting software for same-day surgery: scheduling, role-based patient charts, and case close-out. 29 clinical forms (about 500 questions), with clinical rules enforced on the server. TypeScript, React, Fastify, SQLite. Synthetic patients only.

Education
======
* B.S. in Computer Science, University of Miami, December 2023

Patent
======
* Named inventor, "Systems and Methods for IoT Sewer Management" - a load-cell system for condition-based maintenance of stormwater trash interception devices. Non-provisional application filed by Ardurra; patent pending.

Publications
======
  <ul>{% for post in site.publications reversed %}
    {% include archive-single-cv.html %}
  {% endfor %}</ul>

Skills
======
* **Languages and frameworks:** Python (pandas, FastAPI, SQLAlchemy), TypeScript/JavaScript (React, Vite), SQL (Postgres, DuckDB), HTML/CSS to production polish
* **Data engineering:** Parquet/S3 pipelines with incremental refresh, BI reverse-engineering (PBIX, TMDL, DAX), cross-vendor schema consolidation, migration validation and reconciliation
* **AI engineering:** guardrailed LLM pipelines in production (Claude API), RAG on Azure OpenAI + AI Search, agent tooling (custom skills, automated audits) - orchestration and product engineering, not model training
* **Platform and domain:** Azure (Static Web Apps, IoT Hub, Bicep, CI/CD), FHIR/Medplum and HIPAA-aware design, GIS (Leaflet, shapely), Docker, GitHub Actions
