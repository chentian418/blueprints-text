# Blueprints for Text Analysis Using Python

## Machine Learning Based Solutions for Common Real World (NLP) Applications

[Jens Albrecht](https://www.linkedin.com/in/jens-albrecht), [Sidharth Ramachandran](https://www.linkedin.com/in/sidharthramachandran/), [Christian Winkler](https://www.linkedin.com/in/drchristianwinkler/)

Published by [O'Reilly Media, 2020](https://www.oreilly.com/library/view/blueprints-for-text/9781492074076/)

![cover](https://learning.oreilly.com/library/cover/9781492074076/250w/)

Github: [https://github.com/blueprints-for-text-analytics-python](https://github.com/blueprints-for-text-analytics-python)

-----------------------------------------------------------------------------------

# Content

**This repository is currently in preparation. Please do not yet send any comments.**

This repository contains the code examples of our O'Reilly book. You will find a subdirectory for each chapter containing a jupyter notebook and additional files for the setup. You can view the notebook content here on Github. The most simple way to execute the code without any setup is to use [Google Colab](https://colab.research.google.com/notebooks/intro.ipynb#), Google's free cloud-based service for machine-learning with Python. Simply click on the links provided in the next section. In the section thereafter, you will find instructions to setup the environment on your local computer.

If you discover any problems or have recommendations how to improve the code, do not hesitate to create an issue [here in the repository](https://github.com/blueprints-for-text-analytics-python/blueprints-text/issues).

For errors in the book text, please use [O'Reilly's errata page](https://www.oreilly.com/catalog/errata.csp?isbn=0636920309222).

## Working on Google Colab

Simply click on the link for respective chapter to open a runnable copy of the notebook on Colab. In Colab, click "View&rarr;Expand Sections" to view the complete code immediately. Don't forget to run the first code cells for the setup.

  * [Chapter 1: How to gain first Insights from Textual Data](https://colab.research.google.com/github/blueprints-for-text-analytics-python/early-release/blob/master/ch01/Data_Exploration_Code.ipynb#) 
  * [Chapter 2]() 
  * [Chapter 3]() 
  * [Chapter 4]() 
  * [Chapter 5]() 
  * [Chapter 6]() 
  * [Chapter 7]() 
  * [Chapter 8]() 
  * [Chapter 9]() 
  * [Chapter 10]() 
  * [Chapter 11]() 
  * [Chapter 12]() 
  * [Chapter 13]() 

## Local Setup

The following instructions should work on Linux and Windows. If you are a Windows user familiar with Linux, you should check out the [Windows Subsystem for Linux, Version 2 (WSL2)](https://docs.microsoft.com/en-us/windows/wsl/). This allows to use a Linux system on the Windows machine. However, using native Windows should also be no problem.

It is helpful to install `git` on your machine, but you can also download the full repository from Github as a zip file. If you use git, run the following commands from the command line:

```sh
git clone https://github.com/blueprints-for-text-analytics-python/blueprints-text.git
cd blueprints-text
```

Otherwise download the zip file, unpack it to a location convenient to you, and open a command line terminal in the project directory `blueprints-text`.

For local setup, we recommend to use [Miniconda](https://docs.conda.io/en/latest/miniconda.html), a minimal version of the popular [Anaconda](https://www.anaconda.com/) distribution that contains only the package manager `conda` and Python. Follow the installation instructions on the [Miniconda Homepage](https://docs.conda.io/en/latest/miniconda.html). If you already have Anaconda or Miniconda installed on your system: That's fine. We will create a separate virtual environment for the blueprints book so that our installation will not interfere with your previous setup.

After installation of Anaconda/Miniconda, run the following command(s) from the project directory:

```sh
conda env create --file blueprints.yml
conda activate blueprints
```

The prompt should change after activation and indicate that you are working in the `blueprints` environment. Our installation includes the [Jupyter notebook extensions](https://github.com/ipython-contrib/jupyter_contrib_nbextensions). We suggest to enable the extensions  table of contents (toc2), execute time, and variable inspector (varInspector):

```sh
jupyter nbextension enable toc2/main
jupyter nbextension enable execute_time/ExecuteTime
jupyter nbextension enable varInspector/main
```

Now you can start the Jupyter notebook server:

```sh
jupyter notebook
```

If working on WSL under Windows, add `--no-browser`.

Browse to the respective chapter and open the notebook file (suffix `.ipynb`)
