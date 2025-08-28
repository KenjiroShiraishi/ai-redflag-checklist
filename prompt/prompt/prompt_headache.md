# Headache Red Flag Checklist (Template)

**References:**  
- MSD Manual Professional Edition. *Red flag signs and causes of headache.* Updated 2021.  
- NICE Clinical Knowledge Summaries: Headache and Migraine.  
- American Academy of Neurology (AAN) guidelines on headache management.  

---

## Instructions
- For each patient presenting with headache, mark **Yes / No** for each red flag item.  
- Positive findings require urgent or specialist referral.  
- AI only **organizes and summarizes** information; it does **not diagnose**.  
- Final decisions must be made by the human clinician.  

---

## Red Flag Items

1. **Neurologic symptoms/signs** (altered mental status, confusion, focal deficits, diplopia, papilledema)  
   → Encephalitis, subdural hematoma, subarachnoid hemorrhage, venous sinus thrombosis, intracranial mass, raised intracranial pressure  

2. **Immunosuppression or malignancy history**  
   → CNS infection, metastasis  

3. **Signs of meningeal irritation** (neck stiffness, photophobia)  
   → Meningitis, subarachnoid hemorrhage, subdural abscess  

4. **New headache after age 50**  
   → Higher risk of serious cause (e.g., tumor, giant cell arteritis)  

5. **Thunderclap headache** (maximal intensity within seconds)  
   → Subarachnoid hemorrhage  

6. **Systemic symptoms** (fever, weight loss, visual loss, jaw claudication, temporal artery tenderness, proximal myalgia)  
   → Giant cell arteritis  

7. **Progressively worsening headache**  
   → Secondary headache (tumor, infection, hydrocephalus, etc.)  

8. **Ocular signs** (conjunctival injection, halos around lights)  
   → Acute angle-closure glaucoma  

---

## Input Fields
- Age / Sex  
- Headache onset and duration  
- Headache characteristics (sudden, progressive, chronic)  
- Associated symptoms (fever, vision changes, jaw claudication, neurologic deficits)  
- Medical history (cancer, immunosuppression, systemic disease)  

---

## Example Output (JSON)

```json
{
  "red_flags": [
    "Thunderclap headache → possible subarachnoid hemorrhage",
    "New headache after age 50 → possible temporal arteritis or tumor"
  ],
  "referral_triggers": [
    "Progressive worsening over several weeks"
  ],
  "refer_to": "Neurology / Emergency Department",
  "urgency": "emergent (immediate referral)",
  "patient_message": "This type of headache can sometimes indicate a serious condition such as bleeding or arteritis. Immediate specialist evaluation is recommended.",
  "clinician_next_steps": "Perform basic neuro exam, check ESR/CRP if arteritis suspected, arrange urgent referral."
}
