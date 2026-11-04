---
title: "DatArdurra - AI document search for engineering teams"
excerpt: "Ten access-controlled RAG deployments on Azure OpenAI for Ardurra departments and clients, so teams can ask questions of their regulatory and technical documents."
collection: portfolio
order: 5
redirect_from:
  - /portfolio/05-datardurra/
group: Infrastructure
---

DatArdurra lets engineers ask plain-language questions of their own documents - state environmental regulations, flood-control design manuals, HR policies - and get answers linked back to the source.

I led a team of two that took Microsoft's open-source [azure-search-openai-demo](https://github.com/Azure-Samples/azure-search-openai-demo) and turned it into a platform: ten branded deployments for internal departments and external clients, each with its own document index and Microsoft sign-in. What we added was multi-tenancy, authentication, CI/CD for each deployment, and a usage dashboard built from scratch, so each department can see how its deployment is actually being used.

**Stack:** Azure OpenAI, Azure AI Search, Cosmos DB, Document Intelligence, Bicep, Python (Quart), React + TypeScript.

*Client work; the code is private.*
