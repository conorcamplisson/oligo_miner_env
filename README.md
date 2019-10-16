# OligoMinerEnv

A [conda](https://conda.io/) environment for running [OligoMiner](https://github.com/brianbeliveau/OligoMiner) code.

### Installation and usage

1. Install [conda](https://docs.conda.io/en/latest/miniconda.html)

2. Clone this repo and create the conda environment:

```
$ git clone git@github.com:conorcamplisson/oligo_miner_env.git
$ cd oligo_miner_env/
$ conda env create -f environment.yml
```

3. Activate the new conda environment:

```
$ conda activate oligo_miner_env
```

4. That's it! Now you can run OligoMiner:

```
$ git clone git@github.com:brianbeliveau/OligoMiner.git
$ cd OligoMiner/
$ python probeTm.py -i TATGAGGACGAATCTCCCGCTTATA
32.85
```

