# Prism · HIPAA & security

**Framing:** HIPAA does not "certify" software. What matters is a covered entity / business associate program with BAAs, written policies, workforce training, and live technical safeguards. Clear Billing Services, Inc. runs that program. Prism is the transfer channel to Clear Billing Services, Inc. inside it.

This document describes the **live product posture** for Prism. The public GitHub Pages demo is synthetic only and does not process PHI.

## Organizational / legal

| Control | Clear Billing Services, Inc. |
| --- | --- |
| Business Associate Agreements | BAA with the practice and applicable vendors |
| Written policies | Access control, breach notification, remote device rules |
| Workforce training | Ops + providers trained; acknowledgments on file |
| Unique identities | Named invited emails only (no shared logins) |
| Offboarding | Access removed when someone leaves |

## Technical safeguards (live Prism)

| Control | What runs |
| --- | --- |
| Edge Zero Trust | Cloudflare Access in front of Prism before any app UI |
| Allowlisted identity | Practice emails must be invited. Prism emails a single-use MFA login code |
| Time-boxed sessions | Access sessions last **8 hours**; Out clears the Access session |
| Encrypted transport | HTTPS + HSTS; Cloudflare Tunnel ingress |
| Network posture | App not port-forwarded publicly; not left open on an office LAN |
| Browser hardening | Security headers (frame deny, nosniff, referrer, CSP posture) |
| PHI acknowledgment | Blocking PHI screen before use; acknowledgment stored |
| PHI hygiene | Vault storage; confirmation emails carry **no PHI**; no chart download back to personal devices |
| Audit & backups | Sign-in / intake logging; routine backups on the dedicated host path at Clear Billing Services, Inc. |

## Safer than common shortcuts

| Approach practices still use | Typical gap | Prism |
| --- | --- | --- |
| Email PDFs / text photos | PHI in inboxes, forwarding, weak audit | Prism portal + allowlisted users + vault |
| Shared office password | No identity, hard offboarding | Per-person invited email + Access codes |
| Generic Drive / form links | Broad links, weak BA posture | Zero Trust edge + Prism vault |
| Open cloud app with password only | Public surface, stuffing risk | Cloudflare Access first, then app session |

## What we do not claim

- Not “HIPAA certified” (that product category mostly does not exist)
- Not a replacement for the practice’s own HIPAA program
- Not immune to phishing of a user’s email inbox (Access + allowlist still shrink blast radius)
- New provider emails must be added to the invite list on onboard

## Related docs

- [Prism Provider Guide (PDF)](./Prism-Provider-Guide.pdf)
- Live product (invite-only): `https://prism.clearbillingservices.com`
