# NetworkWalks — Week 4
## Mediroza General Hospital Penetration Test

**Author:** Umer Shahid  
**Batch:** B083  
**Assessment:** Black-box web application penetration test  
**Target:** https://medirozahospital.com  
**Duration:** 5 days

## Project Overview
An authorised penetration-testing assessment covering initial access, PDF encryption recovery, sensitive data exposure and professional reporting.

## Completed Milestones

### M1 — Initial Access
- Reconnaissance and service identification.
- SQL injection authentication bypass.
- Successful access to the patient portal.
- Retrieval of three laboratory PDF reports.

### M2 — Data Extraction
- PDF encryption analysis.
- Password hash extraction using pdf2john.
- Password recovery using John the Ripper.
- Successful decryption using qpdf.

### M3 — Critical Data Exposure
- Public database backup discovery.
- Exposure of staff and shareholder database tables.
- PDF metadata analysis.
- Identification of the database backup location through embedded metadata.

### M4 — Reporting
- Executive summary.
- Scope and methodology.
- Vulnerability findings and proof.
- Risk ratings.
- Remediation recommendations.

## Findings

| Finding | Severity |
|---|---|
| SQL injection authentication bypass | Critical |
| Public database backup exposure | Critical |
| Directory listing | High |
| Weak PDF encryption | High |
| Sensitive PDF metadata | Medium |

## Repository Structure
- `recon/` — Reconnaissance and scan results
- `findings/` — Individual vulnerability findings
- `evidence/` — Evidence storage
- `report/` — Final penetration-testing report
- `tools/` — Supporting scripts

## Evidence Handling
Raw patient reports, decrypted documents, database backups, passwords and personal information are excluded from the public repository.

## Disclaimer
This project was conducted under the written educational authorisation supplied by NetworkWalks. Testing was restricted to the agreed target and scope.
