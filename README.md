### End-to-End Automated NLP Tagging and Semantic Search System

In Misgrid, I designed and implemented a fully automated end-to-end system for intelligent tagging and semantic filtering powered by NLP.

Users can input natural language queries like:  
**"I'm looking for an ML engineer with Python and C++"**  
— and the system intelligently extracts relevant filters (e.g., roles, tools) using a custom language model.

The pipeline goes beyond static filtering:
1. **Dynamic Label Expansion** – During user creation, new tools or professions can be added. A validation model automatically checks whether the new label is relevant (e.g., accepts “C++”, rejects “flower”).
2. **Smart Query Mapping** – In the search interface, user queries are matched to existing filters using **cosine similarity** on embedded vectors, allowing for fuzzy and context-aware retrieval.
3. **Self-Updating Taxonomy** – The system continuously evolves by integrating valid user-generated labels, ensuring scalability while preserving data integrity.

🔍 **Try it live:** You can test how filter detection and semantic matching work here:  
[https://app.misgrid.com/projects](https://app.misgrid.com/projects)

This forms a closed-loop pipeline where **label creation, validation, query parsing, and semantic matching are entirely automated**, enabling intelligent user discovery at scale.
