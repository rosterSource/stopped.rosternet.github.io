---
layout: page
title: Roster Net
---

The quality of physician demographics and which insurance plans they accept remains a challenge across the healthcare ecosystem. Even answering a simple question like “is a particular provider accepting new patients?” is not easy to answer.

No single stakeholder or institution can solve this problem alone. The RosterNet community was created to pull all participants into a single open source community so that resources--senior infrastructure and system architects with the skills needed to manage secure provider roster data--can be shared across institutions. 

# PaaS

Specific to each Data Source, there should be a Data Harvesting Agent which pulls data from the source and provide to the Respective RosterNet Aggregator Agents.
For Example, the NPPES CSV Data Harvesting Agent flow below watches a folder for NPPES CSV files, Read the file and provide the data as JSON.
Based on the Data and Data Source, we will need to create as many Data Harvesting Agents as possible.

# Data Source

Phase 1 : NPPES CSV Data(Available for Download) and Data from NPPES API calls will be the first Data Source for RosterNet. 

Phase 2 and future Phases : Integration to 3rd Party EHR. 

# Add RosterNet features

The RosterNet Platform as a Service (PaaS) gives health systems and health insurers alike the freedom of keeping their data in their own line of business systems but share it in near-real-time with their close partners or the broader ecosystem, including government entities. 

Significant cost savings are achieved through federated roster management shared services and open source software. You’re no longer alone.
