# BUS5001 Assessment 3 – ESG Message Triage

## Project Overview

This project investigates the use of GPT-4o for classifying ESG-related operational messages, including environmental concerns, accessibility issues and supplier compliance risks.

The experiment was developed in Google Colab using Python and the OpenAI API.

## Methodology

1. Developed and refined ESG classification prompts.
2. Tested GPT-4o using five synthetic ESG messages.
3. Built a rule-based Python classifier as a baseline.
4. Compared classification results and investigated errors.
5. Validated structured JSON outputs before and after prompt refinement.
6. Evaluated limitations and proposed an Azure deployment architecture.

## Key Findings

- GPT-4o and the rule-based baseline achieved 100% agreement across 15 field-level comparisons on three original test messages.
- Challenge testing revealed limitations in the baseline's handling of resolved incidents and alternative wording.
- Prompt refinement improved schema compliance from 0/3 to 3/3 on the original messages, with 5/5 valid outputs across all V2 tests.
- Further testing, data protection and human oversight are necessary before production deployment.

## Repository Contents

- **Notebook:** Complete Python implementation and experiment.
- **results/:** Model outputs, comparison tables and validation results.
- **evidence/:** Screenshots of key experimental findings.

## Reproducibility

The notebook requires an authorised OpenAI API key, configured through Google Colab Secrets under `OPENAI_API_KEY`. No credentials are stored in this repository.

All test messages are synthetic and used for academic assessment purposes.

## Limitations

The evaluation uses five synthetic examples. The results demonstrate the prototype's behaviour but do not establish production-level reliability or fairness.
