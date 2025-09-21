# AI-Redflag-Checklist

**AI-Redflag-Checklist** is a public repository of **AI-assisted prompts and checklists** for recognizing clinical red flags in primary care and allied health settings.  
The AI is used **only to structure and summarize information** — it does **not provide diagnoses**.  
All final decisions remain with human clinicians.

---

## Goals
- Support clinicians and allied health professionals in **organizing findings** related to red flags.  
- Improve communication with physicians by producing **structured outputs**.  
- Enable **safe AI-assisted documentation** without transferring diagnostic authority.  

---

## Available Checklists
- [Low Back Pain](https://github.com/KenjiroShiraishi/ai-redflag-checklist/blob/main/prompt/prompt/pmpt_low_back_pain_ja.md)  
  (12-item checklist, based on guidelines such as MINDS 2021, Chou et al. 2020)

- [Headache](https://github.com/KenjiroShiraishi/ai-redflag-checklist/blob/main/prompt/prompt/prompt_headache.md)  
  (thunderclap, meningitis, tumor, temporal arteritis, etc.)

- [Dizziness](https://github.com/KenjiroShiraishi/ai-redflag-checklist/blob/main/prompt/prompt/prompt_dizziness.md)  
  (anemia/bleeding-related red flags, posterior circulation issues)

- [Numbness / Paresthesia](https://github.com/KenjiroShiraishi/ai-redflag-checklist/blob/main/prompt/prompt/prompt_numbness.md)  
  (neurological referral indicators)

- [Kampo (Traditional Medicine) Internal Medicine Referral](https://github.com/KenjiroShiraishi/ai-redflag-checklist/blob/main/prompt/prompt/prompt_kampo_referral.md)  
  (for chronic multiple symptoms, polypharmacy, or patient preference when red flags are excluded)

👉 **Prompt Directory (all templates here):**  
https://github.com/KenjiroShiraishi/ai-redflag-checklist/tree/main/prompt/prompt

---

## Repository Structure
- `prompt/` : Prompt templates (low back pain, headache, dizziness, numbness, Kampo referral)  
- `templates/` : CSV data template, consent & disclosure form, minimal referral note  
- `docs/` : SOP, workflow description, and [Usage Rules](docs/usage_rules.md)  
- `examples/` : Anonymized outputs (PDF/JSON) for transparency  
- `result/` : [Clinical run logs](https://github.com/KenjiroShiraishi/ai-redflag-checklist/tree/main/result) — actual case records with input prompts and AI outputs (PDF/Markdown), anonymized and dated.  
  - Includes one case that led to a **hospital referral** (hypertension detection).  
  - Demonstrates real-world use, transparency, and reproducibility.  
- `LICENSE` : License text  

---

## Safety & Responsibility
- AI acts as an **information-organizing assistant**, not as a diagnostic system.  
- Human judgment is always required for referral decisions.  
- Written informed consent for case publication has been obtained from the patient in the referral case.  
- All other case prompts and outputs have been **fully anonymized**:  
  - Exact ages were generalized into ranges (e.g., "74 years" → "70s").  
  - Specific years of surgery or rare details were replaced with masked values (●●●).  
  - No direct identifiers (names, addresses, contact details) are ever included.  

---

## Reference
If you use or adapt this repository, please refer to:  
**OSF project hub:** https://osf.io/tghr6/  

---

## License
This project is released under the **Creative Commons Attribution-NonCommercial 4.0 International (CC BY-NC 4.0) License**.

You are free to:
- **Share** — copy and redistribute the material in any medium or format  
- **Adapt** — remix, transform, and build upon the material  
- **For non-commercial purposes only**

Under the following terms:
- **Attribution** — You must give appropriate credit, provide a link to the license, and indicate if changes were made.  
- **NonCommercial** — You may not use the material for commercial purposes without explicit permission from the author.  

Full license text: https://creativecommons.org/licenses/by-nc/4.0/

