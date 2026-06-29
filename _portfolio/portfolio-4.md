---
title: "Audio Denoising using Spectral Analysis and FIR Filter Design"
excerpt: "DSP-based audio denoising project using Welch spectral estimation and FIR filter design to suppress a 15.2 kHz interference tone.<br/><a href='/files/DSP_Project.pdf'>Read the report (PDF)</a>"
collection: portfolio
permalink: /projects/audio-denoising-dsp/
---

## Overview
This project focuses on **audio denoising using digital signal processing techniques**.  
A sinusoidal interference at **15.2 kHz** was added to an audio signal and removed using a **linear-phase FIR filter** designed under strict real-time DSP constraints.  
The workflow includes spectral analysis using **Welch PSD estimation**, evaluation of windowing parameters, and comparison between multiple FIR filter design methods.

## Highlights
- Spectral estimation using Welch’s method (FFT = 1024, 50% overlap)
- Analysis of window types: Kaiser, Rectangular, Hanning, Hamming
- FIR filter design under latency and computational constraints
- Comparison of Kaiser, Equiripple, Blackman, and Least Squares designs
- Real-time audio denoising with strong stopband attenuation (> 60 dB)

## Methodology
### Spectral Analysis
- Extracted a 3-second audio segment
- Added a 15.2 kHz sinusoidal interference
- Computed single-sided PSD using Welch estimation
- Studied effects of:
  - FFT size
  - Window type
  - Window length
  - Overlap percentage
  - Sampling frequency

### Filter Design
The digital filtering problem required removing a narrowband interference while preserving audio quality.

**Constraints:**
- Latency < 3.2 ms  
- Filter length: 100–200  
- Stopband attenuation ≥ 50 dB  
- Passband ripple ≤ 0.4 dB  

**Chosen Solution:**
A Kaiser-window FIR filter achieved:
- ~75 dB stopband attenuation
- Minimal passband ripple
- Real-time computational feasibility

## Code
- The code is available on <a href="https://github.com/Hacker1one/Audio-Denoising-and-Spectral-Analysis">GitHub</a>

## Report

<iframe src="/files/DSP_Project.pdf" width="100%" height="900px" style="border:none;"></iframe>

