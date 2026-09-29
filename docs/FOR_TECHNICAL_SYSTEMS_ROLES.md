# Prism → Technical Systems roles

Interview-ready narrative for **Prism Digital Intake** at Clear Billing Services, mapped to technical systems / healthcare payment portal roles (secure onboarding, friction-free data capture, compliance gates).

**Live Pages demo:** https://brivera2005.github.io/clinician-mobile-intake/  
**Production (private):** https://prism.clearbillingservices.com

---

## STARS story: Prism Digital Intake

**Situation.** Client and patient charge data often arrived by email PDF or paper. That created friction, re-keying errors, and compliance exposure for a HIPAA-bound anesthesia billing operation.

**Task.** Design and ship a clinician-facing digital intake gateway so providers could hand off cases securely, on any device, without emailing PHI.

**Action.**

- Built invited-email Access with single-use MFA and an explicit PHI acknowledgment before any work.
- Dual path UX: **Add Case** (practice-tuned forms) for real-time entry, and **Upload PDF** for bulk day/week packets.
- Allowed demographics to catch up later via MRN / DOS sync so the charge path is never blocked on perfect paperwork.
- Wired intake into the Command Center operator loop so coding review and PM/EHR writeback stay downstream of a clean handoff.

**Result.** Intake moved from insecure email into a controlled portal. Onboarding friction dropped. Data entered cleaner at the source. For healthcare payment platforms helping clinics adopt hosted portals and P2PE, the same instincts apply: anticipate transition risk, keep admin UX effortless, and never lose the audit trail.

---

## Talking points

- Security and UX are not a tradeoff: MFA + PHI screen, then a calm two-path home screen.
- Bulk PDF path respects how clinics actually work on busy days.
- Async demos (later sheets) keep revenue moving without skipping identity checks.
- Always know the next system in the chain (here: Command Center).

---

## Pair with Command Center

https://github.com/brivera2005/command-center-demo
