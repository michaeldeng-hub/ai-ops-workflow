# ai-ops-workflow
Compliance, Funding and Fraud RPA workflow

This portfolio showcases three production AI-powered automation systems I designed, built, and deployed at Lucid Motors
(Sep 2022 – Present). 
Each workflow runs in production daily, processing thousands of compliance-critical transactions 
monthly with measurable business impact. All systems were built end-to-end using Python + Playwright with AI-assisted
development (Claude Opus 4.7 + VS Code) and deployed org-wide via one-line push. I own the full lifecycle: problem identification ®
system design ® production deployment ® monitoring ® on-call.
ARTIFACT 1: COMPLIANCE AUTOMATION BOT (CSN Bot)
Problem
Financial Services Ops manually processed 4,000+ credit score disclosure notices per month. Each required 8 discrete steps
across 3 systems (Salesforce ® Dealertrack ® customer email), taking ~4.3 minutes per transaction. At scale, this consumed
65–70+ hours/week of specialist time with constant risk of compliance errors on federally mandated disclosures.
Solution
End-to-end Python + Playwright headless browser automation deployed org-wide via one-line push:
SFDC Report (filtered queue)
® Open Delivery Object ® Match state to dealership
® Navigate to Dealertrack Unifi Portal
® Enter Credit Bureau module ® Pull Experian report
® Enter Compliance module ® Generate Risk-Based Pricing Notice
® Save PDF locally as 'Credit Score Notice'
® Return to SFDC ® Open Finance Object ® Attach PDF
® Send templated email to customer on file
® Tag #CSNS in Sales Memo field 3
Stood up standardized VS Code environments for 3 teammates and 2 adjacent teams (Risk & Compliance, Lease Funding).
Provided hands-on coaching for cross-functional RPA adoption.
Impact
Transactions Processed 4,000+/month at 100% accuracy
Manual Hours Eliminated 200+ hours/month (~$60K+ annual cost savings)
Compliance Errors Zero in 18+ months of production
Peak Volume 4,287 transactions in a single month, single bot instance
Scale 1 operator ® 5 users across 3 teams
Tech Stack: Python · Playwright · Headless Chromium · Salesforce API · Claude (code generation + iteration) · VS Code
ARTIFACT 2: FRAUD DETECTION BOT (LexisNexis InstantID + Emailage)
Problem
Risk & Compliance needed automated identity verification and fraud risk scoring on every financing application. Manual checks
were inconsistent, unscalable, and created audit gaps. The Global Head of Risk & Compliance required a solution with configurable
scan frequency, one-click ad-hoc capability, and a full audit trail for regulatory examination.
Solution
Python + Playwright bot integrating two LexisNexis risk intelligence APIs, designed in collaboration with Risk & Compliance
leadership:
Michael Deng | hdeng1202@gmail.com | linkedin.com/in/mhdeng | AI Operations Portfolio
Salesforce (flagged applications queue)
® LexisNexis InstantID API ® Identity verification score
® LexisNexis Emailage API ® Email/phone fraud risk score
® Pass/Fail determination (configurable thresholds)
® Output file ® SharePoint folder (audit-ready)
® 100% of FAILS ® routed to manual R&C; case review
® PASSES ® sampled for QA (volume-dependent)
Features: Configurable scan frequency (batch or continuous)
One-click ad-hoc scan for manual spot checks
Full SharePoint audit trail for regulatory readiness
Impact
Coverage 100% of flagged transactions processed automatically
Bottleneck Removed Eliminated manual identity verification for R&C;
Audit Readiness Full trail stored in SharePoint from day one
Scalability Enabled fraud screening to scale without headcount
Follow-on Scoped FICO score automation as next initiative with R&C;
Tech Stack: Python · Playwright · LexisNexis InstantID API · LexisNexis Emailage API · SharePoint · Salesforce · Claude (development
acceleration)
ARTIFACT 3: AUTOMATED FUNDING SUBMISSION BOT (S4F)
Problem
After vehicle delivery, specialists manually assembled funding packages (invoice, title application, delivery acceptance,
stipulations) across Salesforce and Dealertrack, then submitted to lender. Each submission required 15+ clicks across 2 systems,
taking ~12 minutes per deal. At 600+ monthly deliveries, this consumed 28–32 hours/week.
Solution
Event-driven Python + Playwright bot triggered by Salesforce delivery status change:
Salesforce Delivery Status = "Confirmed for Delivery"
® Bot triggers automatically
® Pulls funding docs from SFDC (invoice, title app, stips)
® Navigates to Dealertrack Contract tab
® Uploads each document with correct doc type mapping
® Selects all documents ® Submits to lender
® SFDC stage updated to "Funding Pending w/ Lender" 3
Impact: Before ® After
Metric Before After
Time per submission ~12 minutes ~90 seconds
Weekly hours consumed 28–32 hours Under 3 hours
Automation rate 0% ~90%
Error rate Manual entry errors Near-zero
EOQ handling Bottleneck at quarter-end Scaled seamlessly
Tech Stack: Python · Playwright · Salesforce API · Dealertrack API · Claude (code scaffolding + iteration)
Michael Deng | hdeng1202@gmail.com | linkedin.com/in/mhdeng | AI Operations Portfolio
All three systems are live in production. Combined, they process 5,000+ transactions/month, save 230+ manual
hours/month, and have maintained zero compliance errors across 18+ months. Each was designed, built, and deployed
end-to-end by me — from problem identification through production monitoring and on-call support.
