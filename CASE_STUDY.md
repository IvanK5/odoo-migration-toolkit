# Case Study — Odoo Data Structuring & Zero-Discrepancy Migration

**Client:** EdenAppart SAS (Eden Assist) — short-term rental concierge company, Aix-en-Provence, France (~70 properties)
**Role:** Revenue Management & Data Structuring Intern · May–July 2026
**Stack:** Odoo v17 & v19 · Python (XML-RPC) · QWeb · SQL

## The problem

The company's commercial data had outgrown its tools. 350 prospecting records lived in Odoo's **Project module** — the wrong place for a sales pipeline — with no underlying data model, no automated documents, and a version gap (v17 → v19) between instances. Every contract was assembled by hand; pricing knowledge was scattered across individual records.

## What I did

**Designed a 20-table data model** covering the property lifecycle end to end: prospects, owners, properties, contracts, onboarding tasks, and pricing — the schema the business actually runs on, not the one the default modules impose.

**Migrated 350 records across 230+ fields with zero discrepancies.** The migration ran as Python scripts over Odoo's XML-RPC API (cross-instance, v17 → v19). Verification wasn't a spot check: **6,816 field-level comparisons**, every source value tested against its destination.

**Automated contract generation with QWeb** — terms and appendices produced as PDFs directly from CRM data, removing manual assembly.

**Configured the property lifecycle in the Project module**: 16 onboarding tasks per department, phase-based archiving.

**Extracted and structured 69 pricing profiles** from unstructured records, giving management a usable base for direct-booking pricing strategy.

## The result

A CRM the sales team can trust (v19, clean model, zero migration errors), contracts that generate themselves, an onboarding process with a defined lifecycle, and pricing data that became decision-ready. Confidential client data, record contents, and commercial terms are deliberately excluded from this document.

## Why it's transferable

Every growing SMB on Odoo hits this wall: data in the wrong modules, no model, manual documents, version drift. The method — model first, scripted migration, field-level verification, then automation — is repeatable. That's the service I sell.

---

ivankirtis5@gmail.com · [LinkedIn](https://www.linkedin.com/in/ivan-houngbo) · [GitHub](https://github.com/IvanK5)
---

ivankirtis5@gmail.com · [LinkedIn](https://www.linkedin.com/in/ivan-houngbo) · [GitHub](https://github.com/IvanK5)
