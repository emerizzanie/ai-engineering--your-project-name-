# Project Audit

**A RAG-based assistant that helps students review the responsible AI side of their AI projects**

Project Audit is my semester project for AI Engineering. A student describes their AI project and the system looks through public responsible AI guidelines. Which is to explain possible risks, show where the information came from and give a simple checklist to think about.

> This project is still at the planning stage (Week 1/2). Nothing is built yet, and this README will be updated later on.

---

## Problem Statement

When students build AI projects, they mostly focus on getting the model to work. Privacy, bias and trust in the output are often left until the end or forgotten.

Guidelines about these topics exist, but they are long which is written in general terms and spread across different documents. It hard for student to know which parts apply to their own project.

Project Audit tries to help by finding the relevant parts of the guidelines and explaining them in simple words with the source shown.

---

## Evidence of the Problem

- A scoping review in *AI & Society* found that responsible AI guidelines often have little effect in practice. Partly because the principles are too abstract. ([link](https://link.springer.com/article/10.1007/s00146-024-01880-9))
- Leça et al. (2024) interviewed software practitioners and found that some principles are like transparency and accountability and get less attention than others. ([link](https://arxiv.org/abs/2412.07620))
- A 2023 UNESCO survey found that fewer than 10% of the 450+ schools and universities in it had formal guidance on generative AI. ([link](https://www.unesco.org/en/articles/unesco-governments-must-quickly-regulate-generative-ai-schools))

I may look for student-focused evidence later.

---

## Related Work / Existing Approaches

| Existing work | What it does | Limitation |
|---|---|---|
| [NIST AI RMF 1.0](https://doi.org/10.6028/NIST.AI.100-1) | General framework for managing AI risks | Too general. Students must work out what applies to them |
| [Malaysia AIGE (2024)](https://mastic.mosti.gov.my/publication/the-national-guidelines-on-ai-governance-ethics/) | National guidelines with seven AI principles | Voluntary and general. Not interactive |
| [Let's have a chat with the EU AI Act](https://arxiv.org/abs/2505.11946) | RAG chatbot for checking systems against the EU AI Act | Focuses on EU law, not students or Malaysia |
| [gov-rag](https://github.com/rogerramos4/gov-rag) | RAG question answering over NIST AI RMF and EU AI Act | Answers questions only. No project review or checklist |
| [AI Governance & Compliance Assistant](https://github.com/Zaid0205/-AI_Governance_Assistant) | Classifies a described AI use case under EU AI Act risk levels | Mainly EU AI Act. Focused on classification, not learning |

This is a first search only. I will check for more similar tools later.

---

## Engineering Gap

The tools I found mostly focus on EU or US documents and on compliance. Project Audit tries to fill the gap by:

- being made for **students**, with simple explanations
- adding **Malaysian and ASEAN** guidance next to NIST
- taking a **project description** and giving a **checklist**
- being **tested properly**. Including a comparison with a normal LLM without retrieval

---

## Initial Project Objectives

1. **O1:** Collect and organise public responsible AI documents (NIST, Malaysia, ASEAN) for the assistant.
2. **O2:** Build a RAG assistant that explains possible risks in a student project, with source references and a simple checklist.
3. **O3:** Test retrieval relevance, answer correctness, citation accuracy and handling of questions the documents cannot answer and compare with a plain LLM.

---

## Target Users

- University students building AI or machine learning projects (main users)
- Student project teams
- Lecturers who want a starting point to discuss responsible AI

It is not made for professional compliance work.

---

## Proposed Data Sources

1. [NIST AI Risk Management Framework (AI 100-1)](https://doi.org/10.6028/NIST.AI.100-1)
2. [NIST Generative AI Profile (AI 600-1)](https://doi.org/10.6028/NIST.AI.600-1)
3. [Malaysia National Guidelines on AI Governance and Ethics](https://mastic.mosti.gov.my/publication/the-national-guidelines-on-ai-governance-ethics/)
4. [ASEAN Guide on AI Governance and Ethics](https://asean.org/wp-content/uploads/2024/02/ASEAN-Guide-on-AI-Governance-and-Ethics_beautified_201223_v2.pdf)
5. [UNESCO Guidance for Generative AI in Education and Research](https://unesdoc.unesco.org/ark:/48223/pf0000386693)

I will record the version and date of each document and check the terms of use before adding any file to this repo.

---

## Planned Tools (will change)

- **Language:** Python
- **Approach:** RAG (document processing, embeddings, vector search, LLM)
- **Interface:** Streamlit
- **Testing:** Python scripts and a set of manually checked questions

The exact libraries and LLM will be chosen later based on cost and availability.

---

## Weekly Progress

| Week | What I did / plan | Output | Status |
|------|-------------------|--------|--------|
| Week 1 | Chose the topic, wrote the project scope, set up the repo | README, project scope, observation sheet, system map | In progress |
| Week 2 | Requirements and system design | Requirements list and first architecture | Planned |
| Week 3 onwards | Build, test and evaluate | Code, experiments and results | Planned |

This plan is rough and will be updated each week.

---

## Limitations

Project Audit is for learning and a first review only. It cannot replace expert advice, it may miss risks, and it does not approve or certify any project.

---
