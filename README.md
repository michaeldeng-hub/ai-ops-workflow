# AI Ops Workflow

Production automation and AI-assisted workflows for financial services operations. This repo documents end-to-end bots and pipelines I own that remove manual review, enforce compliance, and accelerate funding, processing thousands of transactions per month.

## Overview

I build and operate automation that sits across Salesforce, Dealertrack, and third-party vendor systems. The focus is reliability, auditability, and measurable operational lift, not one-off scripts. Each project below is deployed, documented, and maintained.

## Tech Stack

- **Languages:** Python
- **Automation:** Playwright, RPA scripting
- **Integrations:** Salesforce API, Dealertrack, LexisNexis
- **AI-assisted development:** Claude, Microsoft 365 Copilot
- **Architecture:** Consolidating individual automations into a unified MCP server for centralized orchestration and control

## Projects

### CSNS Compliance RPA
Automates a legal and compliance requirement to deliver each customer a PDF containing their credit score notice. Handles document generation and routing at high volume, removing manual effort and closing a compliance gap.
- **Impact:** Eliminates manual per-customer document handling across a large monthly volume.
- **Stack:** Python, Playwright, PDF generation.

### LexisNexis Fraud Detection Bot
Automates identity and fraud checks against LexisNexis, flagging risk signals before deals advance. Includes security hardening of the RPA scripts to protect credentials and sensitive data.
- **Impact:** Faster, consistent fraud screening with reduced manual review.
- **Stack:** Python, Playwright, LexisNexis integration.

### Funding Submission Bot
Automates identification and routing of funding submissions to reduce manual review effort and accelerate funding time. The bot speeds processing, not credit decisions.
- **Impact:** Shorter funding cycle time and less manual routing.
- **Stack:** Python, Salesforce API, Dealertrack.

### MCP Consolidation
Splices multiple standalone automations into a single MCP server for more robust, centralized workflow control and easier monitoring.
- **Status:** In progress.
- **Goal:** One orchestration layer for all bots.

## Impact Summary

| Area | Result |
|------|--------|
| Compliance | Automated credit score notice delivery at scale |
| Fraud | Automated LexisNexis screening with hardened scripts |
| Funding | Reduced manual review and faster funding time |
| Volume | Thousands of transactions automated per month |

## Notes

These automations run against regulated financial data. Credentials and PII are handled through secured configuration and are never committed to this repository.
