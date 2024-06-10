---
permalink: /
title: "About Me"
excerpt: "About me"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

Hi there! Welcome to my personal page. I am currently a PhD student at the University of Warwick and expect to obtain my degree in the autumn of this year. My research interests include developing cutting-edge deep learning-based control techniques and applying them to autonomous systems such as wind and tidal turbines, as well as unmanned aerial and surface vehicles.

News
======

- 08 May. 2023: My application for participating in the EUTOPIA Impact School has been approvaled by Warwick. Hello Germany!
- 30 Sep. 2023: I have completed the half-year internship (secondment) at National Grid ESO.  

Awesome Projects
======

I am currently working on two EU Horizon projects: WinGrid and ICONIC.

## WinGrid

WinGrid aims to propose cutting-edge techniques to address open issues in the field of wind energy, including wind resource evaluation, wind turbine/farm control, and grid connection. In this project, I have achieved the following milestones:

### Wind Farm Modelling

I have constructed a Computational Fluid Dynamics (CFD)-based wind farm simulator. This simulator can calculate high-fidelity solutions as it integrates the Navier-Stokes equations for wind velocity dynamics and the Actuator Line Model (ALM) for turbine mechanical dynamics. There are many direct applications of this simulator, including:

- Wind farm layout design
- Development of advanced control algorithms/systems
- Machine learning applications such as wind forecasting and turbine lifespan prediction

Prototype of the IEA22 MW wind turbine

<p align="center">
  <img src="../images/IEA22MW.png" alt="turbine" width="400">
</p>

The iso-surface of vorticity

<p align="center">
  <img src="../images/Vorticity.png" alt="Vorticity" width="400">
</p>


The turbine wakes in a wind farm simulated by this simuator:

<p align="center">
  <img src="../images/Velocity.gif" alt="Wakes" width="400">
</p>

### Short-Term Inflow Wind Forcasting

Predictive control of a wind farm requires accurate wind profile forecasts for the upcoming few seconds. Therefore, it is essential to precisely predict the inflow wind in front of a large wind turbine. In this project, I designed a deep-learning model named WindFore to achieve this function. The forecasting results of WindFore are shown below:

<p align="center">
  <img src="../images/pred.gif" alt="First Image" width="250">
  <img src="../images/label.gif" alt="Second Image" width="250">
  <img src="../images/error.gif" alt="Third Image" width="250">
</p>

Left: Prediction via WindFore; Middle: Label from TurbSim; Right: Prdiction Error

### Wind Farm Control

Based on the developed wind farm simulator, I have trained both a single-objective controller and a multi-objective controller for wind farms. The single-objective farm-level controller can coordinate all turbines in a wind farm to mitigate the wake effect by redirecting the wake direction and regulating the wake intensity, thereby increasing the power generation of the wind farm. Building on this, a multi-objective controller has been trained to achieve additional control purposes besides power boost, such as fault ride-through, grid frequency recovery, and more.

The wake patterns without control and the redirection of wakes under various inflow conditions—horizontal inflow, upright inflow, and downright inflow—are illustrated as follows:

![Wake](../images/WakeRediction.png)

## ICONIC
ICONIC leverages AI and creates digital twins to enhance wind farm operations and predict maintenance needs, boosting energy capacity, lowering the average cost of electricity, and accelerating the UK towards its Net Zero target.

The following are visualizations of a portion of the wind farm data collected to train a deep learning-based wind farm wake model, **DeepWake**:

<p align="center">
  <img src="../images/Fig/twilight.png" alt="First Image" width="250">
  <img src="../images/Fig/turbo.png" alt="Second Image" width="250">
  <img src="../images/Fig/terrain.png" alt="Third Image" width="250">
</p>

<p align="center">
  <img src="../images/Fig/Dark2.png" alt="First Image" width="250">
  <img src="../images/Fig/gist_ncar.png" alt="Second Image" width="250">
  <img src="../images/Fig/flag.png" alt="Third Image" width="250">
</p>

<!-- This is the front page of a website that is powered by the [academicpages template](https://github.com/academicpages/academicpages.github.io) and hosted on GitHub pages. [GitHub pages](https://pages.github.com) is a free service in which websites are built and hosted from code and data stored in a GitHub repository, automatically updating when a new commit is made to the respository. This template was forked from the [Minimal Mistakes Jekyll Theme](https://mmistakes.github.io/minimal-mistakes/) created by Michael Rose, and then extended to support the kinds of content that academics have: publications, talks, teaching, a portfolio, blog posts, and a dynamically-generated CV. You can fork [this repository](https://github.com/academicpages/academicpages.github.io) right now, modify the configuration and markdown files, add your own PDFs and other content, and have your own site for free, with no ads! An older version of this template powers my own personal website at [stuartgeiger.com](http://stuartgeiger.com), which uses [this Github repository](https://github.com/staeiou/staeiou.github.io).

A data-driven personal website
======
Like many other Jekyll-based GitHub Pages templates, academicpages makes you separate the website's content from its form. The content & metadata of your website are in structured markdown files, while various other files constitute the theme, specifying how to transform that content & metadata into HTML pages. You keep these various markdown (.md), YAML (.yml), HTML, and CSS files in a public GitHub repository. Each time you commit and push an update to the repository, the [GitHub pages](https://pages.github.com/) service creates static HTML pages based on these files, which are hosted on GitHub's servers free of charge.

Many of the features of dynamic content management systems (like Wordpress) can be achieved in this fashion, using a fraction of the computational resources and with far less vulnerability to hacking and DDoSing. You can also modify the theme to your heart's content without touching the content of your site. If you get to a point where you've broken something in Jekyll/HTML/CSS beyond repair, your markdown files describing your talks, publications, etc. are safe. You can rollback the changes or even delete the repository and start over -- just be sure to save the markdown files! Finally, you can also write scripts that process the structured data on the site, such as [this one](https://github.com/academicpages/academicpages.github.io/blob/master/talkmap.ipynb) that analyzes metadata in pages about talks to display [a map of every location you've given a talk](https://academicpages.github.io/talkmap.html).

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
) that converts a CSV containing structured data about talks or presentations into individual markdown files that will be properly formatted for the academicpages template. The sample CSVs in that directory are the ones I used to create my own personal website at stuartgeiger.com. My usual workflow is that I keep a spreadsheet of my publications and talks, then run the code in these notebooks to generate the markdown files, then commit and push them to the GitHub repository.

How to edit your site's GitHub repository
------
Many people use a git client to create files on their local computer and then push them to GitHub's servers. If you are not familiar with git, you can directly edit these configuration and markdown files directly in the github.com interface. Navigate to a file (like [this one](https://github.com/academicpages/academicpages.github.io/blob/master/_talks/2012-03-01-talk-1.md) and click the pencil icon in the top right of the content preview (to the right of the "Raw | Blame | History" buttons). You can delete a file by clicking the trashcan icon to the right of the pencil icon. You can also create new files or upload files by navigating to a directory and clicking the "Create new file" or "Upload files" buttons. 

Example: editing a markdown file for a talk
![Editing a markdown file for a talk](/images/editing-talk.png)

For more info
------
More info about configuring academicpages can be found in [the guide](https://academicpages.github.io/markdown/). The [guides for the Minimal Mistakes theme](https://mmistakes.github.io/minimal-mistakes/docs/configuration/) (which this theme was forked from) might also be helpful. -->
