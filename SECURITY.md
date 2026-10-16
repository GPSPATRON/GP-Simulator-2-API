# Security Policy

## Scope

This repository contains public documentation of the GP-Simulator 2 Local HTTP API and does not contain the GP-Simulator 2 application source code. Security issues in the API documentation or in the documented behavior can still be reported to GPSPATRON.

## Reporting a vulnerability

Please report suspected vulnerabilities **privately** to **support@gpspatron.com**, with the subject **GP-Simulator 2 — Security Report**. Provide the affected product version, a concise impact description, and steps to reproduce, if available.

Do not post working exploits, credentials, private logs, or personal data in public GitHub issues or pull requests. Please allow the company time to investigate and coordinate remediation before public disclosure.

## Secure configuration reminders

- Prefer **API key** mode instead of **No Auth**.
- Keep **Allow Remote Access** disabled unless necessary.
- The documented local API uses HTTP, not HTTPS: protect any remote connections by suitable network controls.
- Do not publish API keys, customer data, or other confidential information.

This file describes a reporting contact and recommended precautions; it does not represent a security warranty or a service-level agreement.
