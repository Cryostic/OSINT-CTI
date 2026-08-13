# Phishing & Fraud Case Studies

Complete, OSINT-only investigations of **real-world phishing and fraud campaigns** targeting Philippine institutions, organizations, and individuals. Each case was conducted passively — no engagement with adversary infrastructure — and is written to professional intelligence standards: evidence-categorized, confidence-rated, and source-verified.

---

## Case Index

| Case | Status | Vector | Key Focus |
|---|---|---|---|
| [PSA National ID Phishing Investigation](PSA%20National%20ID%20Phishing%20Investigation/) | Complete | Email → phone → Google Meet pivot | Attack chain deconstruction and response |
| [MMDA NCAP Smishing Investigation](MMDA%20NCAP%20Smishing%20Investigation/) | Complete | SMS (smishing) | Lure analysis, infrastructure enrichment, detection content |

---

## Case Summaries
### PSA National ID Phishing Investigation
A complete investigation of a phishing campaign impersonating the Philippine Statistics Authority — attack chain deconstruction (email → phone → Google Meet pivot), IOC summary with confidence tiers, pattern correlation against official PSA advisories, and a filed report to PSA.

### MMDA NCAP Smishing Investigation
A complete investigation of a live SMS phishing campaign impersonating the MMDA No Contact Apprehension Policy (NCAP) — lure deconstruction, sender-ID spoofing analysis, MITRE ATT&CK mapping, and a full passive infrastructure enrichment trail (DNS / RDAP / certificate transparency, verified via VirusTotal, urlscan.io, and URLhaus), concluding with Sigma/YARA detection content and official reporting channels (MMDA, NBI, PNP-ACG).

---

## Reading Order
- Each case folder follows the same numbered structure: `01.` Executive Summary → Evidence → Technical Analysis → Attribution and Pattern Mapping → Attack Flow → Reporting → Recommendations, with appendices (detection content, references, enrichment results) where applicable.
- **Every analytical claim is categorized**: *Fact* (evidence-backed), *Assessment* (analytical conclusion), *Assumption* (unconfirmed inference), or *Hypothesis* (requires further evidence).
- **Confidence levels** (High / Medium / Low) are stated with reasoning and never inflated.
- **Intelligence gaps are explicit** — each case documents what is unknown and what collection would resolve it.

---

## Common Standards

- **Public sources only.** No interaction with adversary infrastructure — passive/OSINT-only, to avoid tipping off actors and to protect the investigator's environment.
- **No fabrication.** Evidence gaps are disclosed explicitly; nothing is invented to fill them.
- **Privacy by design.** Personal data of victims and recipients is redacted; attacker-controlled indicators (sender identifiers, domains, IPs) are defanged and published per standard CTI practice.
- **Responsible disclosure.** Findings are reported to the affected parties through their official channels before public release.

---

## Disclaimer
All case files in this directory contain **independent research** conducted for educational and defensive purposes. They are not affiliated with, endorsed by, or sponsored by any organization mentioned within. All information is derived from publicly available sources and is provided "as is" for the benefit of the defensive security community.
