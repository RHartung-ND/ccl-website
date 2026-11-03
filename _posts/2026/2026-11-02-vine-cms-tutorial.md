---
layout: post
title: "Vine CMS Analysis Stack: Tutorial & Hackathon"
date: 2026-11-02T12:00:00-05:00
author: Cooperative Computing Lab
image: /assets/blog/2026/vine-cms-tutorial/cms.png
categories:
  - news
tags:
  - tutorial
  - cms
  - ccl
  - lab-updates
  - taskvine
description: Join the Cooperative Computing Lab on Nov 12–13 for a hands-on tutorial and hackathon to scale your CMS data analysis codes across thousands of cluster nodes.
toc: false
related_posts: false

---

<div class="row justify-content-sm-center">
  <div class="col-sm-6">
    {% include figure.liquid path="/assets/blog/2026/vine-cms-tutorial/cms.png" title="" class="img-fluid rounded z-depth-1" zoomable=true %}
  </div>
</div>

We are excited to share the Vine CMS Analysis Stack, a platform designed to accelerate your computations and streamline your research workflow (and help graduate students finish sooner!).

Built on years of experience scaling data analysis software for the CMS experiment, this open-source stack has enabled Notre Dame researchers to execute analysis workloads across thousands of cluster nodes simultaneously. We are now expanding our reach to deploy this framework with CMS collaborators worldwide.

On **November 12th and 13th**, the Cooperative Computing Lab (CCL) is hosting a hands-on Tutorial & Hackathon tailored for Notre Dame CMS graduate students, postdocs, and faculty.

# Schedule
Both days include the Tutorial & Hackathon.
* **Thursday, November 12**, 10:00 AM–1:00 PM
* **Friday, November 13**, 2:00–5:00 PM

**Location:** Nieuwland Science Hall, University of Notre Dame (room TBA). Remote participation will also be supported.

### Who Should Attend
Anyone comfortable with a terminal, Python, and a text editor. No prior experience with TaskVine, coffea, or HTCondor is needed.

# Tutorial
You'll take a real CMS analysis from a single process on a login node, to a TaskVine worker on the same machine, and finally to a full HTCondor pool, all without changing your processor code. Along the way, you'll learn how to:

* Run the same analysis locally, on a local TaskVine worker, and on an HTCondor pool
* Package a conda environment so remote workers can run your code
* Read a run's health from the live console and the on-disk logs
* Tune chunk sizes, reduction sizes, and resource declarations
* Use checkpoints to restart a run without redoing finished work
* Keep a run going when some chunks fail
* Run several processors over the same datasets in one job

The analysis is written in both **coffea** and **ROOT's RDataFrame**, and you pick whichever you prefer. Both are installed in the same environment, so you can switch at any time.

All exercises use real CMS Open Data from `Run2012B_SingleMu`, the input to the IRIS-HEP ADL benchmarks: 15 ROOT files and about 3.7 million events.

# Hackathon
Bring your own analysis code! Adapt and scale your workflows with direct support from the CCL team.

### Before the Session
Please complete these steps ahead of time. They won't be covered live, and building the environment can take up to 30 minutes.

* Have a **glados account**.
* Have **conda or pixi** working.
* Clone the repository and build its environment by following **[Module 1: Setup](https://github.com/cooperative-computing-lab/vine-cms-analysis-stack-tutorials/blob/main/docs/module-01-setup.md)**.
* Pick an analysis flavor: coffea or RDataFrame.

# Resources & Registration
* **[Registration Form](https://docs.google.com/forms/d/e/1FAIpQLSff3qqeQGoNlCk39xcAPiwt9AUVlT7ee2qBK0Mscx-Ix2IItg/viewform?usp=publish-editor):** Please register in advance to reserve your spot.
* **[Tutorial Repository](https://github.com/cooperative-computing-lab/vine-cms-analysis-stack-tutorials):** Tutorials and codebase.