# Project Title: Automated PRISMA Diagram Generation for PubMed Searches using Gemini Model and Prompt Engineering

## Project Overview

This project aims to automate the process of generating PRISMA (Preferred Reporting Items for Systematic Reviews and Meta-Analyses) diagrams for systematic literature reviews using a Gemini Model. By leveraging prompt engineering, we will create a natural language pipeline that can effectively structure PubMed search results, apply user-defined inclusion/exclusion criteria, and output a PRISMA diagram along with a summary report, without the need for fine-tuning.

## Objectives

1. **Automate PRISMA Diagram Generation**: Simplify the process of visualizing systematic review search flows by generating accurate PRISMA diagrams directly from PubMed search data.
2. **Standardize Literature Qualification**: Use prompt-based filtering to apply user-provided inclusion and exclusion criteria to PubMed results, creating a standardized, repeatable qualification process.
3. **Streamline Summary Report Creation**: Provide an automated summary report to document key search results, inclusion/exclusion rationales, and a concise overview of eligible studies.

## Project Scope

- **Pipeline Development**:
   - **Search Execution**: The pipeline will accept a search string input for PubMed, execute the search, and retrieve available research articles.
   - **Inclusion/Exclusion Filtering**: Users will input specific criteria for inclusion and exclusion. The pipeline will apply these conditions, leveraging the Gemini Model to evaluate the relevance of retrieved articles based on the provided criteria.
   - **Data Summarization**: The Gemini Model will generate a summary of qualified articles that includes details about the study type, objectives, methods, and main findings.

- **PRISMA Diagram Generation**:
   - Convert the inclusion/exclusion filtering results into a structured PRISMA flow diagram.
   - Reflect each stage of the filtering process, from initial retrieval to final inclusion, in the PRISMA diagram.

## Methodology

1. **Prompt Engineering**: We will use prompt-based queries tailored to guide the Gemini Model in:
   - Interpreting user-defined criteria for inclusion and exclusion.
   - Evaluating each article's relevance to determine whether it qualifies.
   - Generating coherent and structured summaries of eligible studies.

2. **Data Processing Pipeline**:
   - **Search Stage**: The user provides a PubMed search string, which the pipeline processes and executes to retrieve available articles.
   - **Qualification Stage**: The pipeline interprets the inclusion/exclusion criteria through a series of prompts, filtering out non-qualifying studies.
   - **Diagram and Report Generation**: Eligible studies are counted and categorized to produce a visual PRISMA flow diagram and a summary report.

## Deliverables

1. **Automated PRISMA Diagram** for each PubMed search, reflecting the flow of eligible studies through the systematic review stages.
2. **Summary Report** that includes:
   - Number of articles retrieved, qualified, and included.
   - A summary of the final qualified studies, highlighting key insights aligned with PRISMA standards.
3. **Reproducible Code**: A Python-based pipeline with documented prompts for the Gemini Model and modular code to enable reproducibility and adaptability for other systematic review needs.

## Project Timeline

| Phase                  | Deliverables                     | Timeline       |
|------------------------|----------------------------------|----------------|
| **Phase 1**: Setup     | PubMed Integration, Prompt Design | 1 Weeks        |
| **Phase 2**: Filtering | Develop Criteria-Driven Filtering | 1 Weeks        |
| **Phase 3**: Diagram   | Automate PRISMA Diagram Creation  | 1 Weeks        |
| **Phase 4**: Testing   | Test and Validation               | 1 Week         |
| **Phase 5**: Finalize  | Summary Report, Documentation     | 1 Week         |

## Conclusion

By using a Gemini Model with prompt engineering, this project will streamline systematic review preparation, improving the accessibility and reliability of PRISMA diagrams and enabling researchers to focus on insights rather than manual qualification tasks.
