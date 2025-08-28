# AI-Redflag-Checklist

**AI-Redflag-Checklist** is a public repository of **AI-assisted prompts and checklists** for recognizing clinical red flags in primary care and allied health settings.  
The AI is used **only to structure and summarize information** — it does **not provide diagnoses**.  
All final decisions remain with human clinicians.

---

## Objectives
- Support clinicians and allied health professionals in **organizing findings** related to red flags.  
- Improve communication with physicians by producing **structured outputs**.  
- Enable **safe AI-assisted documentation** without transferring diagnostic authority.  

---
## Upcoming Prompts
The first release will include:

- [Low Back Pain](https://github.com/KenjiroShiraishi/ai-redflag-checklist/blob/main/prompt/prompt/pmpt_low_back_pain_ja.md)  
  (12-item checklist, based on guidelines such as MINDS 2021, Chou et al. 2020)

- [Headache](prompt/prompt_headache.md)  
  (red flag checklist: thunderclap, meningitis, tumor, temporal arteritis, etc.)

- [Dizziness](prompt/prompt_dizziness.md)  
  (including anemia/bleeding-related red flags, posterior circulation issues)

- [Numbness / Paresthesia](prompt/prompt_numbness.md)  
  (identify when neurological symptoms require orthopedic or neurology referral)

- [Kampo (Traditional Medicine) Internal Medicine Referral](prompt/prompt_kampo_referral.md)  
  (when red flags are excluded but multiple chronic symptoms, polypharmacy, or patient preference for Kampo-based approaches are present)

---

## Repository Structure
- `prompt/` : Prompt templates (low back pain, headache, dizziness, numbness, Kampo referral)  
- `templates/` : CSV data template, consent & disclosure form, minimal referral note  
- `docs/` : SOP, workflow description, and [Usage Rules](docs/usage_rules.md)  
- `examples/` : Anonymized outputs (PDF/JSON) for transparency  
- `LICENSE` : License text  

---

## Ethics & Governance
- AI acts as an **information-organizing assistant**, not as a diagnostic system.  
- Human judgment is always required for referral decisions.  
- Anonymized data and prompt/output PDFs can be shared via OSF for transparency.  

---

## Citation
If you use or adapt this repository, please cite:  
**OSF project hub:** https://osf.io/tghr6/  

---

## License
This project is released under the **Creative Commons Attribution 4.0 International (CC BY 4.0)** license.

You are free to:
- **Share** — copy and redistribute the material in any medium or format  
- **Adapt** — remix, transform, and build upon the material for any purpose, even commercially  

Under the following terms:
- **Attribution** — You must give appropriate credit, provide a link to the license, and indicate if changes were made.  

Full license text: [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/)
