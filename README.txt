LATRADUCTION CONCEPTS — CERTIFICATE VERIFICATION SYSTEM

WHAT THIS PACKAGE DOES
This is a simple verification portal. Each certificate receives a unique ID such as:
LC-2026-001
LC-2026-002
LC-2026-003

A person can open the verification page with:
https://YOUR-DOMAIN/verify/?id=LC-2026-001

The page checks the certificate registry and displays whether the certificate is valid.

FILES
- index.html                 Verification portal
- certificates.json          Live certificate registry used by the portal
- certificate_registry.csv   Easy-to-edit registry for Excel/Google Sheets
- README.txt                 This guide

ADDING A NEW STUDENT
1. Open certificates.json.
2. Add a new record with a unique certificate_id.
3. Example:
{
  "certificate_id": "LC-2026-002",
  "student_name": "JOHN DOE",
  "date_issued": "20th September, 2026",
  "program": "Training Program",
  "status": "VALID"
}
4. Upload the updated certificates.json together with index.html.

QR CODE
The QR code on each certificate should point to the verification page for that exact certificate.
Example:
https://YOUR-DOMAIN/?id=LC-2026-001

When scanned, it opens the portal and automatically displays the certificate record.

IMPORTANT
This starter system is ready to host, but it is not publicly accessible until the files are uploaded to a web host. The phrase YOUR-DOMAIN is intentionally a placeholder; do not print it on certificates.

For stronger security, keep the certificate registry under the control of Latraduction Concepts and issue IDs sequentially. Do not reuse an ID after cancellation.
