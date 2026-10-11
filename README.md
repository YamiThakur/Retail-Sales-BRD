# Retail Store Sales Reporting System: Business Requirement Document

A Business Requirement Document (BRD) for an interactive sales dashboard that replaces a manual, Excel-based monthly sales review for a retail store with about ₹4.8 crore in annual sales.

| | |
|---|---|
| **Author** | Yamini Thakur, Business Analyst |
| **Version** | 1.0 (30 September 2026) |
| **Status** | Pending approval |
| **Planned go-live** | 11 December 2026 |
| **Estimated budget** | ₹3,78,400 (illustrative) |

📄 **Document:** [`Business_Requirement_Document.docx`](./Business_Requirement_Document.docx)
---

## The problem in brief

- Monthly sales swing by up to ±18%, but nobody can quickly see which categories, customer segments or periods are driving it.
- Sales sit in manually maintained Excel sheets. The monthly review takes about **12 person-hours** and arrives about **10 working days** after month-end.
- Around **6% of records** (about 1,080 a year) are missing, duplicated or inconsistent.
- Decisions on promotions, staffing and purchasing are made on data that is 2 to 6 weeks old.

## The proposed solution

A 3-page, web-based dashboard (Overview, Category and Customer Analysis, Trends and Data Quality) with automated validation, a weekly Monday-by-10:00 refresh, role-based access and filtering by date, category, gender and age group.

| Metric | Today | Target |
|---|---|---|
| Effort to prepare monthly review | 12 hours | ≤ 1 hour |
| Report availability | ~10 working days | ≤ 2 working days |
| Invalid records reaching KPIs | ~6% | < 1% |
| KPI accuracy vs reconciled totals | Not measured | ≤ 0.5% variance |
| Weekly dashboard adoption | 0 users | ≥ 80% of intended users |

---

## Frameworks and methods used

Each framework below is applied in the BRD itself. The section numbers point to where.

### 1. MoSCoW prioritisation (Sections 7, 8, Appendix A)
Every business requirement (BR-01 to BR-10) and functional requirement (FR-01 to FR-15) is tagged **Must / Should / Could**. This keeps the go-live scope focused on what the 9-week timeline and fixed budget can deliver.
- **Must:** centralised view, category and segment analysis, trends, core KPIs, data validation, weekly refresh, access control
- **Should:** filters, average sales per transaction, growth %, exception log
- **Could:** PDF and Excel export
- **Won't (this release):** forecasting, POS integration, profit analysis, mobile app (Section 5.2)

### 2. Objectives with baseline, target and measurement (Section 2)
Five objectives (O-01 to O-05) are written as measurable outcomes, each with a **baseline, target, timeline and measurement source**. This is the same discipline as OKRs and SMART goals. Objectives are linked to the requirements that deliver them.

### 3. KPI definition framework (Section 9.2)
Six KPIs are defined once, with a formula and a requirement link: Total Sales, Total Transactions, Total Quantity Sold, Average Sales per Transaction, Sales Growth % and Category Share %. NFR-08 requires every page to use these single definitions, so the same number never appears with two meanings.

### 4. Current state, future state and gap analysis (Sections 3, 4)
The current process and its quantified pain points are set against the proposed future state in a side-by-side table (Section 4.2). This makes the business case visible before any solution detail is discussed.

### 5. Stakeholder analysis (Section 6)
Eight stakeholders are mapped by role, interest and involvement, including sponsor, data owner, validator, builder and enabler.

### 6. Use cases and process flow (Section 11)
- A 9-step proposed process flow with owners and timings
- Three detailed use cases (UC-01 Analyse sales performance, UC-02 Analyse category and customer segments, UC-03 Refresh and validate weekly data), each with actor, preconditions, main, alternate and exception flows, and linked requirements

### 7. Functional and non-functional requirements (Sections 8, 10)
Requirements are grouped by theme (Data Management, KPIs and Analysis, Filters/Export/Access). Non-functional requirements (NFR-01 to NFR-09) are written with **measurable thresholds** for performance, accuracy, usability, availability, security, scalability, compatibility, consistency and retention.

### 8. Data requirements (Section 9)
A data dictionary, KPI definitions and eight validation rules (DV-01 to DV-08), each with an action (reject, flag or label as Unknown) and a severity. A 5% rejection threshold holds publishing, which acts as a quality gate.

### 9. Requirements traceability matrix (Section 14)
Every **business requirement → objective → functional requirement → non-functional requirement → acceptance criterion** is linked. No requirement exists without a business reason, and none is left untested.

### 10. Acceptance criteria and UAT approach (Section 13)
Twelve testable criteria (AC-01 to AC-12), verified through UAT with 5 users, a test file with 50 seeded invalid records and Finance-reconciled totals for 3 sample months.

### 11. RAID log (Section 12)
**R**isks (with likelihood, impact and mitigation), **A**ssumptions, **I**ssues/constraints and **D**ependencies (with owners and due dates).

### 12. Phased roadmap and lifecycle planning (Sections 15, 16)
- A 9-week delivery plan in five phases: sign-off, data preparation, development, UAT, go-live and handover
- A future-enhancements roadmap (forecasting, real-time/POS integration, margin analysis, scheduled reports and mobile) assigned to Phase 2 and Phase 3, which is also how scope creep is handled through change control (R-05)

### 13. Cost-benefit and payback estimate (Section 15)
Budget breakdown, time saved (about 132 hours a year), estimated uplift and payback period of about 6 to 7 months.

---

## Product management skills demonstrated

| Skill | Where it shows up in this project |
|---|---|
| **Product Requirements** | Sections 7 to 10: business, functional, non-functional and data requirements |
| **Feature Prioritization** | MoSCoW tagging on all requirements; explicit out-of-scope list |
| **OKRs and KPI Definition** | Section 2 objectives with baselines and targets; Section 9.2 KPI definitions |
| **User Experience (UX)** | 3-page information architecture, filter behaviour, empty-state and stale-data messages, and usability targets (NFR-03, AC-10) |
| **Roadmap Planning** | 9-week delivery plan and Phase 2/3 enhancement roadmap |
| **Product Lifecycle Management** | Requirements → build → UAT → go-live → handover → future phases |
| **Product Development** | Traceability to acceptance criteria, UAT design, handover runbook |
| **Product Strategy** | Problem framing, objectives, scope boundaries and phased value delivery |
| **Software Product Management** | Stakeholder management, change control, risk and dependency management |
| **Product Launch** | Go-live and handover phase: training, user guide, runbook and adoption target (O-04) |
| **Product Vision** | A single trusted source of sales data that lets management act on weekly numbers instead of preparing them |

---

## Repository contents

```
├── README.md
└── Business_Requirement_Document.docx
```

## Notes

- Budget, benefit and payback figures are **illustrative estimates for planning**.
- This is a requirements document. It does not contain the built dashboard.

## Author

**Yamini Thakur**, Business Analyst
