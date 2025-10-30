# Workflow (R1/R2/R3) — Common to Acupuncture, Caregiving, and Trainer Settings

The diagram below shows the standard flow from arrival through red-flag screening, local intervention, planned referral (R2), and local care (R3).  
Assumption: **non-physicians do not diagnose; referrals are framed as “requests for evaluation”** (safety-first design).

```mermaid

flowchart TD
  A[Arrival & chief concern intake] --> B[Red-flag check]
  B -->|Present| R1[ R1: Immediate referral (same-day; ED as needed) ]
  B -->|Absent| C[Assess suitability → Proceed with local intervention (acupuncture/care/training)]

  C --> D{Continuity & preference check}
  D -->|Suspected condition\n(repeated high BP / DM & thyroid clusters / irregular pulse)| R2a[ R2: Planned referral (request for evaluation) ]
  D -->|No PCP / No checkup| R2b[ R2-CPR: Planned referral to register with PCP ]
  D -->|Patient requests physician opinion| R2c[ R2-Pref: Preference-based planned referral ]
  D -->|Co-management synergy\n(Kampo / lifestyle & sleep / cessation / pain & rehab / gynecology / mental health)| R2d[ R2-Syn: Planned referral for co-management ]
  D -->|None| R3[ R3: Continue local care & set next review date ]

  %% Post-R1 actions
  R1 --> E[1-page emergent referral letter / stop intervention / log]

  %% Common actions for R2 group
  R2a --> L[1-page referral (evaluation) / education & home monitoring / log]
  R2b --> L
  R2c --> L
  R2d --> L
  L --> L2{SDOH modifiers ≥ 2?}
  L2 -->|Yes| L3[Booking support / dual contact methods]
  L2 -->|No| L4[Next step]

  %% Post-R3 actions
  R3 --> F[Self-care advice / fix next review date / log]

  %% Policy note
  classDef note fill:#f5f5f5,stroke:#bbb,color:#333;
