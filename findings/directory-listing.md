# Finding: Public Directory Listing

Affected paths:
- /patient/
- /patient/reports/
- /old/

Evidence:
- evidence/raw/patient-index.html
- evidence/raw/old-index.html

Observed exposures:
- Patient reports directory
- Application files
- Public database backup filename

Impact: Unauthorised directory enumeration and potential disclosure of restricted application files.

Status: Directory listing confirmed. Individual file access requires separate validation.

## Additional Validation

- /patient/ directory listing: HTTP 200
- /staff/ directory listing: HTTP 200
- /old/ directory listing: HTTP 200
- /patient/reports/: HTTP 403
- /patient/download.php: HTTP 302 to login.php
- /patient/portal.php: HTTP 302 to login.php

The database backup filename is publicly discoverable. Direct file access remains to be validated.
