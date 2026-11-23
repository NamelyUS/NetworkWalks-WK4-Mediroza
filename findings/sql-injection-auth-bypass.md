# F-01: SQL Injection — Patient Authentication Bypass

**Severity:** Critical
**Affected endpoint:** /patient/login.php
**Parameter:** username

## Description
The patient login form was vulnerable to SQL injection.
Authentication was bypassed using the username input:

`admin'--`

No password was entered.

## Impact
Unauthorised access to the patient portal and retrieval of three confidential laboratory reports.

## Evidence
- Successful browser authentication bypass.
- Three downloaded patient PDF reports.
- Original files preserved locally under evidence/raw/.

## Recommendation
- Use parameterised SQL queries and prepared statements.
- Never concatenate user input into SQL queries.
- Implement server-side authentication and session validation.
- Return generic authentication errors.
- Audit authentication logs and invalidate potentially compromised sessions.
