# Artifact Evaluation

This Jupyter notebook automates the process of gathering and filtering a dataset of System Management Mode (SMM) vulnerabilities from both vendor-specific advisories (Intel/AMD) and the global CVE List.

**Key Features:**
- **Vendor Scraping:** Automatically fetches the latest security advisory URLs from the official Intel and AMD security portals.
- **Keyword-Based Filtering:** Employs targeted regular expressions (e.g., "SMM", "SMRAM", "SMI handler") to identify advisories specifically related to System Management Mode.
- **CVE List Integration:** Clones the official CVE v5 repository and performs a deep recursive search through thousands of JSON records to identify SMM-specific vulnerabilities.
- **Structured Data Output:** Processes and aggregates the findings into a structured format (Pandas DataFrame), capturing essential fields such as CVE IDs, descriptions, assigners, and public dates for further analysis.

The Jupyter notebook provided will clone the CVE list and create a python virtual environment installing all the dependencies needed to run it, to recreate the results. This is achieved by running the first cell of the notebook.

