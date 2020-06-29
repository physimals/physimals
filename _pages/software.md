---
title: "Physimals - Software"
layout: textlay
excerpt: "Software"
sitemap: false
permalink: /software/
---

# Software

We have a track record of developing and publicly releasing software
for neuro-image processing and analysis.

### Fabber

<img src="{{ site.url }}{{ site.baseurl }}/images/software/fabberfit.png" class="img-responsive" width="25%" style="float: left" />

Fabber is a Bayesian model fitting framework which uses the Variational Bayes
algorithm to do fast model fitting of nonlinear forward models.

 - [Fabber core](https://fabber-core.readthedocs.io) defines the main model fitting algorithm
   and contains a few simple generic models for testing and demonstration purposes.
 - [Fabber ASL models](https://fabber-asl.readthedocs.io) is a set of Fabber models for
   ASL-MRI data
 - [Fabber DCE models](https://fabber-dce.readthedocs.io) is a set of Fabber models for
   DCE-MRI data
 - [Fabber DSC models](https://fabber-dsc.readthedocs.io) is a set of Fabber models for
   DSC-MRI data
 - [pyfab](https://pyfab.readthedocs.io) is a Python API for Fabber
 - [fabber_matlab](https://fabber-matlab.readthedocs.io) is a simple Matlab interface
   to Fabber
   
<div style="clear: both;"></div>
 
### Processing pipelines

<img src="{{ site.url }}{{ site.baseurl }}/images/software/basilgui.png" class="img-responsive" width="30%" style="float: right" />

These are FSL-based pipelines for processing different types of medical imaging data.
They utilise Fabber for the model fitting but also include pre and post
processing specific to the data type.

 - [oxford_asl / basil](https://asl-docs.readthedocs.io/) is the standard FSL
   based pipeline for processing ASL data.
 - [oxasl](https://oxasl.readthedocs.io) is a new Python-based
   pipeline, largely compatible with `oxford_asl` but with some new features
   and also supporting multiphase and vessel-encoded ASL data.
 - [verbena](https://verbena.readthedocs.io) is a pipeline for processing 
   DSC data.
 - [hcp-asl](https://github.com/ibme-qubic/hcp-asl) is a pipeline for processing ASL data from the Human
   Connectome Project

<div style="clear: both;"></div>

### Quantiphyse

<img src="{{ site.url }}{{ site.baseurl }}/images/software/qpwins.png" class="img-responsive" width="25%" style="float: left" />

Quantiphyse is a GUI viewing and analysis package for biomedical imaging data. 
As well as generic visualisation and processing functionality, it contains a set of
plugins for processing specific kinds of imaging data including ASL, DCE, CEST, DSC
and quantitative BOLD.

- [Quantiphyse](https://quantiphyse.readthedocs.io) is the main application. Other
  repositories contain various plugins however documentation for these is kept
  centrally.
  
<div style="clear: both;"></div>

### Python libraries

- [Toblerone](https://toblerone.readthedocs.io) contains tools for surface based
  analysis including projection and partial volume estimation.
  
- [Regtricks](https://regtricks.readthedocs.io) contains tools for manipulating, 
  combining and applying image transformations.  

### SVB

SVB is an implementation of Stochastic Variational Bayes for inferring on medical
imaging timeseries data. It aims to solve the same problem as Fabber by an alternative
means which may provide advantages in some cases.

- [SVB](https://svb.readthedocs.io) is the main implementation currently containing exponential and ASL models

<div style="clear: both;"></div>

### Software Tutorials
   
 - The [FSL course](https://fsl.fmrib.ox.ac.uk/fslcourse/) contains a practical session on
   ASL-MRI processing using the Basil/Oxford ASL toolbox.
   
 - [Neuroimaging Primers](http://www.neuroimagingprimers.org/) is a series of short, accessible 
   textbooks focused on MRI-based neuroimaging. Under `Example Boxes` you can find a set of interactive
   tutorials on ASL-MRI data processing using the Basil/Oxford ASL toolbox.

 - The [Variational Bayes Tutorial](https://vb_tutorial.readthedocs.io) contains interactive code
   demonstrating simple implementations of Analytic and Stochastic variational Bayes.

 - Tutorials for DCE, qBOLD and ASL using Quantiphyse are included in the general 
   [Quantiphyse documentation](https://quantiphyse.readthedocs.io)


<p> &nbsp; </p>
