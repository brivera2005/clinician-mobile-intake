# ClearBilling · Prism Clinician Intake (Demo)

**Synthetic data only. Not for clinical use. Not connected to production PHI.**

Interactive GitHub Pages demo of **Prism**, the HIPAA-oriented clinician intake portal from Clear Billing Services, Inc.

## Open the demo

**https://brivera2005.github.io/clinician-mobile-intake/**

Or open [`index.html`](./index.html) locally.

## What Prism does

1. **Sign in** with an invited work email + Cloudflare Access login code (8-hour sessions).
2. **Accept the PHI screen**, then choose **How do you want to work today?**
3. **Add cases** (new, recommended) through the day: MRN, DOS, Times, facility, surgeon, procedure (Cataract, iStent, UL, LL, or Add procedure), diagnosis (Glaucoma, or Add DX), additional notes last.
4. **Or Upload PDF** (classic) for charge sheets plus demographic sheets for the whole day, week, or whatever you have. One PDF or several. Either is fine. Through Prism instead of email.
5. **Demographics sync later by MRN** so case capture does not wait on face sheets.

Production URL for invited practices: `https://prism.clearbillingservices.com` (not this public demo).

## Screenshots

Each step, then the screen. Synthetic data, not live examples. Order: sign in → work-today chooser → Add cases → Upload PDF.

| | |
|---|---|
| ![Access login](screenshots/01-access-login.png) | ![How do you want to work today](screenshots/04-mode-gate.png) |
| ![Add cases](screenshots/02-add-case.png) | ![Upload PDF](screenshots/03-upload-pdf.png) |

## Documentation

- [Provider guide (PDF)](docs/Prism-Provider-Guide.pdf) - practice-facing handout
- [HIPAA & security](docs/HIPAA-AND-SECURITY.md) - program + live technical safeguards

## UL / LL

Lid procedures. Chips are labeled **UL** / **LL**. Add procedure is for anything else. ASA is derived in the live app from the procedure (not typed in).

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
