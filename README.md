# Introduction to scientific computing and data science

The materials in this repository were compiled for the course "C268/01: _Foundations of data-driven health science_", developed for the Graduate School of Health Sciences, Aarhus University, Denmark.

## Learning objectives

* Summarize how the main components of a computer relate to, and constrain, the act of "computing".
* Describe the basic organisation of a file system, and navigate it using commands in a "terminal".
* Contrast _textual_ and _binary_ files in terms of their contents and find information in both using tools that can be automated.
* Contrast local and non-local computing resources and file systems, and formulate use cases for both.
* Use _variables_ in a programming language (python) and perform simple operations (manipulations) on the information (data) they contain.
* Write a program to extract, collate and preprocess "raw" data for further processing (statistics, visualisation, _etc._).

## Prerequisites

* a personal computer < 5 years old, with
  * a 64-bit operating system (Windows, Mac or Linux)
  * administrative privileges (password)
  * minimum 20 GB free disk space
* internet access

## How to use the materials

Most of the materials are written as [jupyter notebooks](http://jupyter-notebook.readthedocs.io/en/latest/examples/Notebook/What%20is%20the%20Jupyter%20Notebook.html). Reading and executing these require successful installation of a particular [_software environment_](html/software-environments.html).

You can browse through the materials in static form (_i.e._ without being able to execute any code) on the [GitHub repository-pages](https://github.com/meeg-cfin/scientific_computing_basics).

To get started, [go to the overview-notebook](notebooks/01-Course-Overview.ipynb) and follow the links.

### Using Docker image
A way to get the materials in an all ready functioning and prepackaged way is to use the [Docker](https://www.docker.com/what-docker) image. 

To use the image:

* Install Docker https://docs.docker.com/install/
* Get the Docker image: docker pull meegcfin/scb:latest
* To run the Docker image in a terminal write:
  * docker run -it \-\-rm -p 8888:8888 meegcfin/scb:latest start-notebook.sh
  * This will give a line that looks like this:
	
	http://localhost:8888/?token=56d666e84b27539b51adf4257dc4ddcb8cadd2
	
	Copy and paaste that into a web browser and you are ready to run.
  * If you prefer to use Jupyter Lab start the image with:
  
    docker run -it \-\-rm -p 8888:8888 -e JUPYTER_ENABLE_LAB=1 \-\-rm meegcfin/scb:latest start-notebook.sh

	
