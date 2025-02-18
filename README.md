# Neuromorphic Computing for Spoken Digits Detection

Spiking Neural Network for classification of spoken digits using the [Spiking Heidelberg Digits (SHD)](https://zenkelab.org/resources/spiking-heidelberg-datasets-shd/) dataset.

This dataset contains approximately 10,000 high-quality, studio-aligned recordings of spoken digits (0–9) in both German and English, recorded by 12 distinct speakers. 
Notably, two of these speakers are only present in the test set. Each digit is represented as spikes across 700 channels, 
which were generated using [Lauscher](https://github.com/electronicvisions/lauscher), a neuromorphic [cochlea](https://iopscience.iop.org/article/10.1088/2634-4386/ac4a83#nceac4a83s47) software model

<div align="center">
    <img src="docs/img/digit_samples.png" width="65%" height="65%">
    <p style="text-align: center"> Figure 1: Samples of Spoken Digits</p>
</div>

## Status of the project

Data Analysis and development of an initial model with good performance was implemented in this 
[notebook](notebooks/Classification_of_spoken_digits_with_snnTorch.ipynb).

In the future, this implementation will be used to develop further the code in the `src` folder and to create a more robust and
scalable code.

## Setup

For the setup of the project follow the instructions in the [SETUP.md](docs/SETUP.md) file.

## Project Structure

```bash
│
├── artifacts                 # folders excluded from the repo, what you store here it won't be store in the repo
│     ├── data
│     └── models
│
├── src                      # source code folder for common code and for CRISP-DM steps
│     ├── common
│     ├── data_understanding
│     ├── data_preparation         
│     └── modelling
│
├── dev-requirements.txt     # testing dependencies
├── environment.yaml         # conda formatted dependencies, used by 'make init' to create the virtualenv
├── README.md                
└── requirements.txt         # core dependencies of the library in pip format
```
