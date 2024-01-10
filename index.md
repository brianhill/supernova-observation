# Supernova Observation

*A program of directed study and research aimed at pushing the limits of the Deep Springs Observatory and observing supernovae.*

Terms 4-5 of Spring Semester 2024, Deep Springs College

Mentor/Supervisor: [Prof. Brian Hill](../index.html)

Student Researchers: Ethan Liao (DS 22) and Hexi Jin (DS 23)

## Syllabus

* [Syllabus](./SupernovaObservationSyllabus.pdf) &mdash; A PDF that mirrors what is on this web page

## Overview

This proposal builds on the Academic Year 2022-2023 work of Luke Suess and Sofia Mikulasek. It is a blend of (1) learning the basics of observational astronomy, (2) performing data-taking with research ambitions, and (3) analyzing data in Python. This blend fits under the model of “Research Experience for Undergraduates (REU),” as it is known at many institutions.

We will be guided by the following overarching questions:

* In the dark skies and high altitude which we have at Deep Springs, what observational techniques and conditions make us the most sensitive and accurate that we can we be in detecting and estimating the changes in brightness of stars possibly as least as dim as magnitude 18 with our relatively modest (250mm) telescope? NB: larger numbers are dimmer in the astronomical magnitude system. We have plenty of data that makes us confident that our equipment can easily identify magnitude 18 stars, but supernovae have the added complexity that they are almost always sitting directly on top of a fuzzy background (the galaxy in which they inhabit), and the methods for subtracting background are tricky.
* What are the best practices in the analysis of the data taken in our observations that again push the brightness limits of our setup?
* What transient targets are of the most interest given our data-taking and analysis capability? We believe that supernovae identified by the Zwicky Transient Facility are within our grasp and that supernovae light curves taken over many nights with our gear will be of sufficient interest to the astrophysics community that we can contribute our results to refereed publications. Supernovae have various brightnesses with the brightest ones having peak luminosity brighter than magnitude 17 (see https://www.rochesterastronomy.org/supernova.html).
* How does this work inform preparation for the Vera C. Rubin Observatory which is now just one year from its initial large-scale synoptic surveys?

## Schedule and Work Plan

### Project Activities

All three of us need to be fully cognizant and responsible for the results that we produce. This means that we will (outside of regular meeting times) be independently doing analyses of the data we have taken.

Also, all three of us do not need to be present for all data-taking sessions, so there will be data-taking sessions consisting of just pairs of us taking additional data once the techniques have been established to all three of our satisfaction. A typical data-taking session will run from about 7pm to midnight, which includes time for setup and teardown. Some data-taking sessions will be pre-dawn instead of in the evening (e.g., from about 3am to 7am).

### Phases

Although there is definitely not a hard delineation or progression between (1) establishing technique, (2) using that technique, and (3) analyzing results, there are nonetheless three identifiable phases.

In the first phase, we are principally establishing our experimental technique. A lot of the hard work on this was done in the prior academic year, so in this academic year, we will have the luxury of building on an established technique. Our contribution will be to dramatically increase the accessibility of the passover so that future students have even less wrong turns and debugging to do. Our idea for increasing the accessibility is to create a video passover which should make the many dozens of steps more digestible than they are in their current printed form. Furthermore in the first phase we may want to document the use of a new telescope, to be purchased with funds just gifted to the College.

In the second phase, we are principally using our experimental technique to get one or more excellent datasets. Among the ways that we have to be opportunistic is that supernovae are regularly discovered, but only occasionally (ever few weeks) is one discovered that is suitable for observation with our equipment at our location.

In the third phase, we will be focused on analyzing the best data we have obtained.

### Analytical Work in Python

Our analysis will involve a data-processing pipeline in Python probably using (i) astroalign for alignment (https://astroalign.quatrope.org/en/latest/), and (ii) photutils for aperture-annulus photometry (https://photutils.readthedocs.io/en/stable/getting_started.html). These (and other scientific) packages are most commonly accessed from Jupyter notebooks. Jupyter is an interactive scripting environment for manipulating data, making plots, and running Python code. We will produce the plots for our writeup in Jupyter notebooks.
Research Questions

## Grading/Evaluation

* Observational Work — 35% — This will be comprised of observatory setup and teardown work as well as approximately 10 evenings of data-taking
* Analytical Work — 20% — This will be comprised of data processing using Python packages
* Scientific Record-Keeping — 20% — Records should include: (a) Target Selection Criteria, (b) Listings of Available Targets and their properties, (c) Conditions of Data-Taking, (d) Factors in Data-Processing
* Project Report and Presentation — 25% — We will jointly produce a project report and an expanded passover. If our results are sufficiently significant, our project report will be submitted as a paper to a refereed journal.
