#### PROJECT DOCUMENT: Automated PRISMA Diagram Generation for PubMed Searches using Gemini Model and Prompt Engineering

**For the Kaggle Competition:  Stress Testing Gemini 1.5's Long Context Window**

**Project Overview:**

This project leverages the Gemini 1.5 model's expansive context window (up to 2 million tokens) to automate PRISMA (Preferred Reporting Items for Systematic Reviews and Meta-Analyses) diagram generation for systematic literature reviews. By using prompt engineering, we create a natural language pipeline that processes large volumes of PubMed search results, applies user-defined inclusion/exclusion criteria, and outputs a PRISMA diagram and summary report without fine-tuning. This approach eliminates the need for traditional context management techniques like vector databases or RAG, demonstrating a compelling use case for Gemini 1.5's capabilities.

**Objectives:**

* **Automate PRISMA Diagram Generation:** Simplify and accelerate the visualization of systematic review search flows.
* **Standardize Literature Qualification:**  Implement a standardized and repeatable qualification process using prompt-based filtering with user-specified inclusion/exclusion criteria.
* **Streamline Summary Report Creation:**  Automate the generation of a comprehensive summary report documenting search results, inclusion/exclusion rationale, and an overview of eligible studies.
* **Demonstrate Long Context Window Advantage:** Showcase the power of Gemini 1.5's extended context window by processing extensive PubMed search results directly, eliminating reliance on external context management techniques.


**Project Scope:**

* **Pipeline Development:**
    * **Search Execution:**  Accept PubMed search strings and retrieve large result sets (demonstrating >100,000 token processing). Discussion on handling potential rate limiting and optimizing search strategy within the context window will be included.
    * **Inclusion/Exclusion Filtering:** Process inclusion/exclusion criteria provided by users, using the Gemini model and prompt engineering to evaluate and filter retrieved articles *within its large context window*.
    * **Data Summarization:**  Generate summaries of eligible studies including study type, objectives, methods, and key findings – all within the model's context.
* **PRISMA Diagram Generation:** Convert filtering results into a structured PRISMA flow diagram visualizing the stages of the systematic review process.
* **Context Caching Demonstration:** Explore and utilize Gemini 1.5's context caching functionality to optimize the efficiency of processing large search results.



**Methodology:**

* **Prompt Engineering:** Craft tailored prompts to guide the Gemini model in interpreting user criteria, evaluating article relevance, and generating structured study summaries within its extensive context window.
* **Data Processing Pipeline:**
    * **Search Stage:**  Retrieve large volumes of PubMed articles via the provided search string.  The advantages of using the large context window for this step, compared to alternative approaches, will be documented.
    * **Qualification Stage:**  Filter studies according to user criteria *directly within the context window*, demonstrating efficient use of the expanded context.
    * **Diagram and Report Generation:** Generate PRISMA diagram and summary report based on the qualified studies.
* **Context Caching:**  The notebook will explicitly demonstrate the use and benefit of context caching, showcasing how previously processed context is reused for subsequent tasks within the pipeline, leading to increased efficiency.


**Deliverables:**

* **Automated PRISMA Diagram:**  A visually informative diagram representing the study selection process.
* **Summary Report:** Including retrieved, qualified, and included study counts, along with summaries of eligible studies adhering to PRISMA standards.
* **Reproducible Kaggle Notebook:** A well-documented Python notebook illustrating the pipeline, prompt engineering techniques, context caching strategy, and the advantages of using Gemini 1.5’s large context window, attached to this competition.
* **Public Dataset:**  A Kaggle dataset containing example PubMed search results and accompanying data. This dataset will showcase the volume of data being processed within the Gemini context window.
* **YouTube Video:** A concise (<5 minute) video summarizing the project, explaining the role of the large context window and context caching, demonstrating the results, and serving as an educational resource for other Gemini 1.5 users.


**Project Timeline:**

* **Phase 1: Setup & Data Preparation:** PubMed API integration, Dataset Creation, Prompt Design (Week 1)
* **Phase 2: Long Context Filtering:** Implement Criteria-Driven Filtering within the Large Context Window (Week 2)
* **Phase 3: PRISMA Diagram Generation & Context Caching:** Automate Diagram Creation, Implement and Document Context Caching (Week 3)
* **Phase 4: Testing and Refinement:** Validation and optimization for efficiency (Week 4)
* **Phase 5: Documentation, Video Creation & Submission:** Finalize Notebook, Create YouTube Video, Prepare Competition Submission (Week 5)

**Conclusion:**

This project will showcase the innovative use of Gemini 1.5's long context window for a complex real-world application. By demonstrating the ability to process and analyze extensive PubMed search data directly within the model's context, this project contributes to a better understanding of the potential of large language models for streamlining complex research tasks and ultimately improving the accessibility and efficiency of systematic reviews.
