# ai-ops-workflow
Compliance, Funding and Fraud RPA workflow
AI Operations Portfolio — Michael Deng

AI-powered workflow automation systems designed and deployed in production at Lucid Motors.

## Overview

This repository showcases production automation systems I designed, built, and deployed across Finance Operations, Risk & Compliance, and Funding Operations at Lucid Motors.

Each workflow was developed end-to-end using Python + Playwright with AI-assisted development workflows using Claude and VS Code. These systems currently process thousands of compliance-critical transactions monthly with measurable operational impact.

I owned the full lifecycle for each system:
- Problem identification
- Workflow mapping
- Automation design
- AI-assisted development
- Production deployment
- Monitoring & support

---

# Key Outcomes

- Reduced onboarding and financing decision turnaround from days to seconds
- Eliminated 230+ manual operational hours per month
- Processed 5,000+ transactions monthly
- Maintained zero compliance errors across 18+ months in production
- Built scalable workflows adopted across multiple teams

---

# Featured Systems

## 1. Compliance Automation Bot (“CSN Bot”)

### Problem
Manual processing of 4,000+ monthly credit score disclosure notices required repetitive workflows across Salesforce and Dealertrack, consuming 65–70+ hours weekly with ongoing compliance risk.

### Solution
Built a Python + Playwright automation workflow that:
- Pulled customer credit bureau reports
- Generated compliance disclosures automatically
- Attached PDFs to Salesforce
- Triggered templated customer communications
- Logged operational status updates

### Impact
- 4,000+ monthly transactions automated
- 100% accuracy maintained
- Zero compliance failures
- ~200+ manual hours eliminated monthly

### Stack
Python · Playwright · Salesforce API · Headless Chromium · Claude · VS Code

---

## 2. Fraud Detection Automation

### Problem
Risk & Compliance teams required scalable fraud screening and identity verification with full audit readiness.

### Solution
Built automated workflows integrating:
- LexisNexis InstantID
- LexisNexis Emailage
- SharePoint audit logging
- Salesforce workflow routing

### Impact
- 100% automated coverage of flagged applications
- Eliminated manual identity verification bottlenecks
- Created full audit-ready reporting infrastructure

### Stack
Python · Playwright · LexisNexis APIs · SharePoint · Salesforce · Claude

---

## 3. Automated Funding Submission Bot

### Problem
Post-delivery funding package submission required repetitive multi-system workflows taking ~12 minutes per transaction.

### Solution
Developed an event-driven automation system triggered by Salesforce delivery status changes that:
- Pulled funding documentation automatically
- Uploaded documents to Dealertrack
- Submitted completed lender funding packages
- Updated Salesforce workflow statuses

### Impact
- Reduced submission time from ~12 minutes → ~90 seconds
- Reduced weekly operational workload from 30+ hours → under 3
- Near-zero operational error rate

### Stack
Python · Playwright · Salesforce API · Dealertrack · Claude

---

# How I Use AI

I use AI as an execution and acceleration layer within operational system design.

Primary workflows include:
- Prompt engineering
- Code scaffolding
- Debugging & iteration
- Workflow logic generation
- Rapid prototyping

Tools used:
- Claude
- VS Code

Rather than treating AI as a standalone product, I focus on applying it to real operational bottlenecks and transforming repetitive workflows into scalable systems.

---

# About Me

I’m an operations and systems builder with a background in finance operations and strategy. My focus is designing scalable workflows that improve operational leverage, reduce friction, and accelerate execution.

I specialize in:
- Automation
- Systems thinking
- Cross-functional execution
- AI-assisted workflow design
- Product-adjacent operations

LinkedIn: linkedin.com/in/mhdeng
