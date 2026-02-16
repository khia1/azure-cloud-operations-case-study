# Azure Cloud Operations Case Study

Azure cost governance and operational control simulation demonstrating budget enforcement, monitoring configuration, and resource lifecycle management in a controlled subscription environment.

---

## Project Summary

This project simulates a real-world cloud cost incident within an Azure subscription and demonstrates structured remediation using governance controls.

An unexpected cost spike was identified and resolved through:

- Azure Cost Analysis investigation
- Budget alert configuration
- Resource cleanup validation
- Lifecycle governance implementation

This repository showcases hands-on operational thinking rather than theoretical cloud knowledge.

---

## Scenario Overview

A virtual machine was provisioned and left running without cost controls in place, resulting in unexpected billing overage.

### Response Actions

- Investigated cost breakdown using Azure Cost Analysis
- Identified compute and managed disk charges
- Deleted unused resources
- Implemented CA$20 monthly budget
- Configured 50%, 80%, and 100% alert thresholds
- Verified billing stabilization

Full incident documentation is available in:

`docs/incident-report.md`

---

## Governance Implementation

To prevent recurrence, a structured governance model was introduced including:

- Budget-first deployment policy
- Resource lifecycle validation checklist
- Manual audit workflow
- Risk mitigation strategy

Detailed governance framework:

`docs/cost-governance-strategy.md`

---

## Skills Demonstrated

- Azure Cost Management
- Budget & Alert Configuration
- Resource Group Management
- VM Lifecycle Control
- Incident Documentation
- Operational Risk Analysis
- FinOps Fundamentals

---

## Why This Project Matters

Cloud cost control is one of the most overlooked operational risks in growing environments.

This project demonstrates practical cost governance thinking aligned with real-world cloud operations practices.

It reflects operational accountability, not just certification-level knowledge.
