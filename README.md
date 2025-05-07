# Structured and Distributed Odor Representations in the Piriform Cortex

**Authors**: John Hwang, Ivanna Garibay  
**Course**: Harvard Neuro 120

## Abstract

The mouse piriform cortex enables odor discrimination using a limited number of broadly tuned neurons. To investigate whether odor representations in this circuit are sparse or distributed, we analyzed calcium imaging data from layers 2 and 3 during passive exposure to three structured odor sets (global, tiled, clustered). Lifetime and population sparseness measures (means = 0.82 and 0.93, respectively) indicated high selectivity and low coding density. Hierarchical clustering revealed compact representations in clustered L3, while decoding analyses showed that accuracy increased with more neurons, supporting distributed but sparse coding. Logistic regression classifiers achieved perfect accuracy in global L3 but dropped to ~80% in TeLC conditions, highlighting the role of recurrent connectivity. L2 maintained high-dimensional, chemically structured responses, while L3 representations were more compact and generalized. Together, these results suggest that the piriform cortex encodes odors via sparse, overlapping populations shaped by recurrence, transitioning from fine discrimination in L2 to abstraction in L3.

## Project Overview

This repository contains code and analyses for evaluating how neural population coding in the piriform cortex supports odor discrimination. It replicates and extends methods from:

> Pashkovski et al. (2020). _Structure and flexibility in cortical representations of odour space_. Nature, 583(7815), 253–258.  
> https://doi.org/10.1038/s41586-020-2451-1

## Key Analyses

-   **Neuron Exclusion Decoding**: Test how decoding accuracy changes as high-sparseness or high-response neurons are excluded.
-   **Sparseness Metrics**: Compute lifetime and population sparseness to quantify selectivity and coding density.
-   **Hierarchical Clustering & Silhouette Scores**: Evaluate how odors cluster in neural representation space.
-   **Layer & Manipulation Comparisons**: Compare L2 vs. L3 and the effects of TeLC manipulation across three odor sets.

## File Structure

-   `final_code.ipynb`: Main analysis notebook.
-   `data/`: Folder containing required files:
    -   `pseudopopulations.h5`: Neural responses (trials × ROIs × odors).
    -   `chemical_descriptors.h5`: Odor feature vectors.
    -   `odor_sets_with_cids.csv`: Odor set and CID mapping.
    -   `intuitive_descriptors.csv`: Curated list of top-ranked chemical features including name, description, and source type
-   `LICENSE`: MIT License.
-   `README.md`: Project description and usage instructions.

## Running the Notebook

1. Clone this repository and place data files in the `data/` directory.
2. Open the notebook:
    ```bash
    jupyter notebook final_code.ipynb
    ```
