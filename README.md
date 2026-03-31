# Audio Feature Extraction

A practical notebook covering the key techniques used to extract meaningful features from audio signals — the foundation of any speech, music, or sound classification system.

## Overview

Raw audio is just a wave of numbers. To make it useful for machine learning, we need to extract **features** that describe the sound in a meaningful way. This notebook walks through the most important audio features used in real-world AI systems.

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

- [`pyAudioAnalysis`](https://github.com/tyiannak/pyAudioAnalysis) — short-term & mid-term feature extraction
- [`librosa`](https://librosa.org/) — spectral analysis, MFCC, chromagram, zero crossings
- `matplotlib` — visualisation
- `numpy` — numerical operations
- `sklearn` — normalisation

## Real-World Applications

These features are the backbone of:
- 🗣️ **Speech Recognition** (MFCC is used in Whisper, DeepSpeech)
- 🎵 **Music Genre Classification**
- 😊 **Emotion Detection from Voice**
- 🔊 **Speaker Identification**
- 🏭 **Industrial Sound Anomaly Detection**

## Author
Ali, AI & Data Science Student
