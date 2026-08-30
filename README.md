# AI-Assisted UX Testing and Co-Design for Academic Library Guides

This repository contains the sanitized codebase, prompting methodology, and synthesized visual outputs for my two-phase research project on academic library guide (LibGuides) optimization. 

By applying "vibe coding" approaches using Generative AI (**Google Gemini**) guided by the **CLEAR Framework** (Lo, 2023), I rapidly developed a 7-tab usability testing application with zero reliance on internal IT infrastructure.

---

## Key Features & Components

* **Phase 1: AI-Generated Usability Testing Tool**
  A custom split-screen usability testing interface built in Python using **Gradio** and deployed on **Hugging Face Spaces**. It incorporates embedded CSS styling, dynamic response clearing, and automated logging for performance evaluation across 7 key tasks.
* **Phase 2: Evidence-Based Co-Design & AI Prototyping**
  Quantitative usability gaps from Phase 1 were synthesized with qualitative card sorting (Zoom Whiteboard) to establish a 4-tiered information architecture. **Lovable** was then utilized for rapid web prototyping to transform the co-designed wireframe into a modernized library guide homepage interface.

---

## CLEAR Prompt Engineering Framework

Although stateless LLM chat sessions are not directly preserved, the technical pipeline strictly adhered to the **CLEAR Prompting Framework** (Lo, 2023):

* **Concise (C):** Targeted prompt boundaries framing the specific role (*expert Gradio developer*) and objective (*7-tab usability tool for library search*).
* **Logical (L):** Sequenced instructions moving from UI component placement to backend string validation logic, error logging, and deployment.
* **Explicit (E):** Strictly defined rules including embedded inline CSS, commented verification functions, and instant text field clearing upon task submission.
* **Adaptive (A):** Iterative prompt tuning to resolve UI responsiveness bugs and field state updates across tab switches.
* **Reflective (R):** Continuous feedback loops re-inputting runtime warning messages back into Gemini, achieving a **0% application crash rate** during user testing.

---

## Data Privacy & Anonymization

To comply with research ethics and protect user privacy:
* All Personally Identifiable Information (PII), such as Student IDs, has been strictly sanitized.
* Raw user records are dynamically mapped to randomized labels (`User_1`, `User_2`, etc.) prior to heatmap visualization.
* No raw student identity records are stored or exposed in this repository.

---

## Repository Structure

```text
├── README.md                          <- Project homepage & methodology overview
├── libguide_ux_testing_tool_PUBLIC.ipynb <- Executable Colab Notebook (Sanitized pipeline)
├── requirements.txt                   <- Python dependencies (gradio, pandas, seaborn, matplotlib)
└── sample_results/                    <- Sanitized Excel result examples & high-res heatmaps

---

## Live Application & Executable Code

* **Try the Live Interface:** [Hugging Face Spaces Interactive Demo](https://huggingface.co/spaces/cecilia1217/colab-upload)
* **Run in Colab:** [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Cecilia-Yuen/reviving-libguides-with-lean-ux/blob/main/libguide_ux_testing_tool_PUBLIC.ipynb)
