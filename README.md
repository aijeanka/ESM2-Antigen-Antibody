# Antigen-Antibody Binding Prediction

## Overview
This project is part of a capstone at Argentys Informatics, focusing on **predicting antigen-antibody binding** using machine learning techniques. This prediction is based on sequence information, contributing to the broader field of in silico de novo antibody design. The goal is to aid in the development of antibody therapies for various diseases, such as cancer and autoimmune disorders.

## Project Goals
- Predict binding affinity between antigens and antibodies solely based on sequence information.
- Achieve high prediction accuracy using advanced machine learning models.
  
## Methods
- **Data Collection**: Utilized public databases documenting antibodies and nanobodies capable of binding to coronaviruses (e.g., SARS-CoV2, SARS-CoV1, and MERS-CoV), consisting of 12,916 entries.
- **Feature Extraction**: Converted amino acid sequences into token embeddings.
- **Modelling**: Employed ESM2, a state-of-the-art protein model for masked language modeling, leveraging around 65 million unique sequences.

## Results
- Achieved **89% accuracy** with an AUROC > 0.90.
- Model demonstrated high precision and was effective at classifying binding interactions, particularly with CDR3 regions and epitopes.

## Tools and Technologies
- **Data Sources**: CoV-AbDab database and other publicly available resources.
- **ML Models**: ESM2 for sequence processing, with Epitope and CDR3 region extraction tools.
- **Additional Tools**: AlphaFold3 for computationally intensive tasks in structure prediction.

## Discussion
- The project leverages open-source databases and tools for efficient data processing and model training.
- By focusing on specific protein regions (CDR3 and epitopes), the model achieves a higher level of accuracy with less data.

## Future Work
- Enhance the developability of predictions by integrating additional structure-function prediction tools.
- Optimize for computational efficiency in epitope extraction and antibody design.

## References
Key references include works from Lin et al. (2023) on ESM2 modeling, Raybould et al. (2021) on the CoV-AbDab database, and Huang et al. (2022) on antibody-antigen interaction prediction methods.

