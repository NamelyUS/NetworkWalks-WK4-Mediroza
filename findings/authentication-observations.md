# Patient Portal Authentication — Initial Observations

- Endpoint: /patient/login.php
- Backend: PHP 8.2.36
- Method: POST
- Input fields: username, password
- Session cookie: PHPSESSID
- Secure attribute: Present
- HttpOnly attribute: Not observed
- SameSite attribute: Not observed
- Visible CSRF token: Not observed

These observations require further validation. No vulnerability is confirmed at this stage.

Evidence: evidence/raw/patient-login.html and patient-login-headers.txt
