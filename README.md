# rgbd_enhancement



This repository is for research of depth enhancement.



## Installation

**Warn** The following installation command will install datasets and models. They are may heavy. Take care your PC disk usage.

```
git clone xxx
```



## Directory structure

| Directory      | Description                                                |
| -------------- | ---------------------------------------------------------- |
| `configs`      | Experiment configurations                                  |
| `data`         | Dataset such as DREDS, TransCG, Hand-Surface, etc.         |
| `src/datasets` | Classes to provide unified interfaces to different dataset |
| `src/models`   | Classes to definition of model architecture                |
| `src/metrics`  | Classes of MAE, RMSE, etc.                                 |
| `src/utils`    | Classes of common functions for train, validation, test    |
| `tools`        | Entry point of execute experiment                          |
| `third_party`  | Other great researches, such as Lingbot                    |
| `runs`         | Log of experiments                                         |
| `notebooks`    | Jupyter notebook                                           |
| `reports`      | Experiment results that is described by figures            |



## Record rules

In `runs` directory, 

- One directory, one experiment record.
- Directory name should be `NUMBER_MODELNAME_FEATURE`. For example `003_toy_unet`.
- One directory has `cofig.yaml`, `best.pth`, `metrics.json`, `predictions`.