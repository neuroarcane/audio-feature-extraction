# Audio Feature Extraction

A practical notebook covering the key techniques used to extract meaningful features from audio signals — the foundation of any speech, music, or sound classification system.

## Overview

Raw audio is just a wave of numbers. To make it useful for machine learning, we need to extract **features** that describe the sound in a meaningful way. This notebook walks through the most important audio features using **librosa**, fully compatible with Python 3.12+.

## Features Covered

| Feature | Description |
|---------|-------------|
| **Short-term Energy** | Measures the loudness/intensity of the signal over short windows |
| **Spectral Centroid** | The "centre of mass" of the frequency spectrum — indicates brightness of sound |
| **Mid-term Features** | Aggregated statistics over longer segments for higher-level understanding |
| **Spectrogram** | Visual representation of frequency content over time (via STFT) |
| **Zero Crossing Rate** | How often the signal crosses zero — useful for distinguishing voiced/unvoiced sounds |
| **Spectral Rolloff** | Frequency below which 85% of the total energy is contained |
| **MFCC** | Mel-Frequency Cepstral Coefficients — the most widely used features in speech recognition |
| **Chromagram** | Energy distribution across 12 musical pitch classes (C, C#, D, ..., B) |

## Libraries Used

- [`librosa`](https://librosa.org/) — all audio feature extraction
- `matplotlib` — visualisation
- `numpy` — numerical operations & mid-term feature aggregation
- `sklearn` — normalisation
- `plotly` — interactive plots

## How to Run

1. Clone the repo:
```bash
git clone https://github.com/YOUR_USERNAME/audio-feature-extraction.git
cd audio-feature-extraction
