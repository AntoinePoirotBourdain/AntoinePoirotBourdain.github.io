---
layout: archive
title: "Research"
permalink: /research/
author_profile: true

---

{% include base_path %}


## Survival Analysis for Pharmacovigilence

Adverse drug reactions are a major public health issue. They are currently detected by The project aims to use the Weighted Cumulated Exposure (WCE) model on SNDS data to search for ADR in a large scale without a priori hypothesis. This large scale screening is made possible due to the implementation of the WCE (and coxPH) model on the survivalGPU lirbary

One important part of the project is tu use the computing power offered by GPUs to calibrate the WCE model to find out if it is applicacable for large scale ADR screening and on which conditions. The model will be compared to the ConvSCCS model. 

Then the model will be tested on real SNDS data to validate it's efficiency in a real situation. 


## GPU acceleration of algorithms

Contribution to the survivalGPU library by implementing new algorithms. There are two alogithms that are under implementation

- The permutation algorithm : an algorithm that simulate survival analysis data and was used to validate the WCE algorithm that we use to detect adverse drug reactions. 
- ConvSCCS : a self controlled based on a convolution Poisson regression that is currently implemented in the tick library

The reimplementation of the algorithms using GPUs will be done using torch and the pyKeops library.
