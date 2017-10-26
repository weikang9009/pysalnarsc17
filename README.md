# Spatial Data Analysis with PySAL @NARSC2017

### Instructors

- [Sergio Rey](http://sergerey.org) - University of California, Riverside
- [Wei Kang](http://spatial.ucr.edu) - Arizona State University


![journeys](figs/readmefigs/routes.png)

---

This repository contains the materials and instructions for the PySAL workshop at [NARSC 2017](http://www.narsc.org/newsite/conference/workshops-and-tutorials/)


## Schedule


* 8:00-10:00
  * Overview of PySAL and workshop
  * Introductions
  * Installation
  * Jupyter notebooks
  * Python primer
* 10:00-10:30
  * Coffee Break
* 10:30-12:30
  * Spatial data processing
  * Choropleth mapping and geovisualization
  * Spatial weights
* 12:30-1:30
  * Lunch
*  1:30-3:00
  * Global spatial autocorrelation
  * Local spatial autocorrelation
  * Spatial inequality analysis
* 3:00-3:30
  * Coffee Break  
* 3:30-5:00
  * Geodemographics and regionalization
  * Spatial dynamics
  * Spatial regression
  
## Obtaining Workshop Materials

If you are familiar with GitHub, you should clone or fork this GitHub repository. Cloning can be done by:

```bash
git clone https://github.com/sjsrey/nasrc17.git
```

If you are not using git, you can grab the workshop materials as a zip file by pointing your browser to (https://github.com/sjsrey/nasrc17.git) and clicking on the green *Download* button in the upper right.

FIXME: put image of button here

## Installation

We will be using a number of Python packages for geospatial analysis, specifically you must have the following installed:

FIXME: list of packages here


An easy way to install all of these packages is to use a Python distribution such as [Anaconda CE](http:/store.continuuum.io/ "Anaconda CE"). In this workshop we will be using Python 2.7 so please select that version of Anaconda.


Once you have downloaded Anaconda or have set up Python another way, start a terminal and run:

```bash
conda-env create -f workshop.yml
```

This will build a conda environment that sandboxes the installation of the required packages for this workshop so we don't break anything in your computer's system Python (if it has one).

This may take 10-15 minutes to complete depending on the speed of your network connection.

Once this completes, you can activate the workshop environment with:
```bash
source activate workshop```

Next, you will want to test your installation with:
```bash
 jupyter-nbconvert --execute --ExecutePreprocessor.timeout=120 check_workshop.ipynb
 ```

you should see something like:
```bash
[NbConvertApp] Converting notebook check_workshop.ipynb to html
[NbConvertApp] Executing notebook with kernel: python2
[NbConvertApp] Writing 435635 bytes to check_workshop.html
```

If you do see the above, you are ready for the tutorial. If not, please contact either of us for help.
