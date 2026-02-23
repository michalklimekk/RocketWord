# RocketWord

This repository contains supplementary materials related to the RocketWord method for time series classification.

RocketWord is a time series classification framework based on the following pipeline:

Time series → ROCKET feature extraction → symbolic discretization → 1-NN classification.

At the current stage, this repository provides documentation of the experimental setup and empirical results used in the evaluation. The full implementation and the corresponding publication will be added after formal publication of the paper.

---

## Data and Benchmark Results Source

The benchmark datasets and reference results used in this repository are derived from the Time Series Classification website (https://www.timeseriesclassification.com), an established resource that hosts widely used collections of time series classification datasets and reference performance results. This includes datasets from the UCR and UEA archives, as well as state-of-the-art results for comparative evaluation.

---

## Repository Structure

The repository includes materials describing the experimental setting and comparative evaluation:

- `datasets.pdf` lists the benchmark datasets used for training and evaluation.
- `algorithms.pdf` contains a list of the state-of-the-art methods used for comparative analysis.
- `results/` contains experimental results obtained under different ROCKET configurations. This includes:
  - main results using 1000 ROCKET kernels (averaged over 10 runs),
  - additional experiments analysing performance as a function of the number of ROCKET kernels (averaged over 5 runs),
  - supplementary statistical summaries where applicable.

Performance is evaluated using classification accuracy, which is reported as the primary metric since the benchmark datasets are class-balanced.

---

## Experimental Setting

Experiments were conducted using 1000 ROCKET kernels, with each algorithm evaluated over 10 independent runs. Additional experiments analyse performance sensitivity to different numbers of ROCKET kernels, with results averaged over 5 runs.

---

## Code Availability

The implementation of the RocketWord method will be made publicly available in this repository after publication.
