# MMDA NCAP Smishing Case Study

**Case:** SMS phishing ("smishing") impersonating the Metro Manila Development Authority (MMDA) No Contact Apprehension Policy (NCAP)

**Case ID:** `PH-SMISH-2026-0813-NCAP-001`

| Field | Value |
|---|---|
| **Date of receipt** | August 13, 2026, 10:51 AM (PHT, as indicated on device) |
| **Delivery vector** | SMS (short message service) |
| **Language** | Filipino (Tagalog/informal "Taglish" register) |
| **Impersonated entity** | MMDA — No Contact Apprehension Policy (NCAP) |
| **Sender indicator** | `el-mashharawi@live[.]de` (email-looking alphanumeric sender identifier) |
| **Embedded link** | `ncapmmda[.]skin` (non-goverment TLD) |
| **Recipient action** | No reply, no click. Evidence preserved passively. |
| **Analysis tier** | Full Intelligence Assessment (defensive CTI) |

---

## Repository Map

| File | Content |
|---|---|
| `01. Executive Summary.md` | Leadership-level summary, key findings, severity |
| `02. Evidence.md` | Case metadata, raw message (defanged), IOC table, pyramid-of-pain assessment |
| `03. Technical Analysis.md` | Delivery mechanics, linguistic analysis, domain/URL analysis, MITRE ATT&CK mapping, kill chain |
| `04. Attribution and Pattern Mapping.md` | What can and cannot be attributed; comparison with known Philippine smishing patterns |
| `05. Attack Flow Diagram.md` | Mermaid diagram + step-by-step narrative of the attack chain |
| `06. Reporting.md` | Official reporting channels (MMDA, NBI, PNP-ACG, NTC, DICT) + reporting template |
| `07. Recommendations.md` | Prioritized defensive recommendations for individuals and organizations |
| `08. Detection Content.md` | Sigma rules, YARA rule, keyword watchlist for detection engineering |
| `09. References.md` | Cited sources with reliability and timeliness assessment |
| `10. Enrichment Results.md` | Passive infrastructure enrichment: DNS, RDAP, certificate transparency, hosting findings (2026-08-13) |

---

## Scope and Methodology

- **Scope:** Defensive analysis of a single received smishing message. No intrusion, no compromise, no interaction with the lure.
- **Method:** Intelligence lifecycle (direction → collection → processing → analysis → production). Evidence is categorized as **Fact**, **Assessment**, **Assumption**, or **Hypothesis**, each with a confidence level.
- **Handling:** The phishing URL and sender identifier are **defanged** throughout (`[.]`, `[at]`, `hxxps://` conventions). No personal data of the recipient is disclosed.
- **Active engagement policy:** The analyst did **not** click the link, reply to the sender, or load the phishing page. Content of the landing page is therefore an assessed unknown (intelligence gap), not an observed fact.

## Disclaimer

This document is provided for educational and defensive security purposes. It does not constitute legal advice. The indicators contained herein were observed on the stated date and may be rotated, reused, or repurposed by the operators at any time. Independently verify all indicators before operational use.

**Analyst note:** This case is part of an active law-enforcement investigation in the Philippines (NBI, per public reporting as of August 2026). When publishing, consider coordinating with or citing official statements rather than publishing raw infrastructure details that could alert the operators.
