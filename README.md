

# 🧠 **CompliSense AI – Next-Gen Advisory Support Platform**

### 🚀 Executive Summary

**CompliSense AI** is an intelligent compliance co-pilot for AIA Singapore’s financial advisory force.
It ensures that **every client recommendation is compliant, suitable, and justifiable**, while simultaneously improving **advisory consistency, turnaround time, and scalability**.

By embedding **GenAI-driven compliance and suitability checks** into the advisory workflow, CompliSense AI reduces regulatory risk, boosts agent productivity, and enhances customer confidence — all while enabling faster, more accurate financial advice delivery.

---

## ⚠️ Problem Statement

### 1. Inconsistent Advisory Quality & Compliance Risk

* Agents spend up to 20% of their time manually checking AIA’s **Financial Health Rules (FHR)**, **product suitability guidelines**, and **regulatory disclosures**.
* Free-text client notes and justifications are **unstructured and unreviewed**, increasing risk of omissions or misstatements.

### 2. Slow Turnaround & Poor Customer Experience

* Manual completeness checks and follow-ups delay the **quote-to-close cycle by 1–2 days**.
* Clients receive non-uniform recommendations, leading to **eroded trust and satisfaction**.

### 3. Scalability & Training Bottlenecks

* New agents require extensive one-on-one coaching on compliance and suitability, **slowing down distribution growth**.

---

## 💡 Proposed Solution

CompliSense AI introduces a **multi-layered AI orchestration** framework combining Natural Language Processing (NLP), Rule-Based Engines, and Knowledge Graphs to continuously validate financial advice against AIA’s standards.

### 1. **Automated Rule Compliance Analysis**

* Instantly detect deviations from **Financial Health Rules** and internal guidelines.
* Generate **explainable recommendations** for corrective actions using AI reasoning traces.
* Example: *“Income-to-premium ratio exceeds affordability threshold; consider product X instead of Y.”*

### 2. **Free-Text Compliance Intelligence**

* Parse agent-written justifications and client dialogues to check for:

  * Missing disclosures (e.g., risk tolerance not stated)
  * Misaligned rationale (“client is risk averse” vs “recommended high-risk equity product”)
  * Potential mis-selling patterns
* Auto-summarize client intent + advisor recommendation → compliance alignment score.

### 3. **Scorecard Lapse Detection**

* Continuously monitor gaps in **BSC (Balance Scorecard)** and trigger proactive compliance nudges.
* Examples: “Missing client signature,” “Incomplete fact-find form,” or “Product mismatch in FHR section.”

### 4. **Product Suitability & Affordability Validation**

* Cross-reference client profiles (income, dependents, risk appetite) with product rules and AIA guidelines.
* Suggest alternative product mixes if affordability or suitability mismatches are found.

---

## 🧩 Expanded Core Use Cases

| Use Case                                | Description                                                         | AI Capability                              |
| --------------------------------------- | ------------------------------------------------------------------- | ------------------------------------------ |
| **FHR Rule Compliance**                 | Analyze FHR data against Basic Financial Guide & Advisory Manual    | Rules engine + LLM for deviation summary   |
| **Free-Text Review**                    | Interpret advisory notes for reasonableness & justification quality | LLM with fine-tuned financial domain model |
| **Scorecard Lapse Detection**           | Identify missing compliance checkpoints                             | ML-based completeness predictor            |
| **Product Suitability & Affordability** | Match recommendations with client capacity                          | Hybrid rules + embedding similarity models |

---

## 🧠 Intelligent Features to Differentiate

### 🔹 1. **Compliance Graph Engine**

A dynamic **knowledge graph** linking:

* Client profile → financial health → recommended product → FHR rules → disclosures
  → This allows reasoning queries like:
  “Show me all high-risk recommendations given to clients above 60 years old”
  or
  “Which agents repeatedly violate affordability ratio rules?”

### 🔹 2. **Real-Time Compliance Copilot (Chat Mode)**

Agents can interact conversationally:

> “Check if my recommendation for Mr. Tan aligns with the FHR guidelines.”
> “Summarize missing disclosures for this proposal.”
> “What alternative low-risk plans fit a monthly income of $3,000?”

### 🔹 3. **Learning Feedback Loop**

Every compliance review result trains a **continual-learning engine** that adapts to regulatory updates or recurring agent mistakes — essentially, **“AI that learns AIA’s evolving compliance DNA.”**

### 🔹 4. **RegTech API Suite**

Expose APIs to integrate with existing systems:

* `/api/premium/calc` → Dynamic premium computation using product rule metadata
* `/api/doc/review` → Document validation & advisory note scoring
* `/api/compliance/check` → Real-time compliance validation for digital proposals

---

## ⚙️ Technical Architecture Overview

**Layers:**

1. **Data Layer**:
   Structured inputs (FHR, BSC, Client Profiles) + Unstructured text (Advisor notes)
   → stored in **Postgres + Azure Blob + Vector DB (e.g., Azure Cognitive Search / PostgreSQL+pgvector)**.

2. **AI Layer**:

   * Fine-tuned **LLM (Azure OpenAI / Gemini)** for compliance & financial language.
   * **Rule Engine** for deterministic validations (income ratio, product rules).
   * **Graph Engine** (Neo4j / NetworkX) for cross-entity relationship inference.

3. **Application Layer**:

   * Web dashboard for agents (compliance summary, alerts, recommendations).
   * Supervisor console with heatmaps for compliance risk scoring.
   * APIs integrated into AIA’s existing **LeadMate / iPoS ecosystem**.

---

## 📊 Example Outputs

| Scenario                                                   | AI Insight                                                                                     |
| ---------------------------------------------------------- | ---------------------------------------------------------------------------------------------- |
| Advisor recommends “Investment Linked Plan” to 62-year-old | ⚠️ *Risk mismatch: client age > 60. Suggest ‘WealthSecure Saver’ or similar low-risk options.* |
| Missing section in FHR notes                               | 🟡 *Disclosure gap detected: client’s emergency fund details not captured.*                    |
| Agent’s free-text justification                            | 🧠 *Detected inconsistent rationale between “risk averse” and “high premium allocation.”*      |

---

## 🌱 Impact Metrics

| Metric                         | Baseline      | Target       |
| ------------------------------ | ------------- | ------------ |
| Advisory review turnaround     | 2 days        | < 30 minutes |
| Manual compliance errors       | 100% (manual) | ↓ 80%        |
| Agent onboarding time          | 2 weeks       | ↓ 60%        |
| Distribution consistency index | 65%           | ↑ 90%        |

---

## 🔍 External Reference Sources

* [MoneySense Financial Planning Guide](https://www.moneysense.gov.sg/planning-your-finances-well)
* [Basic Financial Guide PDF](https://www.moneysense.gov.sg/files/streamlined%20basics%20financial%20planning%20guide.pdf)

---

Would you like me to **expand this into a PRD-style document** (with sections like Vision, Goals, Success Metrics, User Journeys, and Architecture Diagram)?
That would make it ready for submission to the AIA Innovation Council.
