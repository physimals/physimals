---
title: "CoNI Lab - Software"
layout: textlay
excerpt: "Software"
sitemap: false
permalink: /software
---

# Software

We have a track record of developing and publicly releasing software
for neuro-image processing and analysis.

[FSL](#fsl-toolboxes), [HCP WM Atlases](#hcp-white-matter-atlases),
[CUDIMOT](#cudimot), [NFacT](#nfact), [Pipelines and Data](#processing-pipelines-and-data)


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

The CUda DIffusion MOdeling Toolbox (CUDIMOT) is a C front-end that allows the definition and fitting of
non-linear voxelwise models to MRI data using CUDA and GPUs (see
relevant [paper](https://doi.org/10.1016/j.neuroimage.2018.12.015)). The user
needs only to specify a cost function and model fitting
options (deterministic nonlinear fitting-Levenberg Marquardt, Bayesian
fitting-MCMC, priors, noise model) in C header file and the
software translates these choices to CUDA code, which is then compiled
to a binary that performs model fitting and can run on GPUs. The toolbox
has been made with tissue microstructure models for diffusion MRI data
in mind, but it can be used for any voxel-wise model of MRI data. 

[CUDIMOT and precompiled binaries for NODDI-Watson and 
NODDI-Bingham models](https://users.fmrib.ox.ac.uk/~moisesf/cudimot/index.html){:target="_blank"}
are available.

<hr>

### NFacT
<figure>
<img src="{{ site.url }}{{ site.baseurl }}/images/software/nmf.jpg" width="15%">
</figure>

NFacT (Non-negative matrix FACtorisation of Tractography data) is a framework for performing data-driven decomposition of
whole-brain tractography. This allows concurrent delineation of white matter (WM) bundles
and grey matter (GM) networks (see relevant
[paper](https://www.biorxiv.org/content/10.1101/2020.03.09.965079v1)). We
also allow non-negative dual regression for projecting group-wise
WM/GM components to individual subjects.

[NFacT routines](https://github.com/ethompson93/Data-driven-tractography)
are available in python.

<hr>

### Processing Pipelines and Data
<figure>
<img src="{{ site.url }}{{ site.baseurl }}/images/software/pipelines.jpg" width="15%">
</figure>

We provide [neuroimage processing pipelines](https://doi.org/10.5281/zenodo.3624973) (written in bash) for a number of imaging
modalities, including structural MRI, diffusion MRI and functional
MRI. The pipelines perform a number of steps needed on the raw data,
including template-space registrations, tissue segmentation, cortical
surface extractions, distortion and motion correction, cross-modality
alignment, denoising.

* HCP Pipelines
* UK Biobank Pipelines
* dHCP Pipelines
* QuNEX


<p> &nbsp; </p>
