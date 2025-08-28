# Numbness / Paresthesia Red Flag Checklist (Template)

**References:**  
- MSD Manual Professional Edition. *Numbness.* Updated 2021.  
- Chou R, et al. *Red Flags for Back Pain: A Systematic Review.* Ann Intern Med. 2020;173(5):350–361.  
- Verhagen AP, et al. *Red flags presented in current low back pain guidelines: a review.* Eur Spine J. 2016;25:2788–2802.  
- NICE Clinical Knowledge Summaries: Sciatica and Neurological Symptoms.  
- American Academy of Neurology (AAN) practice parameters.  

---

## Instructions
- For each patient presenting with numbness/paresthesia, mark **Yes / No**.  
- Positive findings indicate urgent or specialist referral is required.  
- AI acts only to **organize information**, not to diagnose.  
- Final decision must be made by the human clinician.

---

## Red Flag Items

1. **Sudden onset numbness** (minutes to hours) → Suspect stroke, acute ischemia  
2. **Rapidly progressive weakness with numbness** (hours to days) → Nerve root compression, demyelinating disease  
3. **Numbness with respiratory difficulty** → Guillain-Barré syndrome or severe neuromuscular disease  
4. **Cauda equina signs** (saddle anesthesia, urinary retention/incontinence, fecal incontinence, sphincter dysfunction)  
5. **Bilateral numbness below a specific spinal level** → Transverse myelopathy, spinal cord lesion  
6. **Concurrent numbness in face + trunk/extremities** → Brainstem or central lesion  
7. **Symmetrical “glove and stocking” numbness with motor impairment** → Diabetic neuropathy, toxic/metabolic polyneuropathy, multiple sclerosis  
8. **New numbness with serious comorbidities** (cancer, diabetes, HIV, RA, immunosuppression)  

---

## Input Fields
- Age / Sex  
- Symptom location and distribution  
- Onset speed (sudden, subacute, chronic)  
- Associated symptoms (weakness, bladder/bowel dysfunction, respiratory difficulty)  
- Medical history (cancer, diabetes, immunosuppression, infection risk)  

---

## Example Output (JSON)

```json
{
  "red_flags": [
    "Rapidly progressive weakness with numbness → possible cord compression",
    "Cauda equina signs present"
  ],
  "referral_triggers": [
    "Persistent numbness despite therapy",
    "Functional impairment (grip weakness)"
  ],
  "refer_to": "Neurology / Orthopedics",
  "urgency": "urgent (within days)",
  "patient_message": "Some findings suggest a risk of serious neurological conditions. Please see a specialist promptly.",
  "clinician_next_steps": "Document neurological findings, order MRI, prepare referral note."
}
