# Overview

This repository provides contains artifacts for our Project: 'Using Problem Transformation Methods to Identify Knowledge in API Reference Documentation'  done as part of the course work for CMPUT 663 under the guidance of Professor Sarah Nadi, University of Alberta.

# Abstract
API reference documentation is indispensable to software development. Earlier works studied how modern text classification approaches can automatically identify specific knowledge types in API reference documents. We investigate how effectively problem transformation approaches, which are less computationally costly, can identify certain knowledge types in manually annotated Java and .NET API documentation. We used the results of conventional machine learning (k-NN and SVM) and deep learning approaches from the previous study as our baseline and compared its performance to our proposed classifiers, i.e., Binary Relevance(BR), Label Powerset(LP), and Classifier Chain(CC). The best AUPRC of 99\% was reported when classifying knowledge categories individually (i.e., multiple binary classifiers). The BR and CC classifiers were complementary and delivered outstanding results than our baseline. Even when considering multiple knowledge types at once (i.e., multi-label classification), BR and CC classifier outperformed our baseline, achieving a MacroPrecision, MacroRecall, and MacroF1 of about 99\%. We re-tested our algorithms on the Python documentation dataset to assess how they generalize. Even though none of the classifiers generalized as well as models proposed by the previous work, the Binary Relevance method did show some promising results for the identification of multiple knowledge types.

# Execution Instructions

## Hardware Requirements

- For Mac Os, if you have Python3 installed on your machine, you can run the setup steps on the terminal. Otherwise please install python3.

- For Windows, you need to have a python3 installed on your machine to set up a virtual environment. If you have it installed, open the python terminal to set up the virtual environment by running the commands in the setup section.

-  Alternatively, you can connect to one of the lab machines using the ssh command as shared in the [doc](https://docs.google.com/document/d/1Cz5zpYSWzm29epYLJM5FpGJHZNnoX9pz8sqt-gXhExg/edit). Please follow the document only for using the ssh command. Steps to setup a virtual environment is provided in the setup section below. We have tested our code on the lab machine (uc02.cs.ualberta.ca) by activating a virtual environment.

## Setup
```sh
# Setup python virtual environment
$ virtualenv venv --python=python3
$ source venv/bin/activate

# clone the repo
$git clone https://github.com/SamridhiVaid/SAMRIDHI_RAVIKA_CMPUT663_PROJECT.git

# change directory to the repo where we have requirements file
$ cd SAMRIDHI_RAVIKA_CMPUT663_PROJECT/

# Install python dependencies
$ pip3 install  -r requirements.txt 

```

## Execution
Example usage: use the following commands in the current directory.
To get Cado Results:

`python3 CadoEvaluator.py --classifierchain`

`python3 CadoEvaluator.py --labelpowerset`

`python3 CadoEvaluator.py --binaryrelevance`


To get Python Results:

`python3 PythonDataEvaluator.py --classifierchain`

`python3 PythonDataEvaluator.py --labelpowerset`

`python3 PythonDataEvaluator.py --binaryrelevance`


## Data

The Cado dataset can be found at [datasets/cado](datasets/cado),and python dataset can be found at [datasets/python](datasets/python).

## Output 
The output files for each classifier for both the datasets can be found at [output/](output/) folder.

## Notebooks 
The colab notebooks used to replicate the work of Fucci. et al. can be found at [notebooks/](notebooks/) folder. These notebooks contain the same code as provided by previous work and hosted at [DOI](https://zenodo.org/badge/latestdoi/194706952). Please note these notebooks are our attempt to replicate the [study](https://arxiv.org/pdf/1907.09807.pdf) and may contain some of our practice work.

## Report
The report is a pdf (named "report.pdf") found in the same directory as ReadMe.


# Contibutors
- Ravika Nagpal, [ravika@ualberta.ca](ravika@ualberta.ca)
- Samridhi Vaid, [svaid@ualberta.ca](svaid@ualberta.ca)
