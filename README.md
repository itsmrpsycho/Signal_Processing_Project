# Audio Signal Processing Project

## Team Members
- **Sannidhya Gupta** (2021112012)
- **Krishna Singh** (2021112005)
- **Pratham Kumar Mishra** (2021102036)

## Project Description
This project involves multiple tasks related to audio signal processing, including designing an audio equalizer, distinguishing between different types of signals captured by a stump mic in cricket, separating vocals and instrumentals from audio recordings, and implementing hardware for recording and playing audio signals.

### 1. Audio Equalizer
We developed an audio equalizer to increase the volume of different frequency bands of an audio signal using filtering in the time domain.

- **Band Identification**: The frequency spectrum of the audio signal was divided into 8 parts.
- **Filtering**: We designed band-pass filters by subtracting two low-pass filters.
- **Scaling**: The separated bands were visualized in the frequency domain, and their amplitudes were adjusted.
- **Merging**: The scaled frequency bands were combined to form the final output signal in the time domain.

### 2. Distinguishing Pad and Bat Signals
This task involved distinguishing between the sound of a ball hitting the bat and the sound of a ball hitting the pad in cricket.

- **Denoising**: Applied a median filter and a high-pass filter to remove noise.
- **Processing and Type Identification**: Observed the frequency spectra and identified signals based on the peak frequencies in the FFT.

### 3. Vocal and Instrument Separation
We designed an audio separator to differentiate between tabla sounds and vocals (specifically shrill voices).

- **Identification**: Identified suitable frequency ranges for tabla sounds and distinguished them from vocals.
- **Separation**: Used band-pass and band-reject filters to separate the frequencies.
- **Synthesis**: Converted the frequency domain signals back to the time domain and processed them for enhancement.

### 4. Hardware Implementation
Implemented speaker and microphone circuits as described in Lab 9 and integrated them with the project.

- **Speaker**: Played amplitude arrays by splitting them into parts and playing the dominant frequencies.
- **Microphone**: Recorded sounds and processed them in MATLAB, though practical integration faced challenges due to sampling rate limitations.
