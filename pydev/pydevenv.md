## Python Development Environment

*Documentation of our development environment choices and procedures*

### Install Anaconda

The [2023.09 release](https://www.anaconda.com/blog/new-release-anaconda-distribution-2023-9-and-more) (or higher) of the Anaconda Distribution is the starting point for our development environment. The version of Python in this distribution is 3.11.5. Key tools, services, and apps supporting our work using Python are git, GitHub, Juptyer, PyCharm, and TextMate 2.0. We mostly do analysis on Macs, but we expect our analysis pipeline to be completely portable to any other platform supported by Anaconda.

### Clone the Base Environment

We begin by making a new environment from the base environment:

`conda create --name supernova --clone base`

followed by

`conda activate supernova`

It is a good idea to add the latter command to your `.zshrc` file so that you don't accidentally try to launch jupyter in the base environment.

The environment `supernova` is nothing more than a copy of the environment `base`. However, if we muck the environment up somehow, we can start over by making another copy of `base` rather than re-downloading the Anaconda distribution.

### Launching  Jupyter

First we need to get Jupyter started. In a Terminal window, depending on what notebooks you want to work on, either,

`cd ~/Projects/supernova-observation/pydev`

or,

`cd ~/Projects/supernova-observation/targets`

Then,

`jupyter notebook`

### ccdproc

*ALL THE REST OF THE INFORMATION BELOW HAS NOT BEEN RECENTLY UPDATED. AS WE START A NEW ROUND OF ANALYSES WE WILL UPDATE IT.*

Out data processing pipeline will use [ccdproc](https://ccdproc.readthedocs.io/en/latest/) for image calibration (lights, darks, flats, and biases).

`conda install -c conda-forge ccdproc`

This installed `ccdproc-2.3.1` and various other dependencies.

In a Jupyter notebook, we will follow the [Getting Started](https://ccdproc.readthedocs.io/en/latest/getting_started.html) documentation for `ccdproc`.

### astroalign and twirl

We will use [astroalign](https://astroalign.quatrope.org/en/latest/) for alignment and [twirl](https://github.com/lgrcia/twirl) for plate-solving.

`conda install -c conda-forge astroalign`

Twirl in turn needs astroquery.gaia. Neither twirl nor astroquery are available through the repo.anaconda.com channels, so we use:

`pip install twirl`

`pip install astroquery`

### astropy.visualization

We will use [astropy.visualization](https://docs.astropy.org/en/stable/visualization/index.html) and/or custom stretching routines to examine images at various stages of the data-processing pipeline.

### photutils

We plan to use [photutils](https://photutils.readthedocs.io/en/stable/getting_started.html) for [PSF photometry](https://photutils.readthedocs.io/en/stable/psf.html).

`conda install -c conda-forge photutils`
