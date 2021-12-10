# Project CMPUT 663: Using Problem Transformation Methods to Identify Knowledge in API Reference Documentation
## Contibutors
- Ravika Nagpal, [ravika@ualberta.ca](ravika@ualberta.ca)
- Samridhi Vaid, [svaid@ualberta.ca](svaid@ualberta.ca)


## Execution Instructions

### Hardware Requirements
You need to have a python installed on your machine. Or you can run below commands by connecting to one of the lab machines as shared in the [doc](https://docs.google.com/document/d/1Cz5zpYSWzm29epYLJM5FpGJHZNnoX9pz8sqt-gXhExg/edit)
Execution Environment Used:
We have tested our code on lab machine (uc02.cs.ualberta.ca) by activating a virtual environment.

### Setup
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

### Execution
Example usage: use the following commands in the current directory.
To get Cado Results:

`python3 CadoEvaluator.py --classifierchain`

`python3 CadoEvaluator.py --labelpowerset`

`python3 CadoEvaluator.py --binaryrelevance`


To get Python Results:

`python3 PythonDataEvaluator.py --classifierchain`

`python3 PythonDataEvaluator.py --labelpowerset`

`python3 PythonDataEvaluator.py --binaryrelevance`


### Data

The Cado dataset can be found at [datasets/cado](datasets/cado),and python dataset can be found at [datasets/python](datasets/python).

### Output 
The output files for each classifier for both the datasets can be found at [output/](output/) folder.

### Notebooks 
The colab notebooks used to replicate the work of Fucci. et al. can be found at [notebooks/](notebooks/) folder. These notebooks contain the same code as provided by previous work and hosted at [DOI](https://zenodo.org/badge/latestdoi/194706952). Please note these notebooks are our attempt to replicate the [study](https://arxiv.org/pdf/1907.09807.pdf) and may contain some of our practice work.

### Report
The report is a pdf (named "report.pdf") found in the same directory as ReadMe.
