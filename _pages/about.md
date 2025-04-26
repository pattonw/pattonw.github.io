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

Undergrad:
Virginia Tech:
1. [Mathematics](https://catalog.vt.edu/undergraduate/college-science/mathematics/mathematics-bs-applied-discrete-mathematics/)
2. [Computational Modeling and Data Analytics](https://data.science.vt.edu/programs/cmda.html).

Work:

2018-2021: Software engineer with an emphasis on machine learning and computer vision in 3D microscopy at [Janelia Research Campus](https://www.janelia.org/). I worked with the [cardona lab](https://www.janelia.org/our-research/former-labs/cardona-lab), [funke lab](https://www.janelia.org/lab/funke-lab), [mouselight project team](https://www.janelia.org/project-team/mouselight), and [scicomp](https://www.janelia.org/support-team/scientific-computing-software).

2021-present: Machine Learning Consultant. I continued to work with teams at Janelia: [cellmap](https://www.janelia.org/project-team/cellmap) as well as a few other labs and companies including [E11 BIO](https://e11.bio/), Uri Manor at the [salk](https://www.salk.edu/) and [Kate McDole](https://www2.mrc-lmb.cam.ac.uk/group-leaders/h-to-m/kate-mcdole/) at Cambridge

Most of my work has been in running machine learning projects for large scale image processing in massive 3D volumes of neurons and other cell types throughout tissue samples ranging from drosophila neural tissue to mouse liver, kidney, and heart. I have worked with a wide variety of microscopy data from many different microscope setups such as cryo-em, fib-sem, lightsheet, confocal, and spinning disk. 

Code
====

I am very interested in the intersection of software engineering and scientific computing. I have quite a few libraries that I have contributed to and/or maintain related to the field of large scale segmentation.
1. [gunpowder](https://github.com/funkelab/gunpowder), a package that helps build data processing pipelines in a compute graph structure. This package is extremely helpful for generating training data for volumetric image processing models.
1. [daisy](https://github.com/funkelab/daisy), a tool for blockwise parallelized processing of large volumes with robust logging and error handling. It has some very neat tools for handling the parallelization of tasks that have complicated block boundary interactions.
1. [funlib.*](https://github.com/orgs/funkelab/repositories?q=funlib), a collection of packages containing helpful generalized solutions for simple tasks such as creating and opening datasets with the appropriate metadata, querying our data with appropriate units, and visualization code with [neuroglancer](https://github.com/google/neuroglancer).
  - [funlib.geometry](https://github.com/funkelab/funlib.geometry) - Provides `Coordinate` and `Roi` classes as helpers for working with spatial arrays.
  - [funlib.persistence](https://github.com/funkelab/funlib.persistence) - Provides crud (create/read/update/delete) interfaces for large scale arrays and graphs along with convenient api calls to read/write with spatial queries using `Coordinate` and `Roi` objects.
  - [funlib.math](https://github.com/funkelab/funlib.math) - Some reusable helper functions such as `n` dimensional cantor pairing function along with its inverse.
  - [funlib.show.neuroglancer](https://github.com/funkelab/funlib.show.neuroglancer) - Provides a nice command line interface for spinning up a neuroglancer instance for the visualization of local `n` dimensional zarr arrays.
  - [funlib.learn.torch](https://github.com/funkelab/funlib.learn.torch) - Provides custom torch modules and loss functions commonly used in deep learning applications in microscopy environments.
1. [dacapo](https://github.com/janelia-cellmap/dacapo), a framework designed to help manage configure and apply top machine learning methods on volumetric microscopy data. Used extensively by the [openorganelle](https://www.openorganelle.org/) project to manage the hundreds of networks we trained for various organelles and datasets.
1. [mwatershed](https://github.com/pattonw/mwatershed), a rust implementation of [mutex watershed](https://arxiv.org/abs/1904.12654) that is easily pip installable.
1. [tems](https://github.com/pattonw/tems), a library that provides models that are particularly convenient for blockwise processing.
