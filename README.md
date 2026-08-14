# ClearBilling · Prism Clinician Intake (Demo)

**Synthetic data only. Not for clinical use. Not connected to production PHI.**

Interactive GitHub Pages demo of **Prism**, the HIPAA-oriented clinician intake portal from Clear Billing Services, Inc.

## Open the demo

**https://brivera2005.github.io/clinician-mobile-intake/**

Or open [`index.html`](./index.html) locally.

## What Prism does

1. **Sign in** with an invited work email. Prism emails a single-use MFA login code (8-hour sessions).
2. **Accept the PHI screen**, then choose **How do you want to work today?**
3. **Add cases** (new, recommended): custom-built to your practice and workflow (most-used procedures, diagnoses, and the rest of the form). Enter each case as you finish it, on phone, tablet, or computer.
4. **Or Upload PDF** (classic) for charge sheets plus demographic sheets for the whole day, week, or whatever you have. One PDF or several. Either is fine. Through Prism instead of email.
5. Either path can **sync to that MRN or DOS**. Demographic sheets can arrive later.

**$49 / month.** Covers the Prism app, secure login, PHI screen, maintenance, dedicated hosting, power, uplink, and backups.

Production URL: `https://prism.clearbillingservices.com` (not this public demo).

## Screenshots

Each screenshot is synthetic, not a live example.

| | |
|---|---|
| ![Access login](screenshots/01-access-login.png) | ![How do you want to work today](screenshots/04-mode-gate.png) |
| ![Add cases](screenshots/02-add-case.png) | ![Upload PDF](screenshots/03-upload-pdf.png) |

## Documentation

- [Provider guide (PDF)](docs/Prism-Provider-Guide.pdf) - practice-facing handout
- [HIPAA & security](docs/HIPAA-AND-SECURITY.md) - program + live technical safeguards

## UL / LL

Lid procedures. Chips are labeled **UL** / **LL**. Add procedure is for anything else.

## Pair with Command Center (portfolio)

Downstream coding / operator desk demo:

- Flagship: https://github.com/brivera2005/command-center-demo
- Operator guide: https://github.com/brivera2005/command-center-demo/blob/main/docs/OPERATOR_GUIDE.md
- Portfolio index: https://github.com/brivera2005/healthcare-portfolio

## Author

Benjamin M. Rivera · Clear Billing Services, Inc.  
LinkedIn: https://linkedin.com/in/brivera2005  
Email: brivera2005@gmail.com

## License

MIT
