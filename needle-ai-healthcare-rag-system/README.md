# NeedLE AI: Agentic RAG System for CMS Medical Coverage Decision Support

## Project Overview

NeedLE AI is a healthcare-focused Retrieval-Augmented Generation (RAG) and agentic AI system designed to assist with CMS National Coverage Determination (NCD) policy interpretation and medical coverage decision support.

The system integrates structured healthcare coverage rules, CMS policy retrieval, large language models, and LangGraph-based workflow orchestration to generate grounded, explainable coverage recommendations.

This project demonstrates how generative AI can be applied to medical necessity and coverage decision workflows while using guardrails to reduce hallucination and keep responses tied to retrieved CMS policy evidence.

---

## Key Features

- Healthcare-focused RAG pipeline
- CMS NCD policy retrieval
- CPT and ICD-10 extraction and validation
- Structured coverage decision support
- LangChain tool-based workflow
- LangGraph agentic workflow
- Evidence-grounded responses
- Guardrails for insufficient or missing information
- Explainable final answers with confidence scoring
- Demo queries and evaluation examples

---

## Technologies Used

- Python
- Jupyter Notebook / Google Colab
- LangChain
- LangGraph
- OpenAI API
- pandas
- NumPy
- PyPDF
- JSON
- CMS NCD policy files

---

## Repository Structure

```text
needle-ai-healthcare-rag-system/
│
├── README.md
├── requirements.txt
├── .gitignore
├── LICENSE
│
├── notebooks/
│   └── NeedLE_AI_CMS_Coverage_Assistant.ipynb
│
├── docs/
│   └── DATA_SOURCES.md
│
└── sample_outputs/
    └── coverage_examples.md
```

---

## Data Sources

This project was developed using CMS coverage-related resources, including:

- CMS National Coverage Determination (NCD) Manual
- CMS ICD-10 NCD coverage spreadsheet
- ICD-10-CM reference files
- CPT description reference files

Large CMS source files are **not included** in this repository. Users should download the files directly from CMS or use their own authorized local copies.

See [`docs/DATA_SOURCES.md`](docs/DATA_SOURCES.md) for details.

---

## How the System Works

The notebook follows this workflow:

1. Load CMS policy and structured coverage files
2. Parse NCD policy sections from PDF source material
3. Load CPT, ICD-10-CM, ICD-10-PCS, and reference datasets
4. Build policy retrieval functions
5. Integrate coverage rule validation with retrieved policy evidence
6. Build LangChain tools for coverage decision support
7. Create an agentic workflow using LangGraph
8. Run demo queries
9. Evaluate outputs and save results

---

## Example Use Case

Example question:

```text
Is CPT 84443 covered for ICD-10 E03.9 on 2026-01-01?
```

Expected output includes:

- Coverage decision
- CPT and ICD-10 interpretation
- Relevant NCD evidence
- Supporting policy explanation
- Confidence score
- Missing information if applicable

---

## Setup Instructions

### 1. Clone the repository

```bash
git clone https://github.com/YOUR-USERNAME/needle-ai-healthcare-rag-system.git
cd needle-ai-healthcare-rag-system
```

### 2. Install dependencies

```bash
pip install -r requirements.txt
```

### 3. Set your OpenAI API key securely

Do **not** hard-code API keys in the notebook.

Use one of the following methods:

```bash
export OPENAI_API_KEY="your_api_key_here"
```

or use Google Colab Secrets.

### 4. Add source data files

Place required CMS files in your local project folder or Google Drive path and update the notebook file paths accordingly.

---

## Security and Privacy Notes

- No PHI should be uploaded or used in this repository.
- API keys should never be committed to GitHub.
- Raw CMS source files and large local data files are excluded using `.gitignore`.
- The notebook included here has outputs cleared and hard-coded credentials removed.

---

## Limitations

This project is a prototype for educational and research purposes. It is not intended for direct clinical or claims adjudication use without additional validation, governance, and compliance review.

---

## Future Work

- Add a Streamlit or Gradio user interface
- Add automated CMS file download and update pipeline
- Improve structured CPT/ICD validation
- Add unit tests for coverage logic
- Add persistent vector database support
- Add audit logs for decision traceability
- Expand evaluation with more test cases

---

## Author

**Divya Verma**  
MS Health Informatics  
Rutgers University
