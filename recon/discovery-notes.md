# Initial Web Reconnaissance

## robots.txt
HTTP 200
Disallowed paths:
- /patient/
- /staff/
- /old/

## Sitemap
HTTP 200
Public pages:
- /index.html
- /about.html
- /doctors.html
- /contact.html

## Homepage Links
- /patient/login.php
- /staff/login.php

## Initial Observations
The robots.txt entries are crawler directives, not access controls.
Login endpoints are linked from the homepage but absent from the sitemap.
Further validation is required.
