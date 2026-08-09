# OSINT-CTI — Cyber Threat Intelligence Portfolio

Independent open-source threat intelligence research focused on the **Southeast Asia and Philippines threat landscape**. All analysis is defensive in intent, derived exclusively from public sources, and produced to professional intelligence standards: evidence-categorized, confidence-rated, and source-verified.

---

## Repository Contents

| Project | Status | Description |
|---|---|---|
| [Philippines Threat Landscape](Philippines%20Threat%20Landscape/README.md) | Complete | Strategic and operational assessment of threats targeting Philippine government, enterprise, and critical infrastructure sectors |
| [Threat Actor Profiles](Threat%20Actor%20Profiles/README.md) | In progress | Structured profiles of advanced persistent threat (APT) actors operating in the ASEAN / APAC theater |
| [PSA National ID Phishing Investigation](PSA%20National%20ID%20Phishing%20Investigation/) | Complete | Full investigation of a real-world phishing campaign impersonating the Philippine Statistics Authority (PSA) |

---

## Projects

### 1. Philippines Threat Landscape — Complete

An open-source intelligence repository covering the threats actively targeting Philippine networks:

- **Key Judgments** — prioritization of the most significant threats (state-sponsored espionage, ransomware, vulnerability exploitation)
- **Threat Actor Assessment** — Diamond Model analysis and structured hypotheses for each significant actor
- **Campaign Analysis** — observed intrusion patterns and malware distribution chains
- **Vulnerability & Malware Intelligence** — exposure assessment relevant to Philippine infrastructure
- **Industry & Geographic Impact** — sector and regional targeting trends
- **MITRE ATT&CK Mapping** — confirmed TTP matrix for Philippines-relevant operations
- **Detection, Recommendations, Risk Matrix, and Intelligence Gaps** — actionable defensive output

### 2. Threat Actor Profiles — In progress

Structured profiles tracking aliases, attribution confidence, victimology, campaign history, and TTPs for APT actors relevant to the region. Each profile follows a consistent numbered template.

**Currently covered:** APT40, Dark Pink, Earth Lusca, Mustang Panda, Naikon, OceanLotus, Patchwork, SideWinder

**Status:** Sections 01–05 (Executive Summary, Attribution, Victimology, Campaign History, TTPs) are complete for all actors. Sections 06–10 are under development; profiles are being finished depth-first rather than released half-complete.

### 3. PSA National ID Phishing Investigation — Complete

A complete investigation of a phishing campaign impersonating the Philippine Statistics Authority, conducted as a passive, OSINT-only case:

- **Evidence handling** — documented chain of custody and explicit redaction policy
- **Technical analysis** — attack chain deconstruction (email → phone → Google Meet pivot) and IOC summary with confidence tiers
- **Attribution** — pattern correlation against official PSA advisories and independent vendor research (sources verified)
- **Reporting & Recommendations** — a filed report to PSA and a public awareness guide
- **Honest gap disclosure** — collection limitations documented rather than omitted

---

## How to Read This Repository

- **Numbered files are reading order.** Each project starts at `01.` and progresses to the final section; appendices (`Appendix A`, `Appendix B`) provide supporting detail.
- **Every analytical claim is categorized**: *Fact* (evidence-backed), *Assessment* (analytical conclusion), *Assumption* (unconfirmed inference), or *Hypothesis* (requires further evidence).
- **Confidence levels** (High / Medium / Low) are stated with reasoning and are never inflated.
- **Intelligence gaps are explicit** — each project documents what is unknown and what collection would resolve it.

---

## Methodology & Standards

This repository operationalizes the **Intelligence Lifecycle**: Direction → Collection → Processing → Analysis → Production → Dissemination.

**Analytical frameworks applied:**

- MITRE ATT&CK (Enterprise) for technique mapping
- Diamond Model for adversary-victim-infrastructure-capability analysis
- Structured Analytic Techniques — including Analysis of Competing Hypotheses (ACH)
- Cyber Kill Chain / Unified Kill Chain for intrusion lifecycle mapping
- Intelligence Priority Requirements (PIRs) to guide collection focus

**Standards:**

- **Public sources only.** No engagement with adversary infrastructure — all investigations are passive/OSINT-only to avoid tipping off actors and to protect the investigator's environment.
- **No fabrication.** Evidence gaps are disclosed explicitly; nothing is invented to fill them.
- **Privacy by design.** Personal data is redacted; attacker-controlled indicators are published per standard CTI practice.
- **Responsible disclosure.** Findings are reported to affected parties through their official channels.

---

## Status & Roadmap

-  Philippines Threat Landscape — complete; maintained as new public reporting emerges
-  PSA National ID Phishing Investigation — complete
-  Threat Actor Profiles — 01–05 complete across 8 actors; 06–10 in development (depth-first)

**Planned additions:** detection artifacts (Sigma / YARA), IOC enrichment exercises, regional campaign tracking.

---

## Disclaimer

This repository contains **independent research** conducted for educational and defensive purposes. It is not affiliated with, endorsed by, or sponsored by any organization mentioned within. All information is derived from publicly available sources and is provided "as is" for the benefit of the defensive security community.
