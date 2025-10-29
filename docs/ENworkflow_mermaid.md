flowchart TD
  A[Arrival and chief concern intake] --> B[Red-flag check]
  B -->|Present| R1[R1: Immediate referral (same day; ED as needed)]
  B -->|Absent| C[Assess suitability - perform local intervention (acupuncture; care; training)]

  C --> D{Continuation decision and patient preference}
  D -->|Suspected condition (repeated high BP; DM or thyroid clusters; irregular pulse)| R2a[R2: Planned referral (request for evaluation)]
  D -->|No PCP or no checkup| R2b[R2-CPR: Planned referral to register with PCP]
  D -->|Patient requests physician opinion| R2c[R2-Pref: Preference-based planned referral]
  D -->|Co-management synergy (Kampo; lifestyle and sleep; cessation; pain and rehab; gynecology; mental health)| R2d[R2-Syn: Planned referral for co-management]
  D -->|None| R3[R3: Continue local care and set next review date]

  R1 --> E[One-page emergent referral letter - stop intervention - log]

  R2a --> L[One-page referral (evaluation) - education and home monitoring - log]
  R2b --> L
  R2c --> L
  R2d --> L
  L --> L2{SDOH modifiers >= 2?}
  L2 -->|Yes| L3[Booking support - dual contact methods]
  L2 -->|No| L4[Next step]

  R3 --> F[Self-care advice - fix next review date - log]
