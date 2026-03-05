# Guideline IQ Demo Script: "Scale Personalisation with Real-Time Compliance"

*This is a ready-to-read script for your demo. Words in **bold** are actions you take on the screen.*

---

## 1. Introduction & The Problem (2 minutes)
**[Share screen showing Bodhi platform blank workflow or dashboard]**

"Hi everyone. Today I'm going to walk you through a solution for a major pain point in Asset and Wealth Management: **Scaling personalisation with real-time compliance.**

Asset managers want to deliver highly tailored portfolios to their clients. But every client has a complex mandate—specific rules like 'no single issuer above 10%' or 'never hold emerging markets.' 

Historically, tracking a live portfolio against hundreds of pages of legal text means manual reviews, slow decisions, and high operational risk. 

Today we'll show you how Agentic AI solves this across three pillars:
1. Instant extraction of mandates and policy constraints
2. Continuous detection of risk, breaches, and inconsistencies
3. Portfolio-wide adherence monitoring with clear escalation paths

Let's run the workflow."

---

## 2. Running the Workflow & Pillar 1: Extraction (3 minutes)

**[Click Run and upload the sample IMA PDF]**

"I've just uploaded a 25-page Investment Management Agreement (IMA) for a $2.5 Billion pension fund. 

While the workflow runs, let me explain what the first few nodes are doing. This covers our first pillar: **Instant extraction.**

- **The Document Nodes:** These break down the legal PDF and identify all the critical sections automatically.
- **Master Clause Extractor:** Instead of a human reading 25 pages, this AI agent extracts every single enforceable rule into specific data points.
- **Conflict & Gap Detector:** This agent reads those rules and looks for contradictions or missing regulatory coverage, like MiFID II requirements.

Instead of taking 3 days for a paralegal to map this out, Bodhi just did it in seconds."

---

## 3. Pillar 2: Real-Time Breach Detection (3 minutes)

**[Scroll to the middle of the workflow showing the Parallel Risk Processor and Breach Detector]**

"Now we move from theory to reality. This is our second pillar: **Continuous Detection.**

- **Parallel Risk Processor:** This splits the extracted rules into batches and runs 3 AI agents in parallel to score the risk of every single clause. 
- **Portfolio Snapshot:** In a real setup, this connects to the firm's Order Management System (OMS). For this demo, it’s simulating live positions for the $2.5B fund—showing us exactly what stocks and bonds we hold today.

**[Highlight the Real-Time Breach Detector node]**

- **Real-Time Breach Detector:** This is the magic node. It takes the legal rules we just extracted, and cross-references them against the live portfolio snapshot. It’s analyzing: *'Based on what the PDF says we are allowed to do, are any of our actual stock positions in breach right now?'*"

---

## 4. Pillar 3: Automated Escalation & Personalisation (4 minutes)

**[Scroll to the end of the workflow and open the final Executive Summary or Dashboard]**

"And here are the final results. This covers our third pillar: **Escalation and Portfolio Monitoring.**

Because the Breach Detector found issues, the workflow automatically routed to the escalation path. Let's look at what the agents generated:

- **Escalation Alert Generator:** It didn't just say 'we have a problem.' It built a clear escalation path. It notified the Portfolio Manager to act in 2 hours, the Chief Compliance Officer in 4 hours, and the CIO by end-of-day.
- **Personalisation Engine:** It generated exact trade instructions to fix the breaches. For example, it found we hold 12% in Apple, but the mandate limit is 10%. It generated a specific instruction to *'Sell $50M of Apple'* to get us back into compliance. 
- **Compliance Verification Agent:** A final check by an autonomous agent using compliance tools to ensure the report meets regulatory standards before sending it to humans.

---

## 5. Conclusion & Value Proposition (1 minute)

"To summarize: We went from a raw 25-page legal PDF to a live portfolio compliance check in under a minute without slowing down portfolio decisions.

**What did we achieve?**
We standardised and automated compliance at scale. We orchestrated AI agents across mandates, portfolios, and market data.

**How does this help the firm?**
- **Speed:** Portfolio Managers can make decisions instantly with real-time compliance checks.
- **Risk:** We significantly reduce operational risk by eliminating manual PDF reviews.
- **Scale:** You deliver highly tailored investment strategies to thousands of clients because compliance checking is now automated and real-time.

Are there any questions on the workflow?"

---

## Node Cheat Sheet (For Q&A)

*If anyone asks "What exactly does this specific node do?", use these simple 1-sentence answers:*

**Input & Extraction Nodes:**
## 1. **Client Intake Form (trigger):** Where the user uploads the IMA PDF to start the process.

## 2. **Enterprise PDF Chunker:** Splits the large PDF into smaller, readable pieces for the AI.

##3. **DocType Classifier:** Quickly identifies if the document is an IMA, Prospectus, or ISDA.

##4. **Metadata Extractor:** Pulls out basic info like "Client Name", "Date", and "Jurisdiction".
## 5. **IMA Section Mapper:** Maps out the document structure (where the ESG rules vs. Liquidity rules are).

##6. **Master Clause Extractor:** Pulls out the exact legal rules (e.g., "No single stock over 10%").

##7. **Conflict & Gap Detector:** Finds contradictory rules or missing regulatory language inside the IMA.

**Analysis & Risk Nodes:**
## 8. **Parallel Risk Processor (Repeat):** A container that runs 3 agents at the same time to speed up processing.

## 9. **Batch Risk Analyser:** Scores the risk (High/Medium/Low) for a small batch of clauses.
## 10. **Risk Results Collector:** Cleans and compresses the data so the next AI node doesn't get overloaded.

##11. **Risk Aggregator:** Merges the 3 parallel batches back into one central risk report.
 ##12. **Regulatory Cross-Reference:** Tags each risk with the exact law it relates to (like FCA or MiFID II).

**The Demo Core Nodes:**
## 13. **Portfolio Snapshot Builder:** Simulates our $2.5B portfolio with live stock and bond positions.
## 14. **Real-Time Breach Detector:** Compares the live portfolio against the IMA rules to find immediate violations.

## 15. **Breach Status Classifier:** Looks at the detector's output and shouts a clear "BREACH" or "CLEAN".

## 16. **Breach Decision Router (Switch):** Automatically sends the workflow down the Red path (Escalation) or Green path (Clean Report).

**Output & Action Nodes:**
## 17. **Escalation Alert Generator:** Creates the notification path (PM → Head of Compliance → CIO) with deadlines.

## 18. **Personalisation Engine:** Generates the exact trades needed to fix the portfolio (e.g., "Sell $50M Apple").

## 19. **No-Action Compliance Report:** Generates a Clean bill of health if no breaches were found.

## 20. **Bodhi Compliance MCP:** Gives the AI secure access to external compliance databases or tools.

## 21. **Compliance Verification Agent:** A smart agent that double-checks the final report for quality and accuracy.

## 22. **Rule Engine Coder:** Translates the English IMA rules into actual computer code for automated daily checking.

## 23. **Executive Summary Generator:** Writes the final, board-ready report we see at the end.

## 24. **UI_JSON_Builder:** Formats all the data nicely for the final visual dashboard.

## 25. **Preview Node:** Displays the final visual dashboard to the user.
