# bio-signal-denoising-benchmark
ECG/biological signal noise characterization and denoising benchmark

**Project Overview**

This repository contains code and analysis for benchmarking noise characterization and denoising methods on biological time-series signals (e.g., ECG). The goal is to evaluate how different signal processing techniques suppress noise while preserving key physiological features. The project includes noise identification, spectral analysis, denoising techniques (bandpass, notch, wavelet), and quantitative evaluation.

**Motivation**

Biological signals such as electrocardiograms (ECG) contain noise from multiple sources—baseline wander, power-line interference, and sensor artifacts. Effective denoising is essential for accurate downstream analysis (e.g., heartbeat detection). This project provides a computational benchmark and comparison of denoising pipelines.

## Progress Log

### Day 1
- Set up Python virtual environment
- Installed core scientific libraries
- Loaded ECG dataset
- Visualized raw ECG waveform using Matplotlib

## Next Steps
- Quantify noise characteristics
- Implement baseline denoising methods (filters)
- Compare performance using SNR and RMSE

**Data**

We use publicly available ECG and biosignal datasets. Example sources include:

PhysioNet — Physionet hosts clinical ECG databases such as the MIT-BIH Arrhythmia Database.
https://physionet.org/content/mitdb/1.0.0/

BioSPPy Example Data — A Python library with example ECG signals and preprocessing tutorials. 

**Tools & Libraries**

Install dependencies: pip install numpy scipy matplotlib biosppy pywavelets

**Useful libraries**:

BioSPPy — Python toolkit for biosignal processing (ECG, EEG, EMG). 
PyPI

PyWavelets — Wavelet transforms for denoising.

SciPy — Filters and signal utilities.

**Noise Characterization**
Load ECG signals and plot:

- Time domain waveform

- Frequency spectrum (FFT / PSD)

Identify noise patterns:

- Baseline drift

- Power-line interference

- Motion artifacts

**Denoising Methods**
1. Bandpass Filtering

Suppresses frequencies outside a physiological range (e.g., 0.5–40 Hz for ECG).

2. Notch Filtering

Targets specific narrowband noise (e.g., 50/60 Hz power line interference).

3. Wavelet Denoising

Performs multiscale decomposition and thresholding to reduce noise while preserving morphology. Similar approaches are used in other repositories that apply wavelet denoising to ECG signals.

**Evaluation Metrics**

We evaluate methods based on:

Signal-to-Noise Ratio (SNR)

Mean Squared Error (MSE) against baseline

Preservation of ECG features (e.g., R-peak)

**Example Repositories & References**

These repositories and tools offer useful context, code examples, or alternative methods I can reference or adapt:

ECG Signal Processing – Basic Python scripts for ECG denoising & processing. 
GitHub

[https://github.com/tejasa97/ECG-Signal-Processing
](url)

ECG Denoising with Wavelets & Filters – Combines wavelet and Savitzky–Golay filters. 
GitHub

[https://github.com/MichWozPol/ECG_denoising
](url)

Feature Extraction from ECG Signals – Wavelet decomposition and ECG feature detection. 
GitHub

[https://github.com/Soroushsrd/ECG_Feature_Extraction
](url)

BioSPPy Library – Useful Python biosignal processing library with ECG support. 
PyPI

[https://github.com/scientisst/BioSPP
](url)




