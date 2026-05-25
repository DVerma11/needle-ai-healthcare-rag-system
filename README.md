# NeedLE AI: Agentic RAG System for CMS Medical Coverage Decision Support

## Project Overview

NeedLE AI is a healthcare-focused Retrieval-Augmented Generation (RAG) and agentic AI system designed to assist with CMS National Coverage Determination (NCD) policy interpretation and medical coverage decision support.

The system integrates structured healthcare rules, vector-based policy retrieval, large language models, and LangGraph-based agent workflows to generate grounded and explainable coverage recommendations.

## Key Features

- Healthcare-focused RAG pipeline
- Agentic AI workflow using LangGraph
- CMS NCD policy retrieval
- CPT and ICD-10 validation
- Coverage determination support
- Structured evidence-based responses
- Hallucination mitigation strategies
- Prompt engineering guardrails
- Medical necessity assistance
- Explainable AI outputs

## Technologies Used

- Python
- LangGraph
- LangChain
- OpenAI API
- Vector Embeddings
- Retrieval-Augmented Generation (RAG)
- Healthcare NLP
- Pandas
- Jupyter Notebook

## Agent Workflow

The system uses a multi-agent workflow:

1. Input Normalization Agent
2. CPT/ICD Extraction
3. Retrieval Agent
4. Coverage Validation Agent
5. Evidence Verification
6. Final Response Generation

The workflow ensures grounded responses using retrieved CMS policy evidence.

## Data Sources

- CMS National Coverage Determination (NCD) Lab Manual
- CMS CPT–ICD Mapping Files
- ICD-10-CM datasets
- Structured CMS policy documents

## Example Query

Question:
Is CPT 84443 covered for ICD-10 E03.9?

Output:
- Coverage Decision
- Supporting Evidence
- Relevant NCD
- Required Documentation
- Confidence Assessment

## Healthcare Informatics Applications

This project demonstrates:
- Clinical decision support concepts
- Medical necessity workflow automation
- Healthcare policy retrieval
- AI-assisted coverage validation
- Explainable healthcare AI
- Agentic healthcare reasoning systems
