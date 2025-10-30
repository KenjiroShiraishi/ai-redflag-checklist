# Workflow (R1/R2/R3) — Common to Acupuncture, Caregiving, and Trainer Settings

The diagram below shows the standard flow from arrival through red-flag screening, local intervention, planned referral (R2), and local care (R3).  
Assumption: **non-physicians do not diagnose; referrals are framed as “requests for evaluation”** (safety-first design).

```mermaid
flowchart TD
  A[Arrival and intake] --> B[Red flag check]
  B --> R1[R1 Immediate referral]
  B --> C[Local intervention]
  C --> D{Decision and preference}
  D --> R2a[R2 Planned referral - eval request]
  D --> R2b[R2 Planned referral - assign PCP]
  D --> R2c[R2 Planned referral - patient request]
  D --> R2d[R2 Planned referral - co management]
  D --> R3[R3 Local care and next review date]
  R1 --> E[Emergent letter - stop intervention - log]
  R2a --> L[Referral letter - education - home monitoring - log]
  R2b --> L
  R2c --> L
  R2d --> L
  L --> L2{SDOH modifiers two or more}
  L2 --> L3[Booking support - dual contact]
  L2 --> L4[Next step]
  R3 --> F[Self care advice - fix next review date - log]
