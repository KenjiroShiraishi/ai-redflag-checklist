flowchart TD
 A[Arrival and intake] --> B[Red flag check]
 B -->|Present| R1[R1 Immediate referral (same day or ED)]
 B -->|Absent| C[Assess suitability -> Local intervention]
 C --> D{Continuation decision and patient preference}
 D -->|Suspected condition| R2a[R2 Planned referral (request for evaluation)]
 D -->|No PCP or no checkup| R2b[R2 Planned referral to register with PCP]
 D -->|Patient requests opinion| R2c[R2 Preference based planned referral]
 D -->|Co management synergy| R2d[R2 Co management planned referral]
 D -->|None| R3[R3 Continue local care and set next review date]
 R1 --> E[Emergent one page letter / Stop intervention / Log]
 R2a --> L[One page referral / Education and home monitoring / Log]
 R2b --> L
 R2c --> L
 R2d --> L
 L --> L2{SDOH modifiers two or more}
 L2 -->|Yes| L3[Booking support and dual contact methods]
 L2 -->|No| L4[Next step]
 R3 --> F[Self care advice / Fix next review date / Log]
