# odoo-migration-toolkit

Python (XML-RPC) patterns for structuring and migrating Odoo data across instances and versions — battle-tested on a real v17 → v19 migration: 350 CRM records, 230+ fields, 6,816 field-level checks, **zero discrepancies**.

Full write-up of the underlying project: [CASE_STUDY.md](CASE_STUDY.md)

## The method

**Model first.** Design the target data model before touching records — the schema the business actually runs on, not the one the default modules impose.

**Scripted migration.** Batch reads and writes over the XML-RPC API, with explicit field mapping between source and destination — including cross-version renames and type changes.

**Field-level verification.** Every source value tested against its destination. On the reference project that meant 6,816 comparisons — a verification loop, not a spot check.

**Automate after.** Document generation (QWeb) and lifecycle workflows come only once the data is trusted.

## Contents

`CASE_STUDY.md` — the real-world migration this repo distills. Sanitized script templates (connection/auth, batch export, field mapping, migration writer, verification loop) are being added — July 2026.

## Stack

Odoo v17/v19 · Python 3 · XML-RPC · QWeb

---

Sègnon Ivan Jonas Houngbo · [LinkedIn](https://www.linkedin.com/in/ivan-houngbo) · ivankirtis5@gmail.com
