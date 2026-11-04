---
title: "Basil Health - clinical reporting for DEXA scans"
excerpt: "Turns DEXA body-composition scans into personalized clinical reports and a longitudinal patient record. In production at three paying clinics; 300 patients processed."
collection: portfolio
order: 1
redirect_from:
  - /portfolio/01-basil-health/
group: Healthcare
---

Basil turns DEXA body-composition scans into personalized clinical reports and a longitudinal patient record. It's in production at three paying clinics, with 300 patients processed. Clinics invest six figures in a DEXA scanner, but patients usually leave with a printout they never read.

I built the whole path: reverse-engineered the scanner's Access database, wrote the Postgres ingestion pipeline, and ship LLM-generated reports with deterministic clinical guardrails. A tested full-stack patient portal (58 API tests, 19 Playwright end-to-end specs) is frozen as the spec while I re-platform onto a FHIR-native stack (self-hosted Medplum), with byte-parity tests keeping the Python and TypeScript insight engines clinically identical.

The work behind it is also a study: I'm first author on "From DEXA Data to Patient Action: AI-Assisted Body Composition Reporting in Bariatric Care," which I presented at the 7th International Bariatric Club World Congress, University of Oxford, in September 2026 ([details](/portfolio/#research)).

**Stack:** Python, Postgres, FastAPI, React + TypeScript, FHIR/Medplum, Claude API, Playwright, Docker.

*In production. Code is private - it handles patient data.*
