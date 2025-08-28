# Low Back Pain Red Flag Checklist (Template)

**Source references:**  
- Chou R, et al. *Red Flags for Back Pain: A Systematic Review.* Ann Intern Med. 2020;173(5):350–361.  
- Verhagen AP, et al. *Red flags presented in current low back pain guidelines: a review.* Eur Spine J. 2016;25:2788–2802.  
- NICE Guideline NG59 (Low Back Pain and Sciatica, 2020 update).  
- Japanese Orthopaedic Association, *Low Back Pain Clinical Practice Guideline 2019* (for local comparison).  

---

## Instructions
- For each patient with low back pain, mark **Yes / No**.  
- Any positive response should trigger further evaluation and consideration of referral.  
- The AI assistant will only **organize and summarize** the findings — final judgment is by the human clinician.

---

## Red Flag Items

1. **Age <20 or >55** at onset → possible fracture, tumor, systemic disease  
2. **History of trauma** (fall, accident, heavy lift) → possible fracture  
3. **History of cancer, immunosuppression, steroid use, or HIV** → risk of malignancy or infection  
4. **Unexplained weight loss** → malignancy, infection  
5. **Fever, chills, systemic illness** → infection (osteomyelitis, discitis, epidural abscess)  
6. **Pain at rest or night pain** not relieved by position/activity → malignancy, infection, inflammatory disease  
7. **Chest pain, abdominal pulsation, or vascular risk** → aortic aneurysm/dissection  
8. **Progressive neurological deficit** (motor weakness, sensory loss) → nerve root compression, spinal cord lesion  
9. **Cauda equina symptoms** (urinary retention/incontinence, fecal incontinence, saddle anesthesia) → emergent referral  
10. **Widespread or severe neurological signs** (bilateral deficits, reflex changes) → central lesion  
11. **Structural spinal deformity** (kyphosis, scoliosis, collapse) → tumor, infection, fracture  
12. **Severe localized tenderness or swelling** over a vertebra → fracture, infection, tumor  

---

## Output Example (JSON Contract)

```json
{
  "red_flags_positive": ["Age >55", "Night pain not relieved"],
  "refer_to": "Orthopedics / Spine specialist",
  "urgency": "urgent",
  "reasons": [
    "Night pain without relief suggests possible tumor or infection",
    "Age over 55 increases risk of fracture or malignancy"
  ],
  "patient_message": "Because some findings raise concern for more serious conditions, we recommend you see an orthopedic specialist soon.",
  "clinician_next_steps": "Check neurological function (motor, sensory, reflexes), bladder/bowel status, document red flags, prepare referral note."
}
