# PolicySynth Lite 2.0 – Equity-Aware Policy Intelligence

PolicySynth Lite 2.0 is an AI-powered assistant that helps public-sector teams, nonprofits, and civic innovators rapidly understand a policy issue and generate equity-aware options.  
The system retrieves relevant information about a civic topic, summarizes it using large-language models (LLMs), and produces a structured, human-readable brief.

This prototype is inspired by the Burnes Center for Social Change’s **AI for Impact Program** and the **Policy Synth** initiative, which apply generative AI to make policymaking more evidence-based, transparent, and inclusive.

---

## Objectives
- Automate first-stage policy research and briefing  
- Embed equity and accessibility considerations in AI outputs  
- Demonstrate transparent LLM prompting and retrieval pipelines  
- Show how generative AI can support – not replace – human decision-making  

---

## Features
- **Topic-to-Brief Pipeline** – enter any civic topic and receive a structured summary  
- **Retrieval + Summarization** – gathers and condenses public data or sample documents  
- **Equity Lens** – highlights vulnerable populations and inclusion challenges  
- **Stakeholder Mapping** – surfaces agencies, NGOs, and community partners  
- **Policy Options Generator** – creates 2–3 actionable solutions with pros, cons, and equity notes  
- **Optional Streamlit Dashboard** – interactive interface for exploration  

---

## Tech Stack
Python | LangChain | OpenAI GPT-4 | FAISS | Streamlit | pandas | Requests | dotenv  

---

## Workflow
1. User enters a civic topic (for example, “food insecurity in Massachusetts”).  
2. The system retrieves or reads sample texts.  
3. Text is chunked and summarized via LLM.  
4. The model outputs a structured JSON brief containing:  
   - Issue summary  
   - Affected populations  
   - Key stakeholders  
   - 2–3 policy options with pros / cons  
   - Risks, data gaps, and next steps  
5. Results can be viewed or exported through the Streamlit dashboard.  

---

## Repository Contents
| File | Description |
|------|--------------|
| `PolicySynth_Lite_2_0.ipynb` | Google Colab notebook with complete workflow |
| `policysynth_app.py` | Streamlit interface for policy brief generation |
| `data/sample_sources/` | Optional folder with sample civic text files |
| `requirements.txt` | Python dependencies |

---

## Example Use Cases
- Drafting rapid policy briefs for city departments  
- Supporting student or fellowship product-based learning projects  
- Conducting quick landscape scans for nonprofits  
- Generating background context for grant proposals or policy memos  

---

## Responsible AI Considerations
- Outputs require human review and interpretation  
- Retrieval grounding mitigates hallucination risk  
- Bias and framing must be reviewed for fairness and inclusivity  
- API keys and credentials should remain private  

---

