# Usage Rules for AI-Redflag-Checklist

This repository provides **prompt templates** to help clinicians organize clinical information about common symptoms (low back pain, headache, dizziness, numbness, etc.) and identify possible **red flags** or **referral triggers**.

⚠️ **Important Disclaimer**  
- The AI **does not diagnose**.  
- The AI **only organizes and summarizes input information**.  
- All final decisions, including whether to refer to a specialist, must be made by the **human clinician**.  

---

## Workflow

### Step 1: Red Flag Detection
- Enter patient information into the relevant checklist prompt.  
- If **red flags are detected** (e.g., cauda equina, sudden-onset neurological deficits, thunderclap headache), → **immediate referral**.  
- If **no red flags**, proceed to Step 2.

### Step 2: Referral Triggers
- Add examination findings or persistent symptoms (e.g., **SLR positive**, **progressive weakness**, **no improvement with therapy**).  
- The AI will highlight these as **“referral triggers.”**  
- These are not emergencies, but reasons to advise specialist referral.

### Step 3: Patient Explanation
- The AI can draft a **patient-friendly message** explaining:  
  - Why referral is recommended  
  - Why it is not urgent (if no red flags)  
  - What signs/symptoms require urgent re-evaluation  
- Example:  
  *“Your symptoms are not life-threatening, but the positive SLR test suggests a pinched nerve. An orthopedic consultation can confirm this and prevent worsening.”*

### Step 4: Documentation
- Save the input prompt and AI output as a PDF/JSON.  
- Add to `examples/` for transparency and reproducibility.  
- Clinician records the **final decision** in the patient’s chart.

---

## Example Use Case
- **Case:** 40-year-old male, leg numbness, SLR positive, no red flags.  
- **AI Output:**  
  - `red_flags: []`  
  - `referral_triggers: ["SLR positive suggests possible lumbar disc herniation"]`  
  - `refer_to: Orthopedics`  
  - `urgency: non-emergent but timely`  
  - `patient_message: "Not an emergency, but seeing an orthopedic specialist soon is recommended."`  
- **Clinician Decision:** Referral to orthopedics, with instructions to return immediately if red flag symptoms develop.

---

## Key Principles
- **Red flags first** → safety.  
- **Referral triggers second** → thoroughness.  
- **Patient explanation always included** → transparency and trust.  
- **Human final decision** → accountability.
