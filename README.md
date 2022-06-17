# Parkinson's disease progression modelling 

![Hidden Markov Model](https://github.com/kaminAI/pdp/blob/master/docs/HMM.jpg)


## Abstract

In this project we investigate Parkinson's disease (PD) progression modelling through the use of latent variable models. Specifically we focus on the hidden Markov model (HMM). The HMM, by virtue of its exposition, produces a latent sequence of states. This state sequence is what we will be using as a proxy (and a new metric) for PD progression, by entertaining the states themselves as disease stages. We build on previous work in using HMMs for disease progression modelling and note their utility in dealing with noisy measurements, by employing an abstraction for the disease progression via the latent state sequence. We employ old methods and derive new ones, which are used to analyse the PD progression of subjects in the PPMI and PRECEPT datasets. Variables `UPDRS-II` and `UPDRS-III` togher with with DaT-scan Putamen and Caudate mean intensity values are found to be the most signification and useful for modelling progression. A 13--state HMM model is developed to model progression on a granular level, which is found to be coherent with most clinical metrics. Clustering is performed to identify patients with different progression dynamics. 

## Report

For more information see the [technical report](https://github.com/kaminAI/pdp/tree/master/docs/Lundbeck_PD_Progression_Report_v1.pdf).

## Dependencies

- Python 3.6
- Please refer to `requirements.txt` or `Pipfile.lock` for package dependencies

## Installation

1. Recommended python installation: Anaconda 5.3.1 distribution (https://www.anaconda.com/download/)

2. Python downgrade: terminal command from anywhere: `conda install python=3.6`

3. Pipenv installation: terminal command from anywhere: `pip install pipenv`

4. Create virtuell enviroment from Pipfile: terminal command from project root folder: `pipenv install`

5. Spawn virtuell environment: terminal command from project root folder: `pipenv shell`

6. Create ipython kernel from virtuell enviroment:
terminal command in virtuell environment: `python -m ipykernel install --user --name=pdp`


## Usage

1. Place dataset in pdp\data\raw\lundbeck
2. Launch juptyter labs terminal command from project root folder: `jupyter labs`
3. Open and explore demo notebooks in the `demos` folder

## Demos

`HMM_demo.ipynb`

`IOHMM_demo.ipynb`

`Segmentation_demo_PPMI.ipynb`
