# Usage Rules for AI-Redflag-Checklist (3-Layer Safety Gate)

This repository provides prompt templates to help clinicians organize clinical information about common symptoms (low back pain, headache, dizziness, numbness, etc.) using the **3-Layer Safety Gate (3LSG)**—a structured workflow designed to support safe triage, referral decisions, patient communication, and accountability.

---

## Purpose of the 3-Layer Safety Gate (3LSG)

The 3LSG is aligned with a simple 3-tier triage decision structure:

- **Gate 1 ↔ R1 (Immediate referral):** Red flag detection / danger-range screening  
- **Gate 2 ↔ R2 (Planned referral):** Gray zone clarification / borderline risk organization  
- **Gate 3 ↔ R3 (Local care, conditional):** Proceed-with-care management **with rapid-referral preparedness**  
  *(referral-ready notes, patient-facing message, and logging)*

### Gate Summary
- **Gate 1: Red Flag Detection (R1)**
- **Gate 2: Gray Zone Clarification (R2)**
- **Gate 3: Proceed-with-Care Management + Rapid-Referral Triggers (R3)**  
  *(referral-ready notes, patient-facing message, and logging)*

---

## ⚠️ Important Disclaimer

- **The AI does not diagnose.**
- The AI only **structures and summarizes** the information provided.
- All final decisions—including whether to refer, urgency level, and what to communicate—must be made by the **human clinician**.

---

# Workflow (3-Layer Safety Gate)

## Gate 1 (R1): Red Flag Check
Enter patient information into the relevant checklist prompt.  
If red flags are detected (e.g., cauda equina syndrome, sudden-onset neurological deficits, thunderclap headache) → **consider immediate referral / same-day medical evaluation (ED as needed)** and **stop intervention if appropriate**.  
If no red flags are detected, proceed to **Gate 2**.

---

## Gate 2 (R2): Gray Zone Organization
For cases without clear red flags but with uncertain findings or borderline concerns, the AI highlights these as **gray zones**.

**Examples:**
- Persistent symptoms without a clear cause
- Ambiguous neurological findings
- Non-specific systemic complaints

Gray zones are **not emergencies**, but they help clinicians decide whether **closer follow-up, further testing, co-management, or non-urgent referral** is appropriate.

---

## Gate 3 (R3): Proceed-with-Care Management + Rapid-Referral Triggers  
*(referral-ready notes, patient-facing message, and logging)*

For cases that do not meet R1/R2 criteria, the clinician may proceed with local care **conditionally**, while explicitly preparing a **rapid-referral plan**.

The AI supports this by structuring **referral-related notes** for clear, efficient communication with specialists, including:
- Which findings would justify referral
- What would make referral **urgent vs non-urgent**
- Key points to include in a referral letter / consultation note

In addition, Gate 3 emphasizes:
- **Rapid-referral triggers:** predefined “return-now / refer-now” warning signs
- **Patient-facing message:** clear instructions and safety-netting
- **Logging:** saving prompts/outputs for accountability

---

# Recommended Add-ons

## Patient Explanation (Patient-Facing Message)
The AI can draft a patient-friendly message explaining:
- Why referral or observation is recommended
- Why it is not urgent (if no red flags)
- Which warning signs require immediate re-evaluation

**Example:**  
“Your current findings are not life-threatening, but ongoing high blood pressure means it is safer to see an internal medicine specialist. Please go soon, and return immediately if chest pain or severe headache occurs.”

---

## Documentation (Logging)
- Save the input prompt and AI output as **PDF/JSON**.
- Add them to `examples/` to improve **transparency and reproducibility**.
- The clinician records the **final decision and rationale** in the patient’s chart.

---

# Example Use Case

**Case:** Male in his 60s with recurrent dizziness; no red flags, but persistent high blood pressure.

**AI Output (example):**
- `red_flags: []`
- `gray_zone: ["persistent hypertension"]`
- `referral: Internal Medicine`
- `urgency: non-emergent but necessary`
- `patient_message: "Your blood pressure is consistently high. It is not an emergency, but you should see an internal medicine doctor soon."`

**Clinician Decision:** Refer to internal medicine, with instructions to return immediately if neurological red flag symptoms appear.

---

# Key Principles

- **Red flags first** → minimum safety net (Gate 1 / R1).
- **Gray zones next** → avoid overlooking subtle risk (Gate 2 / R2).
- **Proceed with care, but prepare rapid referral** → conditional local care with safety-net triggers (Gate 3 / R3).
- **Patient explanation included** → transparency and trust.
- **Human final decision** → accountability.
