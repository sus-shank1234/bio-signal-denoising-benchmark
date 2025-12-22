# bio-signal-denoising-benchmark
ECG/biological signal noise characterization and denoising benchmark

**Project Overview**

This repository contains code and analysis for benchmarking noise characterization and denoising methods on biological time-series signals (e.g., ECG). The goal is to evaluate how different signal processing techniques suppress noise while preserving key physiological features. The project includes noise identification, spectral analysis, denoising techniques (bandpass, notch, wavelet), and quantitative evaluation.

**Motivation**

Biological signals such as electrocardiograms (ECG) contain noise from multiple sources—baseline wander, power-line interference, and sensor artifacts. Effective denoising is essential for accurate downstream analysis (e.g., heartbeat detection). This project provides a computational benchmark and comparison of denoising pipelines.

**Data**

We use publicly available ECG and biosignal datasets. Example sources include:

PhysioNet — Physionet hosts clinical ECG databases such as the MIT-BIH Arrhythmia Database.
https://physionet.org/content/mitdb/1.0.0/

BioSPPy Example Data — A Python library with example ECG signals and preprocessing tutorials. 

