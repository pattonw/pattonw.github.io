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

Getting started
======
1. Register a GitHub account if you don't have one and confirm your e-mail (required!)
1. Fork [this repository](https://github.com/academicpages/academicpages.github.io) by clicking the "fork" button in the top right. 
1. Go to the repository's settings (rightmost item in the tabs that start with "Code", should be below "Unwatch"). Rename the repository "[your GitHub username].github.io", which will also be your website's URL.
1. Set site-wide configuration and create content & metadata (see below -- also see [this set of diffs](http://archive.is/3TPas) showing what files were changed to set up [an example site](https://getorg-testacct.github.io) for a user with the username "getorg-testacct")
1. Upload any files (like PDFs, .zip files, etc.) to the files/ directory. They will appear at https://[your GitHub username].github.io/files/example.pdf.  
1. Check status by going to the repository settings, in the "GitHub pages" section

Site-wide configuration
------
The main configuration file for the site is in the base directory in [_config.yml](https://github.com/academicpages/academicpages.github.io/blob/master/_config.yml), which defines the content in the sidebars and other site-wide features. You will need to replace the default variables with ones about yourself and your site's github repository. The configuration file for the top menu is in [_data/navigation.yml](https://github.com/academicpages/academicpages.github.io/blob/master/_data/navigation.yml). For example, if you don't have a portfolio or blog posts, you can remove those items from that navigation.yml file to remove them from the header. 

Create content & metadata
------
For site content, there is one markdown file for each type of content, which are stored in directories like _publications, _talks, _posts, _teaching, or _pages. For example, each talk is a markdown file in the [_talks directory](https://github.com/academicpages/academicpages.github.io/tree/master/_talks). At the top of each markdown file is structured data in YAML about the talk, which the theme will parse to do lots of cool stuff. The same structured data about a talk is used to generate the list of talks on the [Talks page](https://academicpages.github.io/talks), each [individual page](https://academicpages.github.io/talks/2012-03-01-talk-1) for specific talks, the talks section for the [CV page](https://academicpages.github.io/cv), and the [map of places you've given a talk](https://academicpages.github.io/talkmap.html) (if you run this [python file](https://github.com/academicpages/academicpages.github.io/blob/master/talkmap.py) or [Jupyter notebook](https://github.com/academicpages/academicpages.github.io/blob/master/talkmap.ipynb), which creates the HTML for the map based on the contents of the _talks directory).

**Markdown generator**

I have also created [a set of Jupyter notebooks](https://github.com/academicpages/academicpages.github.io/tree/master/markdown_generator
) that converts a CSV containing structured data about talks or presentations into individual markdown files that will be properly formatted for the Academic Pages template. The sample CSVs in that directory are the ones I used to create my own personal website at stuartgeiger.com. My usual workflow is that I keep a spreadsheet of my publications and talks, then run the code in these notebooks to generate the markdown files, then commit and push them to the GitHub repository.

How to edit your site's GitHub repository
------
Many people use a git client to create files on their local computer and then push them to GitHub's servers. If you are not familiar with git, you can directly edit these configuration and markdown files directly in the github.com interface. Navigate to a file (like [this one](https://github.com/academicpages/academicpages.github.io/blob/master/_talks/2012-03-01-talk-1.md) and click the pencil icon in the top right of the content preview (to the right of the "Raw | Blame | History" buttons). You can delete a file by clicking the trashcan icon to the right of the pencil icon. You can also create new files or upload files by navigating to a directory and clicking the "Create new file" or "Upload files" buttons. 

Example: editing a markdown file for a talk
![Editing a markdown file for a talk](/images/editing-talk.png)

For more info
------
More info about configuring Academic Pages can be found in [the guide](https://academicpages.github.io/markdown/). The [guides for the Minimal Mistakes theme](https://mmistakes.github.io/minimal-mistakes/docs/configuration/) (which this theme was forked from) might also be helpful.
