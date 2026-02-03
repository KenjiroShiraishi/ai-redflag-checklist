# Red Flag Checklist for Non-specific / Multi-system Symptoms — Template
(3-Layer Safety Gate / R1-R2-R3)

> **For**: Non-physician frontline practitioners to standardize “do-not-miss” danger signals  
> **Scope**: Non-specific complaints (dizziness, fatigue, palpitations, dyspnea, headache, insomnia, appetite loss, etc.) where the cause is not established. **Post-COVID/Long COVID may be included but this is not exclusive to it.**  
> **Principle**: AI is for **information organization only**; final decisions remain with humans.

---

## References (minimum set)
- NICE NG188: *COVID-19 rapid guideline: managing the long-term effects of COVID-19* (symptom-based assessment prioritizing exclusion of serious illness). https://www.nice.org.uk/guidance/ng188  
- CDC: *Signs and Symptoms of Stroke*. https://www.cdc.gov/stroke/signs-symptoms/  
- American Heart Association: *Monitoring your blood pressure at home* (measurement steps; 180/120 with symptoms = emergency). https://www.heart.org/en/health-topics/high-blood-pressure/understanding-blood-pressure-readings/monitoring-your-blood-pressure-at-home  
- StatPearls (NCBI Bookshelf): *Hypertensive Crisis*. https://www.ncbi.nlm.nih.gov/books/NBK507701/  
- NHS: *Heart attack symptoms* / *Pulmonary embolism*. https://www.nhs.uk/conditions/heart-attack/symptoms/ / https://www.nhs.uk/conditions/pulmonary-embolism/

---

## How to use
- Record **Yes/No** for each item.
- If any item is “Yes”, **prioritize safety** and consider urgent referral rather than proceeding with treatment.
- If vitals are available, record **BP/HR/SpO2/temperature** to support medical communication.

---

## Vitals (recommended)
- Date/time:  
- BP: 1st ____ / ____ mmHg, Pulse ____ /min  
- BP: 2nd ____ / ____ mmHg, Pulse ____ /min (repeat after 1–2 minutes)  
- SpO2: ____ % (if available)  
- Temperature: ____ °C  
- Posture: □seated □standing (note orthostatic worsening)

---

## Red flags (R1/R2/R3)

### R1: Emergency (any “YES” → EMS/ED)
- □ Severe shortness of breath at rest / cannot speak full sentences  
- □ Chest pain/pressure (diaphoresis, nausea, radiating pain, etc.)  
- □ Altered consciousness, seizure, syncope with injury  
- □ Possible stroke: facial droop, one-sided weakness/numbness, speech difficulty, sudden vision loss, sudden severe dizziness/ataxia  
- □ Sudden “worst headache” or neck stiffness  
- □ Marked SpO2 drop (clearly lower than usual, consistent with dyspnea)  
- □ Very high BP: roughly ≥180/120 mmHg WITH chest pain, dyspnea, neuro/visual symptoms, confusion  
- □ Suspected thromboembolism: sudden dyspnea + pleuritic chest pain/hemoptysis; or unilateral leg swelling/pain + respiratory symptoms

### R2: Urgent assessment (same day to 48 hours)
- □ Persistent/worsening dizziness/imbalance affecting walking (≥24 hours continuous or worsening)  
- □ New palpitations/irregular pulse with dizziness/presyncope  
- □ Recurrent syncope, or syncope with chest pain/palpitations/dyspnea  
- □ High fever/rigors or clear systemic deterioration  
- □ New/worsening headache or visual symptoms  
- □ Repeated elevated BP: e.g., ≥160/100 repeatedly, or ≥140/90 sustained with symptoms (headache, palpitations, dizziness)  
- □ New neurological symptoms that recur/worsen (numbness, weakness, diplopia, dysarthria, dysphagia)  
- □ Exertional dyspnea or chest discomfort suggesting cardiac/pulmonary causes

### R3: Planned medical review (days to 2 weeks)
- □ Ongoing symptoms ≥4 weeks with functional impairment  
- □ Recurrent orthostatic intolerance (lightheadedness/palpitations when standing)  
- □ Recurrent cough/dyspnea/chest discomfort (needs cardiopulmonary review)  
- □ Significant anxiety/depression/insomnia (coordinate mental health support with safety planning)

---

## Example output (JSON contract)
Case: persistent dizziness + elevated BP

**De-identified patient info**
- Male, 50s  
- Complaint: persistent dizziness  
- Vitals: BP 135/95 HR 79; BP 125/94 HR 89  
- No chest pain, no dyspnea, no focal neuro deficits (example)

**AI output (organization only)**
- detected_red_flags:
  - R2: repeated elevated BP (diastolic ≥90 mmHg) with persistent symptoms
- not_detected_red_flags:
  - R1: no chest pain, dyspnea, altered consciousness, or clear stroke signs (example)
- interpretation:
  - No clear emergency features, but persistent symptoms + repeated elevated diastolic BP warrant medical reassessment.
- recommendation:
  - Share vitals with a physician; confirm measurement conditions; repeat BP and consider further workup as indicated. Escalate to emergency care if R1 features appear.
- patient_explanation_draft:
  - “Your dizziness is ongoing and your blood pressure has been elevated on repeated readings. This is not necessarily an emergency, but it does warrant medical reassessment.”

**Final clinical decision (human)**
- Document actions and referrals.

