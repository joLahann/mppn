# MPPN
> This repository contains the source code of the paper Multivariate Business Process Representation Learning for Predictive Process Analytics, which is currently under review for the BPM 2021.


## Installation

The recommended way to install the scripts is:
```
cd mppn
conda create --name mppn python=3.7.
conda activate mppn
python setup.py install
```
This way all requirements are also installed including pytorch, cuda and fastai.


To run the jupyter notebooks you also have to create a jupyter kernel:

```
python -m ipykernel install --user --name mppn
```

## Content

- `00_preprocessing.ipynb` contains all the pre-processing logic for the process prediction tasks, including normalization and categorization, subsequence generation and data loader creation.
- `01_pipeline.ipynb` includes the pipeline and the runner method to run all prediction models and tasks.
- `02_baselines.ipynb` includes the implementation of 4 current approaches of process prediction.  
- `03_mppn.ipynb` presents the implementation of the MPPN that is described in the paper.
- `04_prediction_evaluation.ipynb` runs the evaluation and logs the results.
- The four jupyter notebooks build up and are also exported to python files that are located under `./mppn/`. 
- The experiment can also be run from command line with `python mppn/prediction_evaluation.py`
- The event logs are stored under `./event_logs/`
- The results are stored under `./results/`




The repository is build with the nbdev package -> https://nbdev.fast.ai/.
