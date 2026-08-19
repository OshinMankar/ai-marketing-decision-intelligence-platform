# MarketLens — Marketing Decision Intelligence Platform

> **From campaign data to actionable marketing decisions.**

MarketLens is an **AI-powered Marketing Decision Intelligence Platform** designed to help marketing teams move from **campaign data → performance understanding → AI diagnosis → recommendations → decision → reporting** within a single workflow.

The project explores how centralized analytics, AI-assisted analysis, and structured decision support can reduce the manual effort involved in campaign performance monitoring and help marketing teams make faster, evidence-backed decisions.

---

## 🎯 Product Vision

Marketing teams have access to large volumes of campaign data, but turning that data into a decision often requires several manual steps:

**Collect data → Consolidate spreadsheets → Calculate KPIs → Analyze performance → Identify problems → Determine actions → Prepare reports**

MarketLens redesigns this workflow around a centralized decision-support experience:

**Data → Analysis → Diagnosis → Recommendation → Decision → Reporting**

The goal is not simply to provide another marketing dashboard, but to reduce the gap between:

> **“What happened?” → “Why did it happen?” → “What should we do next?”**

This decision-first approach is the core product concept documented across the business requirements, functional specification, process design, and UX work.

---

## 💡 Business Problem

Digital marketing teams increasingly manage campaigns across platforms such as Google Ads, Meta Ads, LinkedIn Ads, and other analytics tools.

As campaign volumes increase, marketing teams can face:

* Fragmented campaign data across multiple platforms
* Manual data consolidation
* Repetitive KPI calculations
* Time-consuming campaign analysis
* Delayed performance insights
* Inconsistent reporting
* Heavy dependence on analyst expertise
* Reactive rather than evidence-backed optimization decisions

The BRD identifies these challenges as the primary business need for a centralized marketing intelligence solution.

### The opportunity

Instead of requiring analysts to manually move between spreadsheets, dashboards, reporting tools, and separate AI tools, MarketLens brings the core decision workflow into one platform.

---

# 🚀 Proposed Solution

MarketLens provides a centralized environment where users can:

1. Upload campaign performance data
2. Validate the dataset
3. Monitor standardized marketing KPIs
4. Investigate campaign performance
5. Ask questions using natural language
6. Receive AI-assisted insights and diagnosis
7. Review prioritized recommendations
8. Make the business decision
9. Generate an executive-ready report

The future-state process design represents this transformation from fragmented, manual analysis to a centralized AI-assisted decision-support workflow.

---

# 🔄 Core Decision Workflow

```text
Campaign Data
      ↓
Data Validation
      ↓
Performance Analysis
      ↓
AI Diagnosis
      ↓
Insights / Risks / Opportunities
      ↓
Recommendations
      ↓
Human Decision
      ↓
Reporting
```

The product deliberately keeps the **human decision-maker in the loop**.

AI provides analysis, evidence, and recommendations; it does not automatically change campaign settings. This is an explicit business rule in the requirements.

---

# 🧩 Product Modules

MarketLens is organized around five primary user-facing modules, supported by authentication.

| Module               | Purpose                                                 |
| -------------------- | ------------------------------------------------------- |
| **Dashboard**        | Portfolio-level campaign performance overview           |
| **Campaigns / Data** | Upload, validate, preview, and manage campaign datasets |
| **AI Intelligence**  | AI-powered analysis and conversational exploration      |
| **Recommendations**  | Prioritized, evidence-backed optimization suggestions   |
| **Reports**          | Generate and export decision-ready performance reports  |

The Product Feature Map defines the same five-module structure and connects them through the core workflow of **Data → Performance → Intelligence → Recommendation → Decision → Report**.

---

# 📊 Dashboard

The Dashboard acts as the central workspace for understanding campaign performance.

### Key capabilities

* Spend
* Revenue
* ROAS
* Conversions
* Impressions
* Clicks
* CTR
* CPC
* Conversion Rate
* Performance trends
* Campaign performance table
* Date filters
* Campaign filters
* AI-generated performance insights
* Attention indicators

The UX specification defines the Dashboard around the principle of showing the most important information first, allowing users to understand whether performance is improving or declining without navigating through multiple pages.

---

# 📁 Campaigns / Data

The quality of AI analysis depends on the quality of the underlying campaign data.

The Campaigns / Data module therefore provides:

* CSV / Excel upload
* Dataset validation
* Required-field detection
* Missing / invalid data identification
* Data preview
* Data-quality warnings
* Dataset history
* Active dataset management
* Dataset replacement / re-upload

For the MVP, MarketLens uses a controlled dataset-based workflow rather than live advertising-platform integrations.

### Data flow

```text
Upload Dataset
      ↓
File Validation
      ↓
Data Preview
      ↓
Validation Successful?
      ↓
Analytics Dashboard
```

This ensures that users do not blindly rely on AI-generated insights from incomplete or invalid data.

---

# 🤖 AI Intelligence

The AI Intelligence module is designed to help users investigate campaign performance using natural language.

### Core capabilities

* Automated campaign analysis
* Performance anomaly identification
* Natural-language questions
* Campaign comparison
* KPI explanation
* Trend interpretation
* Performance diagnosis
* Root-cause analysis
* Contextual follow-up questions

Example questions include:

> “Why is Competitor Conquest underperforming?”

> “Which campaign should receive more budget?”

> “Compare Meta and Google performance.”

The UX design specifically emphasizes that AI should **explain the data rather than simply provide an answer**.

---

# 💡 Recommendations

The Recommendations module converts analysis into potential business actions.

Each recommendation is designed to provide:

* Priority
* Recommendation
* Associated campaign
* Supporting KPIs
* Analysis / rationale
* Expected impact
* Recommendation status

Users can:

* Mark a recommendation as complete
* Mark it for review
* Dismiss it

The product requirements also establish that recommendations should provide supporting evidence where sufficient data is available and should remain decision-support information rather than automatically modifying campaign settings.

---

# 📄 Reports

The Reports module converts the analysis into a decision-ready business output.

### Report capabilities

* Reporting period selection
* Campaign selection
* Report configuration
* Executive summary
* KPI summary
* Campaign performance
* AI insights
* Recommendations summary
* PDF export

The UX design defines the report as a **decision-ready output rather than simply a data dump**.

---

# 👥 Target Users

MarketLens is designed for stakeholders involved in marketing performance monitoring and decision-making.

| User                              | Primary Need                                                      |
| --------------------------------- | ----------------------------------------------------------------- |
| **Marketing Analyst**             | Upload data, analyze KPIs, identify trends, and generate insights |
| **Performance Marketing Manager** | Monitor campaigns and evaluate optimization opportunities         |
| **Marketing Director**            | Review overall performance and strategic insights                 |
| **CMO / Executive**               | Access summarized performance information and executive reports   |

For the MVP, the primary user is the **Marketing Analyst / Performance Marketing Manager**, because these users interact most directly with campaign data and optimization workflows.

---

# 🏗️ MVP Scope

The MVP is intentionally focused on demonstrating the complete decision-support workflow.

### Included in MVP

* User login
* CSV / Excel campaign data upload
* Data validation
* KPI dashboard
* Interactive campaign analysis
* AI-generated insights
* AI assistant
* Optimization recommendations
* Executive report generation
* PDF reporting

The Product Functional Specification defines the MVP around a controlled, dataset-based workflow.

### MVP completion flow

```text
Upload
   ↓
Validate
   ↓
Analyze
   ↓
Ask AI
   ↓
Get Recommendations
   ↓
Generate Report
   ↓
Export PDF
```

The MVP is considered functionally complete when the core workflow can be demonstrated end-to-end and the required acceptance criteria are satisfied.

---

# 🗺️ Product Roadmap

The current MVP intentionally excludes several advanced capabilities so that the core decision workflow can be demonstrated first.

### Future Enhancements

| Area                 | Future Capability                                                            |
| -------------------- | ---------------------------------------------------------------------------- |
| **Data Integration** | Live Google Ads, Meta Ads, LinkedIn Ads and other platform integrations      |
| **Analytics**        | Advanced drill-downs, cross-channel comparison, custom dashboards            |
| **AI Intelligence**  | Forecasting, anomaly detection, automated alerts, deeper root-cause analysis |
| **Recommendations**  | Automated budget optimization and personalized optimization strategies       |
| **Reporting**        | Scheduled reports, email delivery, customizable templates                    |
| **Automation**       | Automated campaign monitoring and workflow triggers                          |
| **User Management**  | Role-based access, teams, organizations and advanced permissions             |
| **Scalability**      | Multi-client / multi-organization support                                    |

These capabilities form part of the future product roadmap rather than the current MVP commitment.

---

# 🎨 UX & Product Design

The UX is designed around a simple principle:

> **Reduce the time between seeing a marketing problem and deciding what to do about it.**

The interface follows the progressive workflow:

```text
Overview
   ↓
Investigate
   ↓
Understand
   ↓
Act
   ↓
Report
```

The five core product experiences are:

1. **Dashboard**
2. **Campaigns / Data**
3. **AI Intelligence**
4. **Recommendations**
5. **Reports**

The wireframe documentation defines these screens and connects them into one continuous decision-making experience.

### UX Design Principles

* **Decision-first** — prioritize information that supports decisions
* **Explainable AI** — show the metrics and reasoning behind insights
* **Progressive disclosure** — show high-level information first
* **Actionability** — connect insights to recommendations
* **Data transparency** — make dataset quality visible
* **Consistency** — maintain consistent interaction and visual patterns

---

# 🔗 Product & Business Analysis Documentation

This project was developed as a structured Business Analysis and Product Design case study.

| Document                             | Description                                                                                  |
| ------------------------------------ | -------------------------------------------------------------------------------------------- |
| **Project Charter**                  | Project context, business background, objectives, scope, assumptions and risks               |
| **Business Requirements Document**   | Business needs, stakeholders, requirements, business rules, success metrics and traceability |
| **TO-BE Process Design**             | Current-state vs future-state workflow and AI intervention points                            |
| **Product Functional Specification** | Product behavior, functional requirements, MVP scope, dependencies and acceptance criteria   |
| **Product Feature Map**              | Product modules, feature hierarchy, prioritization and dependencies                          |
| **Wireframes & UX Design**           | Information architecture, user flow, screens, UX principles and responsive design            |


The documentation set is intentionally structured as a progression from **business discovery and requirements → process redesign → functional definition → feature prioritization → UX design**. The BRD also establishes traceability between business requirements, functional requirements, TO-BE processes, wireframes, and MVP modules.

---

# 🎨 Interactive Prototype

### Figma Prototype

**[View Interactive Prototype](https://rush-flick-23474810.figma.site/)**

The prototype demonstrates the core user experience across the primary product workflow.

---

# 🖥️ Product Screens

### Dashboard

Central workspace for monitoring campaign performance, KPIs, trends, and AI-identified areas requiring attention.

### Campaigns / Data

Upload, validate, preview, and manage the campaign dataset powering the analysis.

### AI Intelligence

Investigate campaign performance through conversational AI and evidence-backed analysis.

### Recommendations

Review prioritized optimization opportunities with supporting KPIs, rationale, and expected impact.

### Reports

Generate a structured performance report containing KPIs, campaign performance, AI insights, and recommendations.

The PFS maps the MVP functionality across six primary screens: **Login, Dashboard, Campaign Data, AI Assistant, Recommendations, and Reports**.

---

# 🧠 Business Analysis Approach

This project demonstrates an end-to-end Business Analysis and Product Design approach:

### 01 — Business Problem Definition

Identified the operational challenges created by fragmented marketing data and manual analysis.

### 02 — Requirements Analysis

Defined business requirements, business rules, functional requirements, stakeholders, success metrics and acceptance criteria.

### 03 — Process Analysis

Compared the current-state workflow with the proposed TO-BE process.

### 04 — Product Definition

Translated business requirements into product modules, features and dependencies.

### 05 — Feature Prioritization

Separated MVP capabilities from future enhancements.

### 06 — Functional Specification

Defined system behavior, user actions, inputs, outputs, business rules and acceptance criteria.

### 07 — UX Design

Translated the product workflow into information architecture, user flows, wireframes and screen-level experiences.

### 08 — Prototype

Created an interactive product prototype to demonstrate the proposed solution.

This progression reflects the documented transition from the BRD into TO-BE process design, functional specification, UX design and MVP development.

---

# 🛠️ Tools & Skills

### Business Analysis

* Requirements Analysis
* Business Requirements Documentation
* Stakeholder Analysis
* As-Is / To-Be Process Analysis
* Process Mapping
* Business Rules
* Requirements Traceability
* Acceptance Criteria
* Feature Prioritization
* MVP Definition

### Product Management & UX

* Product Vision
* Product Feature Mapping
* User Flow Design
* Information Architecture
* Wireframing
* Dashboard Design
* UX Design
* Functional Specifications
* Interactive Prototyping

### Analytics & AI

* SQL
* Excel
* Power BI
* Tableau
* Python
* Generative AI
* AI-assisted Product Design
* Marketing Performance Analytics

### Design & Prototyping

* Figma
* Canva

---

# 📌 Project Status

**Current Stage: Product Discovery → Business Analysis → Product Definition → UX Prototype**

The project currently demonstrates the **business analysis, product definition and UX/prototype layer** of the solution.

The documentation establishes the requirements, future-state process, product functionality, MVP scope, feature dependencies, acceptance criteria and UX design required to progress into implementation.

Technical implementation—including backend services, database, API integrations and production deployment—is outside the current portfolio deliverables and represents the next stage of development.

---

# 👩‍💻 My Role

### Business Analyst / Product Case Study

I independently worked across the project lifecycle, including:

* Business problem definition
* Project charter
* Business requirements
* Stakeholder analysis
* Business rules
* Success metrics
* Requirements traceability
* Current-state / future-state process analysis
* AI intervention analysis
* Product vision and scope
* Functional specifications
* MVP definition
* Feature prioritization
* Feature dependency mapping
* Acceptance criteria
* Information architecture
* User flows
* Wireframes
* UX design
* Interactive prototype
* AI-assisted decision-support concepts

---

# 📈 Expected Business Value

The proposed future-state process is designed to improve marketing operations by:

* Reducing manual campaign data consolidation
* Reducing repetitive KPI calculation
* Improving performance visibility
* Accelerating campaign analysis
* Supporting evidence-backed decisions
* Improving reporting consistency
* Reducing manual report preparation
* Allowing marketing teams to focus more on strategic optimization

The TO-BE process specifically contrasts the current manual workflow with centralized intelligence, automated KPI generation, AI-assisted analysis, automated reporting, and evidence-backed decision support.

---

# ⚠️ Portfolio Disclaimer

**MarketLens is an independent portfolio project.**

The business scenario, organization, stakeholders, campaign environment and supporting documentation are fictional and have been created for **Business Analysis and portfolio demonstration purposes**.

The project does not represent an actual implementation for a real organization.

The Project Charter explicitly identifies the business scenario as fictional and created for educational and portfolio demonstration purposes.

---

# 🔮 Future Direction

The longer-term vision is to evolve MarketLens from a controlled dataset-based MVP into a broader marketing decision-intelligence platform capable of supporting:

```text
Live Marketing Data
       ↓
Continuous Performance Monitoring
       ↓
Advanced Analytics
       ↓
AI Diagnosis & Forecasting
       ↓
Prioritized Recommendations
       ↓
Human Decision
       ↓
Automated / Scheduled Reporting
```

The core principle remains unchanged:

> **Turn marketing performance data into understandable insights and evidence-backed decisions.**

---

## ⭐ Project Objective

MarketLens is ultimately about moving marketing teams beyond **performance reporting** toward **decision intelligence**.

**Not just:**

> What happened?

**But:**

> What changed?
> Why did it change?
> Where is attention required?
> What opportunity exists?
> What action should be considered?
> What evidence supports that decision?

That is the product vision behind MarketLens.
