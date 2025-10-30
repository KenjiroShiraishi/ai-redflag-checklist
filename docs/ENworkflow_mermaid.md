flowchart TD

  A[Arrival and intake] --> B[Red flag check]
  B -->|Present| R1[R1 Immediate referral]
  B -->|Absent| C[Local intervention]
  C --> D{Decision and preference}
  D -->|Suspected condition| R2a[R2 Planned referral]
  D -->|No PCP or no checkup| R2b[R2 Planned referral to PCP]
  D -->|Patient requests opinion| R2c[R2 Preference based referral]
  D -->|Co management synergy| R2d[R2 Co management referral]
  D -->|None| R3[R3 Local care and next review date]
  R1 --> E[Emergent letter / Stop intervention / Log]
  R2a --> L[Referral letter / Education and home monitoring / Log]
  R2b --> L
  R2c --> L
  R2d --> L
  L --> L2{SDOH modifiers two or more}
  L2 -->|Yes| L3[Booking support / Dual contact]
  L2 -->|No| L4[Next step]
  R3 --> F[Self care advice / Fix next review date / Log]
