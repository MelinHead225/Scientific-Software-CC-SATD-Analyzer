# Scientific-Software-CC-SATD-Analyzer

This repository is an artifact from the research paper: 

Exploring Scientific Debt: Harnessing AI for SATD Identification in
Scientific Software.

Context: Developers often leave behind clues in their code, admitting where it falls
short, known as Self-Admitted Technical Debt (SATD). In the world of Scientific Software (SSW),
where innovation moves fast and collaboration is key, such debt is not just common but deeply im-
pactful. As research relies on accurate and reproducible results, accumulating SATD can threaten
the very foundations of scientific discovery. Yet, despite its significance, the relationship between
SATD and SSW remains largely unexplored, leaving a crucial gap in understanding how to
manage SATD in this critical domain. Objective: This study explores SATD in SSW repos-
itories, comparing SATD in scientific vs. general-purpose open-source software and evaluating
transformer-based models for SATD identification. Method: We analyzed SATD in 27 scien-
tific and general-purpose repositories across multiple domains and languages. We fine-tuned and
compared 10 transformer-based models (100M–7B parameters) on 67,066 labeled code comments.
Results: SSW contains 9.25x more Scientific Debt and 4.93x more SATD than general-purpose
software due to complex computations, domain constraints, and evolving research needs. Further-
more, our best model outperforms existing ones. Conclusions: This study uncovers how SATD
in SSW differs from general software, revealing its impact on quality and scientific validity. By
recognizing these challenges, developers and researchers can adopt smarter strategies to manage
debt and safeguard the integrity of scientific discovery.

The notebook ```SSW_SATD_Analyzer.ipynb``` is a script that leverages a fine-tuned version of BERT-large for identifying SATD source code comments in scientific software. To use simply replace the line ```"https://github.com/healpy/healpy.git"``` in the notebook with your selected github repository that you would like to analyze. The script will then output relevant information pertaining to SATD in the respository along with saving a CSV file with all identified SATD instances and file paths.

For any questions or inquires please reach out to ericmelin@u.boisestate.edu.
