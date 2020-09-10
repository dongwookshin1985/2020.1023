[//]: # (Important note for Teng Huang - 20200828: Make sure I check all hidden comments before publishing this repo.)

[![INFORMS Journal on Computing Logo](https://INFORMSJoC.github.io/logos/INFORMS_Journal_on_Computing_Header.jpg)](https://pubsonline.informs.org/journal/ijoc)

# JANOS: An Integrated Predictive and Prescriptive Modeling Framework

This archive is distributed in association with the [INFORMS Journal on
Computing](https://pubsonline.informs.org/journal/ijoc) under the [MIT License](LICENSE).

<<<<<<< HEAD
The software and data in this repository are associated with [the paper](https://arxiv.org/abs/1911.09461) by David Bergman, Teng Huang, Philip Brooks, Andrea Lodi, and Arvind U. Raghunathan. 

[//]: # (Need to change the arxiv link to ijoc link.)

**Important: This code is being developed on an on-going basis at 
https://github.com/iveyhuang/2019-11-OA-272. Please go there if you would like to
get a more recent version or would like support.**

[//]: # (Need to change the github repo name to match the final DOI.)

## Version

The version of the software used in the paper is tagged in this repository as `janos 0.0.9`.

It is based on [this SHA](https://github.com/tkralphs/JoCTemplate/commit/f7f30c63adbcb0811e5a133e1def696b74f3ba15) in the development repository. 

[//]: # (Need to update this SHA link.)

## Cite

To cite this software, please cite [the paper](https://arxiv.org/abs/1911.09461) and the software, using the following DOI.

[![DOI](https://zenodo.org/badge/285853815.svg)](https://zenodo.org/badge/latestdoi/285853815) 

[//]: # (Need to update the paper link to ijoc link.)
[//]: # (Need to update the DOI when it is known.)
=======
The software and data in this repository are a snapshot of the software and data
from the [development repository](https://github.com/iveyhuang/2019-11-OA-272)
that were used in the research reported on in the paper 
[JANOS: An Integrated Predictive and Prescriptive Modeling Framework](https://arxiv.org/abs/1911.09461). 

**Important: This code is being developed on an on-going basis at 
https://github.com/iveyhuang/2019-11-OA-272. Please go there if you would like to
get a more recent version or would like support.**

## Cite

To cite this software, please cite [the paper](https://arxiv.org/abs/1911.09461) using its DOI and the software, using its DOI.

[![DOI](https://zenodo.org/badge/288628730.svg)](https://zenodo.org/badge/latestdoi/288628730)
>>>>>>> upstream/master

## Description

JANOS is an integrated predictive and prescriptive modeling framework. It seamlessly integrates the two streams of analytics, for the first time allowing researchers and practitioners to embed machine learning models in an optimization framework.

JANOS allows specifying a prescriptive model using standard optimization modeling elements such as constraints and variables. The key novelty lies in providing modeling constructs that allow for the specification of commonly used predictive models and their features as constraints and variables in the optimization model. JANOS considers two sets of decision variables: regular and predicted. The relationship between the regular and predicted variables are specified as pre-trained predictive models.


## How to use

JANOS works in `python3` and can be downloaded and installed via `pip` using the following command:

`pip install janos`

If you need to upgrade the package at a future date, please install and upgrade using the following command:

`pip install janos --upgrade`

## Replicating

To execute a `.py` file and replicate our experimental results in [the paper](https://arxiv.org/abs/1911.09461), direct to the folder where the `.py` file is located (in `scripts`) in the command line, type `python rewrite_08_20200430_s1.py` and press enter, here taking `rewrite_08_20200430_s1.py` as an example.

<<<<<<< HEAD
[//]: # (update the paper link to a ijoc link when it is available.)

### Data files
`college_student_enroll-s1-1.csv` contains the 20,000 randomly generated student records for training predictive models.

`college_applications6000.csv` contains 6,000 student application records. We randomly draw certain number of records from this pool for our experiments in the paper.


### Code files

`rewrite_08_20200430_s1.py` is for comparing JANOS_Discrete, JANOS_CONTINUOUS, and a greedy heuristic when using logistic regression models and neural networks respectively.

`evaluate_linearize_logistic_20200430.py` is for evaluating the accuracy of the linearization component for logistic regression models.

`evaluate_linear_regression_20200430.py` is for evaluating the performance of JANOS at solving various-sized problems when using linear regression models.

`evaluate_logistic_regression_20200430.py` is for evaluating the performance of JANOS at solving various-sized problems when using logistic regression models.

`evaluate_neural_network_20200430.py` is for evaluating the performance of JANOS at solving various-sized problems when using neural networks.

### Result files

`data_all_scale_20200501_summary.csv` contains the formatted results for generating Figure 3 (The average runtimes of three predictive models with different scales) in the most recent version.

`20200501_logistic_regression_approximation_evaluation_13-56-12-20200502.txt` contains the formatted results for generating Figure 4 (The quality of the linear approximation of the logistic regression function at optimal solutions) in the most recent version.

`rewrite_08_s1_full_15/09/27-20200501.xlsx` contains the formatted results for generating Table 1 in the most recent version.

=======
### Data files
`college_student_enroll-s1-1.csv` contains the 20,000 randomly generated student records for training predictive models.

`college_applications6000.csv` contains 6,000 student application records. We randomly draw certain number of records from this pool for our experiments in the paper.


### Code files

`rewrite_08_20200430_s1.py` is for comparing JANOS_Discrete, JANOS_CONTINUOUS, and a greedy heuristic when using logistic regression models and neural networks respectively.

`evaluate_linearize_logistic_20200430.py` is for evaluating the accuracy of the linearization component for logistic regression models.

`evaluate_linear_regression_20200430.py` is for evaluating the performance of JANOS at solving various-sized problems when using linear regression models.

`evaluate_logistic_regression_20200430.py` is for evaluating the performance of JANOS at solving various-sized problems when using logistic regression models.

`evaluate_neural_network_20200430.py` is for evaluating the performance of JANOS at solving various-sized problems when using neural networks.

### Result files

`data_all_scale_20200501_summary.csv` contains the formatted results for generating Figure 3 (The average runtimes of three predictive models with different scales) in the most recent version.

`20200501_logistic_regression_approximation_evaluation_13-56-12-20200502.txt` contains the formatted results for generating Figure 4 (The quality of the linear approximation of the logistic regression function at optimal solutions) in the most recent version.

`rewrite_08_s1_full_15/09/27-20200501.xlsx` contains the formatted results for generating Table 1 in the most recent version.
>>>>>>> upstream/master

## Ongoing Development

Please find more information on [JANOS's website](http://janos.opt-operations.com).

## Support

For support in using this software,  please submit an
[issue](https://github.com/iveyhuang/2019-11-OA-272/issues) or email [David Bergman](mailto:david.bergman@uconn.edu) and [Teng Huang](mailto:teng.huang@uconn.edu).
<<<<<<< HEAD

[//]: # (Be sure to make the repo public when publishing the paper.)
 
=======
 
>>>>>>> upstream/master
