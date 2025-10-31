PolicySynth Lite 2.0 – Equity-Aware Policy Intelligence

PolicySynth Lite 2.0 is a prototype AI assistant that helps public sector teams, nonprofits, and civic innovation labs rapidly understand a policy issue and generate equity-aware options. The tool takes a civic topic (for example, “food insecurity in Massachusetts” or “language access in Boston public services”), retrieves public information, summarizes it using LLMs, and produces a structured brief containing:
	•	issue summary
	•	key stakeholders
	•	affected / vulnerable populations
	•	possible interventions
	•	risks, constraints, and implementation notes

This project is inspired by the Burnes Center for Social Change’s AI for Impact program and the Policy Synth work, where AI is used to make policymaking more evidence-based, transparent, and human-centered.

Objectives
	•	Reduce time to first brief for policy analysts and student teams
	•	Make equity and inclusion an explicit part of AI-generated policy outputs
	•	Demonstrate transparent LLM prompting and retrieval for public sector use cases
	•	Show how generative AI can support, not replace, human decision-making

Features
	•	Topic-to-brief pipeline: enter a civic topic and generate a structured brief
	•	Retrieval + summarization: fetches public web content (or local sample docs) and summarizes it
	•	Equity lens: ensures vulnerable groups and language access are surfaced
	•	Stakeholder mapping: identifies government agencies, community-based organizations, and residents affected
	•	Policy options: generates 2–3 options with pros, cons, and equity impact notes
	•	Streamlit UI (optional): simple front-end to run the workflow

Tech Stack
	•	Python 3.x
	•	LangChain
	•	OpenAI API (or any LLM endpoint)
	•	Requests (for basic retrieval) or SerpAPI (optional)
	•	FAISS (optional, for local retrieval)
	•	Streamlit (optional UI)
	•	pandas

How It Works
	1.	User provides a topic: “paratransit accessibility for disabled riders in Massachusetts”
	2.	The system collects context (news, descriptions, or local markdown files)
	3.	Collected text is chunked and summarized using an LLM
	4.	A policy-brief prompt assembles:
	•	problem framing
	•	who is affected and how
	•	what public value is at stake
	•	2–3 implementable options
	•	risks and data gaps
	5.	Output is returned as structured JSON and rendered in UI

Files
	•	PolicySynth_Lite_2_0.ipynb – notebook with full pipeline
	•	policysynth_app.py – optional Streamlit app to run the workflow
	•	data/sample_sources/ – optional folder with sample civic texts
	•	requirements.txt – Python dependencies

Example Use Cases
	•	Drafting an initial brief for a city department
	•	Supporting a student product-based learning project
	•	Rapid landscape scan for a nonprofit partner
	•	Creating a starting point for a grant or RFP response

Responsible AI Notes
	•	Outputs must be reviewed by a human policy analyst
	•	Model hallucinations should be mitigated by retrieval and source display
	•	When working with vulnerable populations, add domain expert review
	•	Do not expose API keys in the notebook

Getting Started
	1.	Clone this repo
	2.	Create a .env file and add OPENAI_API_KEY=...
	3.	Run the notebook or streamlit run policysynth_app.py

Future Work
	•	Add named-entity recognition for agencies and legislation
	•	Add multilingual output for language-access policies
	•	Add confidence and source scoring
