# Project CMPUT 663: Using Problem Transformation Methods to Identify Knowledge in API Reference Documentation
## Team
|Student name  | CCID    |
|--------------|---------|
|Ravika Nagpal |  ravika |
|Samridhi Vaid |  svaid  |


# 2. Execution Instructions

## Setup
```sh
# Setup python virtual environment
$ virtualenv venv --python=python3
$ source venv/bin/activate

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

Execution Environment Used:
We have tested our code on lab machine (uc02.cs.ualberta.ca) by activating a virtual environment.


## Data

The Cado dataset can be found at [datasets/cado](datasets/cado),and python dataset can be found at [datasets/python](datasets/python).

## Output file 
The output is stored in the csv file under Ouptut folder

## Report
The report is a pdf (named "report.pdf") found in the same directory as ReadMe.
