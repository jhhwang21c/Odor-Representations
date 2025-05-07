# cortical-representations-odour-space

# Structure and flexibility in cortical representations of odour space 

## Authors
Stan L. Pashkovski, Giuliano Iurilli, David Brann, Daniel Chicharro, Kristen Drummey, Kevin M. Franks,Stefano Panzeri, &Sandeep Robert Datta†

†Corresponding author. Email: srdatta@hms.harvard.edu

## Abstract
The cortex organizes sensory information to enable discrimination and generalization. As systematic representations of chemical odour space have not yet been described in the olfactory cortex, it remains unclear how odour relationships are encoded to place chemically distinct but similar odours, such as lemon and orange, into perceptual categories, such as citrus. Here, by combining chemoinformatics and multiphoton imaging in the mouse, we show that both the piriform cortex and its sensory inputs from the olfactory bulb represent chemical odour relationships through correlated patterns of activity. However, cortical odour codes differ from those in the bulb: cortex more strongly clusters together representations for related odours, selectively rewrites pairwise odour relationships, and better matches odour perception. The bulb-to-cortex transformation depends on the associative network originating within the piriform cortex, and can be reshaped by passive odour experience. Thus, cortex actively builds a structured representation of chemical odour space that highlights odour relationships; this representation is similar across individuals but remains plastic, suggesting a means through which the olfactory system can assign related odour cues to common and yet personalized percepts.

## Manuscript

For more details, please see our manuscript [here](https://doi.org/10.1038/s41586-020-2451-1).

# Installation

## Requirements
1. Make a new conda env, e.g. `conda create -n piriform python=3.8`
2. Activate that env `conda activate piriform`.
3. Clone and enter this repo: `git clone git@github.com:dattalab/cortical-representations-odour-space.git && cd cortical-representations-odour-space`
4. To install the specific versions of packages used when testing the scripts in this repo you can do `pip install -r requirements.txt`. Alternatively, the minimal requirements for running the scripts and notebooks in this repo are:
```
pip install seaborn scikit-learn h5py tables
pip install jupyter notebook
```

## Supplementary data

1. Processed data files are hosted on Zenodo:
[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7754362.svg)](https://doi.org/10.5281/zenodo.7754362)

* Download `pseudopopulations.h5` and `chemical_descriptors.h5` from zenodo and add them to the [data](./data/) folder.

2. Data about the odor sets can be found [here](./data/odor_sets_with_cids.csv).

# Examples
Code to replicate key figures in [Pashkovski et al. 2020](https://doi.org/10.1038/s41586-020-2451-1). 

1. Open a new jupyter notebook with `jupyter notebook`.
2. Run the [notebooks](./notebooks). The notebooks should load the mean odor responses and calculate chemical and neural distance matrices.

# Contact
For more details on additional preprocessing steps or analyses, please consult the methods in our manuscript, post an issue here, or contact the authors.
# Odor-Representations
# Odor-Representations
