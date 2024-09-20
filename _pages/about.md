---
permalink: /
title: "Who am I?"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

Education and Work
==================

My path has been fairly simple. I got two undergraduate degrees in [Mathematics](https://catalog.vt.edu/undergraduate/college-science/mathematics/mathematics-bs-applied-discrete-mathematics/) and [Computational Modeling and Data Analytics](https://data.science.vt.edu/programs/cmda.html). I wen't straight from undergrad to working at the [Janelia Research Campus](https://www.janelia.org/). I worked at Janelia for 3 years with the [cardona lab](https://www.janelia.org/our-research/former-labs/cardona-lab), [funke lab](https://www.janelia.org/lab/funke-lab), [mouselight project team](https://www.janelia.org/project-team/mouselight), and [scicomp](https://www.janelia.org/support-team/scientific-computing-software) until I moved to Seattle in the summer of 2021. For reasons relating to the need for remote work I switched to a contractor setup and have since continued working with Janelia, specifically the [cellmap](https://www.janelia.org/project-team/cellmap) as well as a few other labs and companies including [e11](https://e11.bio/), Uri Manor at [the salk](https://www.salk.edu/) and [Kate McDole at Cambridge](https://www2.mrc-lmb.cam.ac.uk/group-leaders/h-to-m/kate-mcdole/)

Most of my work has been in running machine learning projects for large scale image processing in massive 3D volumes of neurons and other cell types throughout tissue samples ranging from drosophila neural tissue to mouse liver, kidney, and heart. I have worked with a wide variety of microscopy data from many different microscope setups such as cryo-em, fib-sem, lightsheet, confocal, and spinning disk. 

My Interests
============

I am very interested in the intersection of software engineering and scientific computing. I have quite a few libraries that I have contributed to and/or maintain related to the field of large scale segmentation.
1. [gunpowder](https://github.com/funkelab/gunpowder), a package that helps build data processing pipelines in a compute graph structure. This package is extremely helpful for generating training data for volumetric image processing models.
1. [daisy](https://github.com/funkelab/daisy), a tool for blockwise parallelized processing of large volumes with robust logging and error handling. It has some very neat tools for handling the parallelization of tasks that have complicated block boundary interactions.
1. [funlib.*](https://github.com/orgs/funkelab/repositories?q=funlib), a collection of packages containing helpful generalized solutions for simple tasks such as creating and opening datasets with the appropriate metadata, querying our data with appropriate units, and visualization code with [neuroglancer](https://github.com/google/neuroglancer).
1. [dacapo](https://github.com/janelia-cellmap/dacapo), a framework designed to help manage configure and apply top machine learning methods on volumetric microscopy data. Used extensively by the [openorganelle](https://www.openorganelle.org/) project to manage the hundreds of networks we trained for various organelles and datasets.
1. [mwatershed](https://github.com/pattonw/mwatershed), a rust implementation of [mutex watershed](https://arxiv.org/abs/1904.12654) that is easily pip installable.
