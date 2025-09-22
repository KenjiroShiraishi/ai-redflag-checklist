# Usage Rules for AI-Redflag-Checklist

This repository provides **prompt templates** to help clinicians organize clinical information about common symptoms (low back pain, headache, dizziness, numbness, etc.) and structure their reasoning process through:  
1. **Red flag detection**  
2. **Gray zone clarification**  
3. **Referral information organization**

⚠️ **Important Disclaimer**  
- The AI **does not diagnose**.  
- The AI **only organizes and summarizes input information**.  
- All final decisions, including whether to refer to a specialist, must be made by the **human clinician**.  

---

## Workflow

### Step 1: Red Flag Check
- Enter patient information into the relevant checklist prompt.  
- If **red flags are detected** (e.g., cauda equina, sudden-onset neurological deficits, thunderclap headache) → **immediate referral**.  
- If **no red flags**, proceed to Step 2.  

### Step 2: Gray Zone Organization
- For cases without red flags but with **uncertain findings or borderline concerns**, the AI highlights these as **gray zones**.  
- Examples:  
  - Persistent symptoms without clear cause  
  - Ambiguous neurological findings  
  - Non-specific systemic complaints  
- These gray zones are not emergencies, but they help clinicians decide whether close follow-up or further testing is needed.  

### Step 3: Referral Information
- The AI structures **referral-related notes**, such as:  
  - Which findings justify referral  
  - Whether the referral is urgent or non-urgent  
  - Key points to include in a referral letter  
- This ensures smoother communication with specialists.  

### Step 4: Patient Explanation
- The AI can draft a **patient-friendly message** explaining:  
  - Why referral or observation is recommended  
  - Why it is not urgent (if no red flags)  
  - What warning signs require immediate re-evaluation  

Example:  
*“Your current findings are not life-threatening, but ongoing high blood pressure means it is safer to see an internal medicine specialist. Please go soon, and return immediately if chest pain or severe headache occurs.”*  

### Step 5: Documentation
- Save the input prompt and AI output as a PDF/JSON.  
- Add to `examples/` for transparency and reproducibility.  
- Clinician records the **final decision** in the patient’s chart.  

---

## Example Use Case
- **Case:** 60s male, recurrent dizziness, no red flags, but persistent high blood pressure.  
- **AI Output:**  
  - `red_flags: []`  
  - `gray_zone: ["persistent hypertension"]`  
  - `referral: Internal Medicine`  
  - `urgency: non-emergent but necessary`  
  - `patient_message: "Your blood pressure is consistently high. It is not an emergency, but you should see an internal medicine doctor soon."`  
- **Clinician Decision:** Referral to internal medicine, with instructions to return immediately if neurological red flag symptoms appear.  

---

## Key Principles
- **Red flags first** → minimum safety net.  
- **Gray zones next** → avoid overlooking subtle risks.  
- **Referral information structured** → clear communication with specialists.  
- **Patient explanation always included** → transparency and trust.  
- **Human final decision** → accountability.  

