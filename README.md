# ⚖️ Enterprise TOPSIS Decision Engine

**A client-side Multi-Criteria Decision Making (MCDM) engine utilizing the TOPSIS method (Technique for Order of Preference by Similarity to Ideal Solution). Designed for objective, data-driven IT procurement, vendor evaluation, and strategic ranking.**

[![Live Application](https://img.shields.io/badge/Live_TOPSIS_Engine-Launch_Calculator-4f46e5?style=for-the-badge&logo=githubpages)](https://edgarcia-id.github.io/topsis-decision-engine/)
[![Algorithm](https://img.shields.io/badge/Algorithm-TOPSIS_Multi--Criteria-10b981?style=for-the-badge)](#)
[![Architecture](https://img.shields.io/badge/Architecture-100%25_Client--Side-f59e0b?style=for-the-badge)](#)
[![Maintained By](https://img.shields.io/badge/Maintained_By-NusaIT-0f172a?style=for-the-badge)](https://nusait.com)

---

## 🌐 Interactive Multi-Criteria Ranking Lab
When choosing between software vendors, hardware deployments, or consulting agencies, decision-makers are forced to balance conflicting parameters: *Is a 10% lower cost worth a 5% drop in SLA uptime and a 20-day longer implementation schedule?*

We have deployed an interactive client-side TOPSIS calculator to resolve these dilemmas mathematically. It ranks alternatives by finding the option closest to the ideal theoretical solution and farthest from the worst theoretical solution:  
👉 **[Launch the Enterprise TOPSIS Decision Engine](https://edgarcia-id.github.io/topsis-decision-engine/)**

---

## 🧐 Executive Overview: The Power of TOPSIS
In Enterprise Architecture and Procurement, comparing apples-to-oranges (e.g., measuring "Cost in Dollars" against "Uptime in Percentage") is inherently flawed without proper normalization.

**TOPSIS** solves this by:
1. **Normalizing mixed data sets:** Converting disparate units (dollars, days, percentages, subjective 1-10 scores) into a dimensionless matrix.
2. **Applying Weighted Priorities:** Scaling the normalized data by executive-defined weights.
3. **Establishing Theoretical Ideals:** Creating a "Positive Ideal Solution" (combining the best traits of all candidates) and a "Negative Ideal Solution" (combining the worst).
4. **Euclidean Distance Ranking:** Calculating which candidate is geometrically closest to perfection while avoiding the worst attributes.

---

## 🏛️️ The 4-Stage Decision Architecture

This tool automates the linear algebra required for rigorous vendor evaluation:

```text
[ Business Requirements & Candidate Data ]
                 │
                 ▼
┌────────────────────────────────────────────────────────┐
│ STAGE 1: Criteria Modeling & Weight Normalization      │
│ • Define dynamic criteria constraints.                 │
│ • Assign attributes as "Benefit" (higher is better) or │
│   "Cost" (lower is better).                            │
│ • Auto-normalizes custom weights to 100%.              │
└────────────────────────────────────────────────────────┘
                 │
                 ▼
┌────────────────────────────────────────────────────────┐
│ STAGE 2: Matrix Normalization & Evaluation             │
│ • Input raw candidate data (mixed units allowed).      │
│ • Converts raw values via Vector Normalization.        │
└────────────────────────────────────────────────────────┘
                 │
                 ▼
┌────────────────────────────────────────────────────────┐
│ STAGE 3: Ideal Solution Identification (D+ & D-)       │
│ • Automatically derives the Positive Ideal and         │
│   Negative Ideal theoretical limits.                   │
└────────────────────────────────────────────────────────┘
                 │
                 ▼
┌────────────────────────────────────────────────────────┐
│ STAGE 4: Proximity Scoring & PDF Dossier               │
│ • Ranks candidates by Relative Closeness Coefficient.  │
│ • Exports an audit-ready PDF justification report.     │
└────────────────────────────────────────────────────────┘
```

---

## 🛠️ Core Features for C-Level & Procurement Managers

### 1. Dynamic Benefit vs. Cost Toggling
Seamlessly mix operational criteria. Define "Hardware Quality" as a Benefit (maximize) and "Delivery Lead Time" as a Cost (minimize). The engine mathematically reverses the polarity of cost variables during distance calculations.

### 2. Live Proximity Coefficient Ranking
As data is entered, the engine calculates the Relative Closeness Score (0.0 to 1.0). An option scoring 0.85 indicates it is highly correlated with the positive ideal solution.

### 3. Absolute Data Privacy
Built with the "Reachable Code" philosophy. The complex matrix transformations and Euclidean distance calculations execute 100% within the browser via Vanilla JavaScript. **No proprietary vendor bids or internal corporate weights are ever transmitted to an external server.**

### 4. Audit-Ready PDF Export
Generates a highly professional, native PDF report outlining the criteria weights, the input matrix, the distance calculations (D+ and D-), and the final definitive ranking. This document serves as formal evidence for procurement audits and executive steering committees.

---

## 👨‍💻 About the Author & Enterprise Architecture Partner

A mathematical ranking is only the **starting point of procurement**; the real challenge is **vendor management, secure integration, and verifiable SLAs**.

If your organization requires a seasoned technology partner to conduct an **IT Vendor Audit**, design **Enterprise Architectures**, or develop custom **ERP platforms engineered with resilience**:

**Alfredo (Ed) Garcia** is a Senior ERP Architect, IT Infrastructure Lead, and Principal Consultant at **[Nusa Industri Teknologi (NusaIT)](https://nusait.com)**. He brings deep practical expertise in bridging complex governance mandates with reachable, maintainable software architecture.

* 👔 **LinkedIn:** [Alfredo (Ed) Garcia](https://www.linkedin.com/in/alfredo-garcia-elbarta-tarigan/)
* 🏢 **Consulting Firm:** [PT Nusa Industri Teknologi (NusaIT)](https://nusait.com)
* 📧 **Consultation Inquiries:** [NusaIT Contact & Advisory](https://nusait.com/contact)

---
*© 2026 Alfredo Garcia / NusaIT. Released under the MIT License.*
