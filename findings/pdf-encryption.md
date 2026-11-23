# M2 — PDF Encryption Recovery

## Files Analysed
- patient_report_1.pdf
- patient_report_2.pdf
- patient_report_3.pdf

## Encryption
- PDF encryption revision: 3
- Hash extraction: pdf2john.pl
- Password recovery: John the Ripper
- Wordlist: rockyou.txt
- Decryption: qpdf

## Results
- Report 1: Password recovered; decrypted successfully.
- Report 2: Password recovered; decrypted successfully.
- Report 3: Password recovered; decrypted successfully.

## Verification
- All three decrypted PDF files were generated.
- Original encrypted files were preserved.
- SHA-256 hashes were generated for decrypted files.

## Evidence Location
evidence/raw/

Original reports, decrypted reports, password hashes and recovered passwords are excluded from public GitHub.
