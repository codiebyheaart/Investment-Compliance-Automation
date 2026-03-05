# Guideline IQ Demo Script: "Scale Personalisation with Real-Time Compliance"

*This is a ready-to-read script for your demo. Words in **bold** are actions you take on the screen.*

---

## 1. Introduction & The Problem (2 minutes)
**[Share screen showing Bodhi platform blank workflow or dashboard]**

"Hi everyone. Today I'm going to walk you through a solution for a major pain point in Wealth and Asset Management: **Scaling personalisation while maintaining real-time compliance.**

Asset managers want to offer highly tailored portfolios to clients. But every client has their own Investment Management Agreement (IMA) with unique rules—like 'no single issuer above 10%' or 'no emerging markets.' 

Historically, tracking a live portfolio against hundreds of pages of legal text means manual reviews, slow decisions, and high operational risk. 

Today we'll show you how Agentic AI solves this across three pillars:
1. Instant extraction of legal mandates
2. Continuous detection of real-time breaches
3. Automated escalation and personalised trade instructions

Let's run the workflow."

---

## 2. Running the Workflow & Pillar 1: Extraction (3 minutes)

**[Click Run and upload the sample IMA PDF]**

"I've just uploaded a 25-page IMA for a $2.5 Billion pension fund. 

While the workflow runs, let me explain what the first few nodes are doing. This covers our first pillar: **Instant extraction.**

- **The Document Nodes (PDF Chunker & Mapper):** These break down the legal PDF and identify all the critical sections—investment restrictions, ESG rules, liquidity limits.
- **Master Clause Extractor:** Instead of a human reading 25 pages, this AI agent reads the document and extracts every single enforceable rule into specific data points.
- **Conflict & Gap Detector:** This agent reads those rules and looks for contradictions. Often, older IMAs have conflicting clauses, or they miss modern regulatory requirements like MiFID II. It flags those immediately.

Instead of taking 3 days for a paralegal to map this out, Bodhi just did it in seconds."

---

## 3. Pillar 2: Real-Time Breach Detection (3 minutes)

**[Scroll to the middle of the workflow showing the Parallel Risk Processor and Breach Detector]**

"Now we move from theory to reality. This is our second pillar: **Continuous Detection.**

- **Parallel Risk Processor:** This splits the extracted rules into batches and runs 3 AI agents in parallel to score the risk of every single clause. It tags them with regulations like FCA or MiFID II and assigns a risk score.
- **Portfolio Snapshot:** In a real setup, this connects to your Order Management System (OMS). For this demo, it’s simulating live positions for the $2.5B fund—showing us exactly what stocks and bonds we hold today.

**[Highlight the Real-Time Breach Detector node]**

- **Real-Time Breach Detector:** This is the magic node. It takes the legal rules we just extracted, and cross-references them against the live portfolio snapshot. It’s asking: *'Based on what the PDF says we are allowed to do, are any of our actual stock positions in breach right now?'*"

---

## 4. Pillar 3: Automated Escalation & Personalisation (4 minutes)

**[Scroll to the end of the workflow and open the final Executive Summary or Dashboard]**

"And here are the final results. This covers our third pillar: **Escalation and Personalised Strategies.**

Because the Breach Detector found issues, the workflow automatically routed to the escalation path. Let's look at what the agents generated:

1. **Escalation Alert Generator:** It didn't just say 'we have a problem.' It built a 3-level escalation path. It notified the Portfolio Manager to act in 2 hours, the Chief Compliance Officer in 4 hours, and the CIO by end-of-day.
2. **Personalisation Engine:** It generated exact trade instructions to fix the breaches. For example, it found we hold 12% in Apple, but the mandate limit is 10%. It generated a specific instruction to *'Sell $50M of Apple'* to get us back into compliance. 
3. **Compliance Verification Agent:** A final check by an autonomous agent using compliance tools to ensure the report meets regulatory standards before sending it to humans.

---

## 5. Conclusion & Value Proposition (1 minute)

"To summarize: We went from a raw 25-page legal PDF to a live portfolio compliance check in under a minute. 

**What problem did we solve?**
We removed the bottleneck between legal documentation and trading execution. 

**How does this help the firm?**
- **Speed:** Portfolio Managers can make decisions instantly, knowing the AI is checking their trades against the specific client mandate.
- **Risk:** We eliminate human error in reading complex 50-page PDFs.
- **Scale:** You can offer highly personalised, bespoke portfolios to thousands of clients because compliance checking is now automated and real-time.

Are there any questions on the workflow or the specific agents used?"
