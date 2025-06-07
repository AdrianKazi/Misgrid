### NLP-Based Automated Labeling and Search System

I developed an NLP-powered system in Misgrid that allows users to search using natural language queries like:  
**"I look for an ML engineer with Python and C++"**  
The model automatically detects and maps the query to available filters (e.g., roles, tools).

When adding new users, the system allows them to create new tools or professions that don't yet exist in the database. A separate model checks whether the newly added label is valid — for example, adding "C++" is accepted, while something like "flower" is rejected.

In the search filter list, I use cosine similarity to match user queries with relevant labels, enabling fuzzy and semantic search.

This results in a fully automated system for adding, validating, and searching labels using NLP and vector similarity.
