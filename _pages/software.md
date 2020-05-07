---
title: "CoNI Lab - Software"
layout: textlay
excerpt: "Software"
sitemap: false
permalink: /software
---

# Software

We have a track record of developing software for brain image
processing and analysis.

[FSL](#fsl-toolboxes), [HCP WM Atlases](#hcp-white-matter-atlases), [CUDIMOT](#cudimot), [NMF-mapper](#nmf-for-data-driven-mapping-of-structural-connections),
[Pipelines and Data](#processing-pipelines-and-data)


### FSL Toolboxes
<figure>
<img src="{{ site.url }}{{ site.baseurl }}/images/software/FSL_logo.jpg" width="15%">
</figure>

We have led the development or contributed to a number of toolboxes that are publicly released through [FSL](https://fsl.fmrib.ox.ac.uk/fsl/fslwiki){:target="_blank"}, one of the
de-facto software standards for multi-modal neuroimage processing,
used by thousands of researchers in hundreds of institutions
worldwide. These include:
* [XTRACT](https://fsl.fmrib.ox.ac.uk/fsl/fslwiki/XTRACT){:target="_blank"},
  for automated tractography in the human and non-human primate brain
* [Bedpostx / Bedpostx_gpu](https://fsl.fmrib.ox.ac.uk/fsl/fslwiki/FDT/UserGuide#BEDPOSTX){:target="_blank"},
  for Bayesian estimation of WM fibre orientations from diffusion MRI
  data using a number of forward models
* [Qboot](https://fsl.fmrib.ox.ac.uk/fsl/fslwiki/FDT/UserGuide#qboot_-_Estimation_of_fibre_orientations_using_q-ball_ODFs_and_residual_bootstrap){:target="_blank"} for stochastic estimation of diffusion and fibre ODFs from diffusion MRI data
* [Probtrackx / Probtrackx_gpu](https://fsl.fmrib.ox.ac.uk/fsl/fslwiki/FDT/UserGuide#PROBTRACKX_-_probabilistic_tracking_with_crossing_fibres){:target="_blank"} for probabilistic tractography, connectivity fingerprinting and mapping
* [Eddy](https://fsl.fmrib.ox.ac.uk/fsl/fslwiki/eddy){:target="_blank"}
for distortion, outlier, motion correction
* [Eddyqc](https://fsl.fmrib.ox.ac.uk/fsl/fslwiki/eddyqc/UsersGuide){:target="_blank"}
  for quality control and assessment of diffusion MRI data.

<hr>

### HCP White Matter Atlases

<figure>
<img src="{{ site.url }}{{ site.baseurl }}/images/software/hcp_wm.jpg" width="15%">
</figure>
<hr>


### CUDIMOT
<figure>
<img src="{{ site.url }}{{ site.baseurl }}/images/software/cudimot.jpg" width="15%">
</figure>

CUDIMOT is a front-end that allows the definition and fitting of
non-linear voxelwise models to MRI data using CUDA and GPUs. The user
needs only to specify the cost function and the required model fitting
options (determinsitic, stochastic, priors, noise model) and the
software translates these choices to CUDA code, which is then compiled
to a GPU binary. 

[CUDIMOT and precompiled binaries for NODDI-Watson and 
NODDI-Bingham models](https://users.fmrib.ox.ac.uk/~moisesf/cudimot/index.html){:target="_blank"}
are available.

<hr>

### NMF for data driven mapping of structural connections

<figure>
<img src="{{ site.url }}{{ site.baseurl }}/images/software/nmf.jpg" width="15%">
</figure>

[https://github.com/ethompson93/Data-driven-tractography](https://github.com/ethompson93/Data-driven-tractography)

<hr>

### Processing Pipelines and Data

* HCP Pipelines
* UK Biobank Pipelines
* dHCP Pipelines
* QuNEX

* Multimodal image processing pipelines

<p> &nbsp; </p>
