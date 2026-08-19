# Email Automation — Sequence Templates

> The consent-first newsletter system of The People's Register, published as reusable patterns: sequence templates, segmentation model, and compliance notes.

![Production](https://img.shields.io/badge/status-production-3ecf6e) ![Brevo](https://img.shields.io/badge/engine-brevo-0e141d) ![License](https://img.shields.io/badge/license-MIT-b8860b)

---

## The sequence model

```
SIGNUP → DOUBLE OPT-IN → WELCOME → SEGMENTATION → CADENCE → EXIT
```

| Step | Rule |
|---|---|
| Signup | Explicit opt-in checkbox — **no pre-checked consent** |
| Double Opt-In | Confirmation email via Brevo — nothing is sent until confirmed |
| Welcome | Onboarding: the publication, its sources, its cadence |
| Segmentation | Language preference captured at signup (EN / isiXhosa / Afrikaans) |
| Cadence | Weekly briefing + numbered issue-release alerts, verified against primary sources |
| Exit | One-click unsubscribe, honoured instantly |

## The welcome email (production copy)

See `templates/welcome-email.md` for the exact copy shipped in the double opt-in sequence.

## Compliance notes

- Consent language is explicit on the signup form and repeated in the confirmation flow
- Honeypot field for bot defence
- Published privacy notice documents subscription terms and unsubscribe rights
- List hygiene: confirmed addresses only, stable sender identity

---

*Author: Rowan Sampson — Digital Origin. The system runs on Brevo; sender identity: The People's Register.*
