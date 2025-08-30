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

# Case Example: Low Back Pain with Red Flags

## Patient Information (Anonymized)
- Age: 80s, Female
- Chief Complaint: Severe low back pain (2 days duration)
- Trauma history: None
- Past history: Long-term corticosteroid use (prednisone)
- Systemic symptoms: No fever, no weight loss
- Neurological symptoms: No motor weakness, no bladder/bowel dysfunction
- Exam findings: Severe localized spinal tenderness, spontaneous pain

## AI Output (Prompt Summary)
Red Flags Detected:
- Age > 55
- Chronic corticosteroid use
- Severe localized spinal tenderness

No Red Flags Detected:
- No trauma history
- No fever, chills, or systemic illness
- No neurological deficit
- No cauda equina symptoms

**Interpretation:** Findings raise concern for vertebral compression fracture.  
**Recommendation:** Urgent referral to orthopedics for imaging and management.  

**Patient Explanation (AI draft):**  
"Because of your age, use of steroid medication, and the presence of strong localized spinal pain,  
we are concerned about a possible fracture in your back bones.  
It is important to have imaging and see an orthopedic specialist soon."

## Clinician Final Decision
- Action: Referral to orthopedics (same day).
- Outcome: Vertebral compression fracture diagnosed. Managed with appropriate medical care.
- Note: Minimal acupuncture treatment provided prior to referral. Patient was not harmed.

---

## Key Point
This case demonstrates how AI-assisted red flag checklists can help structure clinical reasoning.  
The AI did not make a diagnosis but highlighted risk factors, supporting timely referral and safe patient care.
