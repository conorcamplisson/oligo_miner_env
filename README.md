# OligoMinerEnv

A [conda](https://conda.io/) environment for running [OligoMiner](https://github.com/brianbeliveau/OligoMiner) code.

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

### Background

The magic is done by [environment.yml](./environment.yml), which specifies to conda
the correct version of OligoMiner dependencies:

```
name: oligo_miner_env
channels:
  - bioconda
  - conda-forge
  - defaults
dependencies:
  - biopython=1.74
  - bowtie2=2.3.5
  - jellyfish=2.2.10
  - pip=19.2.3
  - python=2.7.16
  - scikit-learn=0.20.3
```

**NOTE:** This file only contains top-level dependencies, but it results in the following environment:

```
name: oligo_miner_env
channels:
  - bioconda
  - conda-forge
  - defaults
dependencies:
  - _libgcc_mutex=0.1
  - biopython=1.74
  - bowtie2=2.3.5
  - ca-certificates=2019.9.11
  - certifi=2019.9.11
  - jellyfish=2.2.10
  - jemalloc=4.5.0
  - libblas=3.8.0
  - libcblas=3.8.0
  - libedit=3.1.20181209
  - libffi=3.2.1
  - libgcc=7.2.0
  - libgcc-ng=9.1.0
  - libgfortran-ng=7.3.0
  - liblapack=3.8.0
  - libopenblas=0.3.7
  - libstdcxx-ng=9.1.0
  - ncurses=6.1
  - numpy=1.16.4
  - openssl=1.1.1d
  - perl=5.26.2
  - pip=19.2.3
  - python=2.7.16
  - readline=7.0
  - scikit-learn=0.20.3
  - scipy=1.2.1
  - setuptools=41.4.0
  - sqlite=3.30.0
  - tbb=2019.9
  - tk=8.6.9
  - wheel=0.33.6
  - zlib=1.2.11
```
