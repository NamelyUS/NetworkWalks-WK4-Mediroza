# M3 — Public Database Backup Exposure

Target: medirozahospital.com
Endpoint: /old/mediroza_db_backup_2019.sql

## Validation
- HTTP response: 200 OK
- Content type: text/x-sql
- File size: 6,346 bytes
- Authentication required: Not observed

## Database Structure
- staff: 30 records
- shareholders: 10 records

## Exposed Information Categories
- Employee personal and contact information
- National identification numbers
- Monthly salary information
- Shareholder ownership percentages and share classes

## Impact
An unauthenticated visitor can access a database backup containing sensitive employee and ownership information.

## Recommendation
Remove database backups from public web directories, restrict access, rotate exposed credentials where applicable, and review backup storage permissions.

Individual records are intentionally excluded from this repository.

## PDF Metadata Correlation

Inspection of Report 3's PDF Info dictionary revealed:

- Author identifier: j.malik
- Creator: Mediroza CMS 1.4.2
- Producer: Mediroza Lab Reporting Module
- Embedded comment: Database backup moved to /old before site migration; do not delete.

The author identifier corresponds to an IT Systems Administrator account in the exposed staff database.

This metadata provides a direct investigative link to the publicly accessible database backup under /old/.

Evidence: evidence/raw/report3-metadata.txt
