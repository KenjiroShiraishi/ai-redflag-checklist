# Mental Health Red Flag Check “Prompt” — Template
(3-Layer Safety Gate / R1-R2-R3)

> **For**: Non-physician frontline practitioners to standardize “do-not-miss” danger signals and connect people to urgent care  
> **Principle**: AI is for **information organization only**; final decisions and emergency actions remain with humans.  
> **Emergency**: Use your local emergency number (Japan: **119** for ambulance, **110** for police).

---

## References (minimum set)
- NICE **NG225**: *Self-harm: assessment, management and preventing recurrence*. https://www.nice.org.uk/guidance/ng225  
- NICE **CG178**: *Psychosis and schizophrenia in adults*. https://www.nice.org.uk/guidance/cg178  
- NICE **CG185**: *Bipolar disorder: assessment and management*. https://www.nice.org.uk/guidance/cg185  
- NICE **NG222**: *Depression in adults: treatment and management*. https://www.nice.org.uk/guidance/ng222  
- NICE **CG103**: *Delirium: prevention, diagnosis and management*. https://www.nice.org.uk/guidance/cg103  
- NICE **CG192**: *Antenatal and postnatal mental health*. https://www.nice.org.uk/guidance/cg192  
- WHO **mhGAP-IG v2.0** (non-specialized settings). https://iris.who.int/handle/10665/250239  
- Japan MHLW “Mamoru yo Kokoro” helplines (official list). https://www.mhlw.go.jp/mamorouyokokoro/soudan/tel/

---

## How to use (workflow)
1) Screen **R1 → R2 → R3** at the start of the visit (red flags override other decisions)  
2) If possible, record vitals and orientation (name/date/place)  
3) **R1**: do not leave the person alone; ensure safety; arrange emergency care  
4) **R2**: urgent clinical assessment within same day–48 hours  
5) **R3**: planned assessment within days–2 weeks + community supports  
6) Document findings, actions, and consent for sharing

> NG225 emphasizes not relying solely on scores/scales to “predict” suicide/self-harm risk; prioritize a collaborative safety-oriented conversation and linkage to care.

---

## Red flags (R1/R2/R3)

### R1: Emergency now (any “YES”)
**Self-harm / Suicide**
- □ **Imminent risk** (strong intent, specific plan, recent attempt, uncontrollable impulses)  
- □ **After an attempt** or with physical danger (bleeding, poisoning, injury)

**Psychosis / Agitation**
- □ Severe **hallucinations/delusions** with poor reality testing, or **command hallucinations** linked to harm  
- □ Severe agitation/violence risk (risk of harm to self/others)  
- □ Severe **mania** (extreme insomnia + disinhibited/risky behavior + impaired judgement) with inability to ensure safety

**Acute medical/substance-related change**
- □ Sudden confusion/disorientation with fluctuation (suspect **delirium**)  
- □ Fever + rigidity + altered mental status suggesting serious medication reactions (e.g., NMS/serotonin syndrome)  
- □ Acute intoxication or severe withdrawal (tremor, confusion, seizures, etc.)

**Perinatal**
- □ Within 1 year postpartum with acute psychotic symptoms, profound insomnia, or marked confusion (suspect postpartum psychosis)

---

### R2: Urgent assessment (same day–48 hours)
- □ Suicidal thoughts present but not clearly imminent (recurrent/worsening, limited supports)  
- □ Ongoing/recurrent self-harm  
- □ New hallucinations/delusions or marked paranoia  
- □ Suspected hypomania/mania (reduced sleep, irritability, risky spending/sexual behavior, increased activity)  
- □ Severe depression with marked functional decline, psychomotor retardation, profound hopelessness  
- □ Panic-like episodes with recurrent fainting/hyperventilation (needs medical exclusion as well)  
- □ Suspected eating disorder with physical risk (syncope, palpitations, chest pain, dehydration)  
- □ Suspected domestic violence/abuse/exploitation requiring safety planning and referral  
- □ Marked deterioration after medication changes/cessation (side effects/withdrawal/interactions)

---

### R3: Planned review (days–2 weeks) + community supports
- □ Persistent anxiety/depression/insomnia affecting daily function  
- □ Suspected substance use disorder requiring structured care  
- □ Trauma-related symptoms/dissociation/chronic stress response  
- □ Severe social isolation / lack of support resources

---

## Documentation template (audit trail)
- Main complaint (verbatim):  
- Duration/course:  
- Relevant history (psychiatric/medical):  
- Medications (antidepressants, antipsychotics, mood stabilizers, sedatives/benzodiazepines):  
- Substance use:  
- Orientation (name/date/place): □intact □uncertain  
- Red flags today: R1 □ / R2 □ / R3 □ (items: ________)  
- Actions: □EMS/ED □urgent clinic contact □family/support contact □helpline info □watchful waiting (reason:____)  
- Patient-facing explanation:  
- Consent for sharing: □yes □no

---

## Example output (JSON contract)
Case: worsening insomnia/anxiety with suicidal thoughts

AI output (organization only)
- detected_red_flags:
  - R2: suicidal thoughts (non-imminent–moderate), worsening insomnia, possible limited supports
- not_detected_red_flags:
  - R1: no recent attempt, no severe agitation, no clear delirium, no clear psychosis (example)
- interpretation:
  - Not clearly an immediate emergency, but urgent specialist assessment is indicated.
- recommendation:
  - Prioritize safety; avoid leaving the person alone; arrange same day–48h mental health/urgent care evaluation; connect to local helplines as appropriate.
- patient_explanation_draft:
  - “Because your sleep and distress have worsened and suicidal thoughts are present, it’s safest to have an urgent specialist assessment. Let’s connect you to the right support now.”

---

## Copy/paste: AI check prompt
Input the following, and ask the AI to output JSON for organization (not diagnosis).

**Inputs**
- Age/sex:  
- Complaint (verbatim):  
- Duration/course:  
- Self-harm/suicide: none / present (intent, plan, recent attempt):  
- Hallucinations/delusions: none / present (details):  
- Mania signs: none / present (sleep, activity, risky behavior):  
- Orientation: intact / uncertain  
- Substance use:  
- Medications / recent changes:  
- Safety concerns (violence, DV, abuse):  
- Actions already taken:  

**JSON outputs**
- detected_red_flags (label R1/R2/R3)
- not_detected_red_flags
- interpretation
- recommendation
- patient_explanation_draft

---

## License
- Suggested: CC BY 4.0 (adjust to your repository policy)
