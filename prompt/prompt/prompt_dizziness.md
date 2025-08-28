# Dizziness / Vertigo Red Flag Checklist (Template)

**References:**  
- MSD Manual Professional Edition. *Dizziness and Vertigo: Red Flags.* Revised 2022.  
- HINTS exam literature for acute vestibular syndrome (Kattah JC, et al. Stroke. 2009).  
- NICE Clinical Knowledge Summaries: Vertigo and Dizziness.  

---

## Instructions
- For each patient presenting with dizziness/vertigo, mark **Yes / No** for each red flag item.  
- Positive findings require urgent or specialist referral.  
- AI only **organizes and summarizes** information; it does **not diagnose**.  
- Final decision must be made by the human clinician.  

---

## Red Flag Items

1. **Headache or neck pain with dizziness**  
   → Possible stroke, vertebral artery dissection, intracranial pathology  

2. **Gait ataxia or severe imbalance**  
   → Central vestibular lesion, cerebellar stroke  

3. **Loss of consciousness or syncope with dizziness**  
   → Cardiac arrhythmia, brainstem ischemia  

4. **Focal neurologic deficits** (weakness, diplopia, dysarthria, sensory loss)  
   → Central lesion (brainstem/cerebellum)  

5. **Severe symptoms lasting > 1 hour**  
   → Stroke, vestibular migraine, CNS infection  

6. **Sudden severe vertigo with new-onset hearing loss**  
   → Labyrinthitis, vestibular schwannoma, vascular event  

7. **Elderly with systemic risk factors** (anemia, hypotension, polypharmacy, cardiovascular disease)  
   → Higher likelihood of central or multifactorial causes  

---

## Input Fields
- Age / Sex  
- Symptom type (vertigo / lightheadedness / imbalance)  
- Onset and duration (seconds, minutes, hours, chronic)  
- Associated symptoms (hearing loss, tinnitus, headache, nausea, syncope)  
- Medical history (stroke risk factors, trauma, medications, systemic disease)  

---

## Example Output (JSON)

```json
{
  "red_flags": [
    "Gait ataxia with dizziness → possible cerebellar stroke",
    "Loss of consciousness → rule out brainstem ischemia or arrhythmia"
  ],
  "referral_triggers": [
    "Persistent vertigo > 1 week without improvement",
    "New hearing loss associated with dizziness"
  ],
  "refer_to": "Neurology / ENT / Emergency Department",
  "urgency": "urgent (same day referral)",
  "patient_message": "Some findings suggest a serious inner ear or brain cause. Immediate specialist evaluation is recommended.",
  "clinician_next_steps": "Perform basic neurological and ENT exam, consider HINTS test, arrange MRI or urgent referral."
}
