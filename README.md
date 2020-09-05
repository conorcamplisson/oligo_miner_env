# OligoMinerEnv

A [conda](https://conda.io/) environment for running [OligoMiner](https://github.com/brianbeliveau/OligoMiner) code.

### Overview

OligoMiner requires several python and non-python dependencies:

* python 2.7
* biopython
* scikit-learn
* bowtie2
* jellyfish
* NUPACK

The environment and package manager [conda](https://conda.io/) makes the install process easy, and this repository provides a conda environment that is sufficient to run OligoMiner on Linux and MacOS.

### Installation and usage

1. Install [conda](https://docs.conda.io/en/latest/miniconda.html)

2. Clone this repo. Create and activate the conda environment:

```
$ git clone https://github.com/conorcamplisson/oligo_miner_env.git && cd oligo_miner_env/
$ conda env create -f environment.yml
$ conda activate oligo_miner_env
```

3. That's it! Now you can run OligoMiner:

```
$ git clone https://github.com/brianbeliveau/OligoMiner.git && cd OligoMiner/
$ python probeTm.py -i TATGAGGACGAATCTCCCGCTTATA
32.85
```
