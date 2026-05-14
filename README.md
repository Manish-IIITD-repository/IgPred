# igpred: Prediction of Antibody Class-Specific B-cell Epitopes

Welcome to the official documentation for **igpred**, a computational method developed for predicting B-cell epitopes that induce specific classes of antibodies, such as IgG, IgE, or IgA. While traditional methods focus on general B-cell response, AbCpred provides functional insights into the type of humoral immunity a peptide will trigger, which is crucial for vaccine design and allergy research.

**Web Server:** [http://crdd.osdd.net/raghava/abcpred/](http://crdd.osdd.net/raghava/abcpred/)(https://webs.iiitd.edu.in/raghava/igpred)

---

## Citation

Gupta, S., Ansari, H. R., Gautam, A., & Raghava, G. P. S. (2013). 
**Identification of B-cell epitopes in an antigen for inducing specific class of antibodies.** *Biology Direct*, 8, 27. 
[https://doi.org/10.1186/1745-6150-8-27](https://doi.org/10.1186/1745-6150-8-27)

Zonedo:-(https://doi.org/10.5281/zenodo.20097037)

---

## About the Platform

The immune system generates different classes of antibodies (isotypes) to perform various effector functions. AbCpred is the first method designed to understand the relationship between the primary sequence of B-cell epitopes and the specific class of antibody they induce.

### Dataset Overview
The models were trained on a high-quality dataset derived from the Immune Epitope Database (IEDB):
* **IgG-specific epitopes**: 11,981 entries.
* **IgE-specific epitopes**: 2,341 entries.
* **IgA-specific epitopes**: 403 entries.
* **Non-B-cell epitopes**: 22,835 entries.

---

## Key Features

### Prediction and Classification
* **Class-Specific Prediction**: Predicts whether a peptide sequence is a B-cell epitope and identifies its antibody-inducing class (IgG, IgE, or IgA).
* **Amino Acid Analysis**: Utilizes observations that certain residues are preferred in different epitope classes (e.g., Cys in IgE epitopes; Pro and Gly in IgA epitopes).
* **Hybrid Models**: Employs Support Vector Machines (SVM) based on amino acid composition and dipeptide composition for high-accuracy classification.

### Performance Highlights
* **IgG vs. Non-B-cell**: Achieved a maximum accuracy of 74.59% using amino acid composition.
* **IgE vs. Non-B-cell**: Achieved a maximum accuracy of 83.21%.
* **IgA vs. Non-B-cell**: Achieved a maximum accuracy of 80.85%.

---

## Technical Overview

AbCpred leverages various sequence-based features to model the class-specific nature of B-cell epitopes.

* **Machine Learning**: Developed using SVM-light with various kernels (Linear, Polynomial, RBF, and Sigmoid) and validated through 5-fold cross-validation.
* **Feature Extraction**: Includes amino acid composition, dipeptide composition, and binary profile patterns.
* **Analysis Tools**: Provides insights into residue preference and positional conservation at the N and C terminals of epitopes.

---

## Applications

* **Vaccine Development**: Designing epitopes that selectively induce protective antibody classes like IgG or IgA.
* **Allergy Research**: Identifying IgE-inducing epitopes to understand and manage allergic reactions.
* **Immunology**: Understanding the fundamental sequence-level determinants of antibody isotype switching.

---

## Contact & Authors

**Prof. Gajendra P. S. Raghava** Bioinformatics Centre, CSIR-Institute of Microbial Technology, Chandigarh, India.  
**Email**: raghava@imtech.res.in

---

## License

This resource is open-access and distributed under the terms of the **Creative Commons Attribution License**, permitting unrestricted use and distribution provided the original work is properly credited.
