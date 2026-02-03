# Red Flag Checklist for Non-specific Symptoms (including Post-COVID / Long COVID) — Template
**For**: Non-physician frontline practitioners (e.g., acupuncturists, trainers, care workers) to standardize “do-not-miss” danger signals  
**Goals**: (1) Reduce missed serious illness (2) Standardize referral decisions (3) Document explanations and actions (audit trail)  
**Important**: This checklist is **not a diagnosis**. If any red flag is present, **stop/avoid treatment and arrange urgent medical evaluation**.

---

## 0. How to Use (Workflow)
1) At the start of each visit, screen **R1 → R2 → R3** (red flags override other decisions)  
2) Record **vitals** (ideally BP/HR/SpO2/temperature)  
3) **R1 (Emergency)**: Call EMS / send to ED immediately  
4) **R2 (Urgent)**: Same-day to 48-hour medical assessment  
5) **R3 (Planned)**: Medical review within days to 2 weeks (earlier if worsening/functional impairment)  
6) Document red flags, actions, and patient-facing explanation; share with the physician if agreed

---

## 1. Vital Signs (Recommended)
- Date/time:  
- BP: 1st ____ / ____ mmHg, Pulse ____ /min  
- BP: 2nd ____ / ____ mmHg, Pulse ____ /min (repeat after 1–2 minutes)  
- SpO2: ____ % (if available)  
- Temperature: ____ °C  
- Posture: □seated □standing (note orthostatic worsening)

**Measurement note**: quiet rest, correct cuff size, arm supported at heart level, measure on bare upper arm.

---

## 2. Red Flags

### R1: Emergency now (any “YES”)
- □ **Severe shortness of breath** at rest / cannot speak full sentences  
- □ **Chest pain/pressure** (tightness, diaphoresis, nausea, radiating pain)  
- □ **Altered consciousness**, seizure, fainting with injury  
- □ **Possible stroke**: facial droop, one-sided weakness/numbness, speech difficulty, sudden vision loss, sudden severe dizziness/ataxia  
- □ **Sudden “worst headache”** or neck stiffness  
- □ **Marked SpO2 drop** (clearly lower than usual, consistent with dyspnea)  
- □ **Very high BP**: roughly **≥180/120 mmHg** *with* chest pain, dyspnea, neuro/visual symptoms  
- □ **Suspected thromboembolism**: sudden dyspnea + pleuritic chest pain/hemoptysis, or unilateral leg swelling/pain + respiratory symptoms

### R2: Urgent medical assessment (same day to 48 hours)
- □ Persistent/worsening dizziness or imbalance affecting walking (≥24 hours continuous or worsening)  
- □ New palpitations/irregular pulse with dizziness/presyncope  
- □ Recurrent syncope, or syncope with chest pain/palpitations/dyspnea  
- □ High fever/rigors or clear systemic deterioration  
- □ New/worsening headache or visual symptoms  
- □ Repeated elevated BP: e.g., **≥160/100 mmHg** repeatedly, or **≥140/90 mmHg** with symptoms (headache, palpitations, dizziness)  
- □ New neurological symptoms (even mild) that recur or worsen: numbness, weakness, diplopia, dysarthria, dysphagia  
- □ Exertional dyspnea or chest discomfort suggesting cardiac/pulmonary causes

### R3: Planned medical review (days to 2 weeks)
- □ Ongoing symptoms ≥4 weeks with functional impact (fatigue, post-exertional malaise, sleep disturbance, cognitive difficulties, headache)  
- □ Recurrent **orthostatic intolerance** (lightheadedness, palpitations when standing) suggesting dysautonomia (e.g., POTS/orthostatic hypotension)  
- □ Recurrent cough/breathlessness/chest discomfort (needs cardiopulmonary review)  
- □ Significant anxiety/depression/insomnia (coordinate mental health support with safety planning)

---

## 3. Documentation Template (Audit Trail)
- Main complaint:  
- Onset/course:  
- COVID history: □confirmed □suspected □unknown; date:  
- Past history (cardio/cerebrovascular/diabetes/kidney etc.):  
- Medications (antihypertensives, anticoagulants, steroids, etc.):  
- Red flags today: R1 □ / R2 □ / R3 □ (items: ________)  
- Actions taken: □EMS/ED □urgent clinic/doctor contact □referral letter/info □watchful waiting (reason:____)  
- Patient-facing explanation (key points):  
- Consent for sharing: □yes □no

---

## 4. Example Output (JSON contract)
**Case: long-COVID-like complaints + persistent dizziness + elevated BP**

De-identified patient info
- Age/sex: Male, 50s  
- Complaint: persistent dizziness  
- Vitals: BP 135/95 HR 79; BP 125/94 HR 89  
- Associated symptoms: no chest pain, no dyspnea, no focal neuro deficits (example)

AI output (organization only)
- Red flags detected (example)  
  - R2: repeated elevated BP (diastolic ≥90 mmHg) with persistent symptoms (dizziness)  
- Not detected (example)  
  - R1: no chest pain, dyspnea, altered consciousness, or clear stroke signs  
- Suggested next step (example)  
  - Prioritize medical evaluation and share vitals with a physician; reassess BP and consider further workup as indicated

Patient-facing explanation (draft)
“Your dizziness is ongoing and your blood pressure has been elevated on repeated readings. This is not necessarily an emergency, but it does warrant medical reassessment to confirm the blood pressure and check for causes.”

---

## References (examples)
- NICE. *COVID-19 rapid guideline: managing the long-term effects of COVID-19 (NG188).* (2020; updated 2024).  
- WHO. *Clinical case definition of post COVID-19 condition* (2021) and updates (2023).  
- CDC. *Long COVID: Signs and Symptoms* (2025).  
- CDC. *Signs and Symptoms of Stroke* (2024).  
- American Heart Association. *Home blood pressure monitoring / accurate BP measurement guidance* (2025).  
- Kario K, et al. Key points of the 2019 Japanese Society of Hypertension guidelines. *Hypertens Res.* 2019/2020.  
- StatPearls (NCBI Bookshelf). *Hypertensive Crisis* (2025).  
- NHS. *Heart attack – Symptoms*; *Pulmonary embolism – Symptoms* (public guidance).  
- StatPearls (NCBI Bookshelf). *Acute Pulmonary Embolism* (2024).

---

## License
- Suggested: CC BY 4.0 (adjust to your repository policy)
