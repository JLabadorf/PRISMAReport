# PubMed PICO Validation and PRISMA Flow Diagram

## Overview

This repository contains a collection of Python notebooks and scripts designed to automate the process of validating PubMed articles against a specified PICO (Population, Intervention, Comparison, Outcome) statement and generating PRISMA (Preferred Reporting Items for Systematic Reviews and Meta-Analyses) Flow Diagrams. Leveraging Vertex AI with Gemini Flash 1.5, the tools aim to streamline the systematic review process, enhance efficiency, and minimize manual effort in literature qualification.

## Features

- **PubMed Search and Store**: 
  - Search PubMed for articles based on a specified query.
  - Store essential metadata including title, authors, PubMed ID, DOI, abstract, and PDF URL (if available).
  
- **PICO Validation**:
  - Validate article relevance against a PICO statement using Gemini Flash 1.5.
  - Automate the first step of the PRISMA Flow Diagram by filtering articles based on user-defined criteria.

## Getting Started

### Prerequisites

To run the notebooks, ensure you have the following installed:

- Python 3.x
- Required Python libraries:
  - `requests`
  - `pandas`
  - `google-cloud-aiplatform` (for Vertex AI)
  
You can install the required libraries using pip:

```bash
pip install requests pandas google-cloud-aiplatform
```
### Setup

1.Clone the repository:

   ```bash
   git clone https://github.com/jlabadorf/PRISMAReport.git
   cd repo-name
   ```
2.  **Set up Google Cloud credentials for Vertex AI**:
   - Follow the [Google Cloud documentation](https://cloud.google.com/docs/authentication/getting-started) to set up your credentials.

3. **Open the notebooks** in Jupyter Notebook or any compatible environment to start using the tools.

## Usage

### 1. PubMed Search and Store

- Execute the notebook to search for articles in PubMed and store relevant metadata.
- Provide a search string to retrieve articles based on your criteria.

### 2. PICO Validation

- Open the PICO Validation notebook.
- Input the article title and abstract, along with your PICO statement.
- Run the notebook to validate whether each article matches the PICO criteria.

## Contributing

Contributions are welcome! If you have suggestions for improvements or want to report issues, please create an issue or submit a pull request.

## License

This project is licensed under the MIT License. See the LICENSE file for details.

## Contact

For questions or inquiries, please contact:

- **James Labadorf**
- **james@jameslabadorf.com**
- **www.jameslabadorf.com**
## Team Members

- *James Labadorf*: Prompt Engineering, Project Manager
- *Peter Labadorf*: Backend Design, Data Engineering

## Special Thanks To:
Rutgers School of Health Professions, where James is a doctoral student, and his advicor Dr. Barbara Tutfo who is guiding him this research for his dissertation.