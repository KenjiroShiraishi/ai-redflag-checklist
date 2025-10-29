# ワークフロー（R1/R2/R3）/ Workflow (R1/R2/R3)

非医師は診断せず、「評価依頼として紹介」する安全側設計。 / Safety-first: non-physicians do not diagnose; referrals are framed as “requests for evaluation.”

---

<details>
<summary><strong>日本語版を開く / Show Japanese</strong></summary>

```mermaid
flowchart TD
  A[来所・主訴聴取] --> B[レッドフラグチェック]
  B -->|あり| R1[R1：即紹介（当日受診・救急含む）]
  B -->|なし| C[介入の適否確認 → 介入実施（鍼灸／ケア／トレーニング）]

  C --> D{継続ケア判定・患者希望の確認}
  D -->|疑い（高BP反復／DM・甲状腺クラスター／不整脈）| R2a[R2：計画的紹介（評価依頼）]
  D -->|かかりつけ無し／健診未受診| R2b[R2-CPR：PCP登録の計画的紹介]
  D -->|患者が医師意見を希望| R2c[R2-Pref：希望起点の計画的紹介]
  D -->|併用シナジー（漢方／生活・睡眠／禁煙・減酒／疼痛・リハ／婦人科／メンタル）| R2d[R2-Syn：共同管理の計画的紹介]
  D -->|該当なし| R3[R3：現場対応継続・次回再評価日を設定]

  R1 --> E[緊急用1枚紹介状／介入中止／ログ]

  R2a --> L[1枚紹介状（評価依頼）／教育・家庭測定／ログ]
  R2b --> L
  R2c --> L
  R2d --> L
  L --> L2{SDOH修飾子が2つ以上？}
  L2 -->|はい| L3[予約代行／連絡方法の二重化]
  L2 -->|いいえ| L4[次工程へ]

  R3 --> F[セルフケア指導／次回再評価日を固定／ログ]

