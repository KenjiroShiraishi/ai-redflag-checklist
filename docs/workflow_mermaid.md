# ワークフロー（R1/R2/R3）— 鍼灸・介護・トレーナー現場 共通

下図は、来所からレッドフラグ判定、鍼灸等の介入、計画的紹介（R2）、現場対応（R3）までの標準フローです。  
**非医師は診断せず「評価依頼として紹介」**を行う前提（安全側設計）。

```mermaid
flowchart TD
  A[来所・主訴聴取] --> B[レッドフラグチェック]
  B -->|あり| R1[ R1：即紹介（当日受診・救急含む） ]
  B -->|なし| C[介入の適否確認 → 介入実施（鍼灸/ケア/トレーニング）]

  C --> D{継続ケア判定・患者希望の確認}
  D -->|疾患の疑い\n（高BP反復/DM・甲状腺クラスター/不整脈 等）| R2a[ R2：計画的紹介（評価依頼） ]
  D -->|かかりつけ無し/健診未受診| R2b[ R2-CPR：PCP登録の計画的紹介 ]
  D -->|患者が医師意見を希望| R2c[ R2-Pref：希望起点の計画的紹介 ]
  D -->|併用シナジー\n（漢方/生活・睡眠/禁煙・減酒/疼痛・リハ/婦人科/メンタル）| R2d[ R2-Syn：共同管理の計画的紹介 ]
  D -->|該当なし| R3[ R3：現場対応継続・再評価日設定 ]

  %% R1の後処理
  R1 --> E[緊急用1枚紹介状／介入中止／ログ記録]

  %% R2群の共通アクション
  R2a --> L[1枚紹介状（評価依頼）／教育・家庭測定／ログ]
  R2b --> L
  R2c --> L
  R2d --> L
  L --> L2{SDOH修飾子≥2?}
  L2 -->|Yes| L3[予約代行／連絡方法の二重化]
  L2 -->|No| L4[次工程へ]

  %% R3の後処理
  R3 --> F[セルフケア指導／次回再評価日を固定／ログ]

  %% ポリシー注記
  classDef note fill:#f5f5f5,stroke:#bbb,color:#333;

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
