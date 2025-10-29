Overview
This repository contains a project that examines how the human brain responds to visual patterns using electroencephalography (EEG). The focus is on Event-Related Potentials (ERPs), especially the early visual components P1 and N1, which reflect initial stages of sensory processing. By comparing responses to symmetrical versus random visual stimuli, the project seeks to illuminate differences in early visual processing and provide insights into perceptual and cognitive mechanisms.

Introduction
Visual perception is a cornerstone of how humans interact with their environment. EEG is a non-invasive technique that records electrical brain activity with high temporal resolution, making it especially suitable for studying the timing of sensory and cognitive processes. ERPs are time-locked responses within EEG recordings that reveal how the brain reacts to distinct events-here, visual stimuli that are either symmetrical or random. This study concentrates on the P1 and N1 ERP components because they index early stages of visual encoding and attention allocation. By analyzing and contrasting ERPs elicited by the two stimulus types, the project contributes to understanding how pattern regularity influences early cortical responses.

Installation
To use the analysis code and reproduce results, clone the repository and install the required Python packages. The project assumes a working Python 3 environment and relies on common scientific libraries for EEG processing and plotting.

Steps:

Clone the repository and change into its directory.
Install dependencies listed in the requirements file using pip.
Required software includes:

Python 3.x
MNE-Python (for EEG preprocessing and ERP analysis)
Pandas (for data handling)
NumPy (for numerical operations)
Matplotlib (for plotting and visualization)
Usage
Once the environment is prepared, run the analysis script to process raw EEG recordings, perform preprocessing steps, compute ERPs, and generate visualizations. The main script automates the standard pipeline: filtering, artifact removal, epoching, baseline correction, and averaging across trials to produce evoked responses. Outputs include time-series plots of ERPs at selected electrodes and topographic maps showing spatial distributions of ERP amplitudes, enabling direct comparison of P1 and N1 between symmetrical and random stimulus conditions.

Typical command:

Execute the analysis script provided in the repository (for example, python analyze.py).
Methodology
The analysis pipeline follows established EEG/ERP practices to ensure data quality and interpretability. Key stages are:

Data acquisition and preprocessing

EEG was recorded while participants viewed symmetrical and random visual patterns.
Preprocessing steps include bandpass filtering to retain frequencies relevant to early visual components while reducing noise (a typical range used is 0.05–50 Hz).
Independent Component Analysis (ICA) is applied to identify and remove artifacts such as eye blinks and muscle activity.
Continuous data are segmented (epoched) around stimulus onsets to isolate event-related responses.
Baseline correction is applied to each epoch to normalize activity relative to a pre-stimulus reference.
ERP computation and analysis

Trials are averaged within each condition to compute evoked responses.
Peak detection and amplitude/time-window analyses are used to identify P1 and N1 components.
Visualizations include line plots of evoked potentials at representative electrode sites and scalp topographies to inspect spatial patterns.
These steps aim to produce reliable measures of how symmetry versus randomness affects early visual ERP components.

Results
The analysis revealed notable differences in early visual ERPs elicited by the two stimulus classes. Symmetrical patterns tended to evoke stronger P1 and N1 amplitudes compared to random patterns, suggesting that symmetry engages early visual processing more robustly. These differences are visible in the averaged waveforms and the topographic distributions, indicating both temporal and spatial modulation of cortical responses by stimulus regularity. Such findings are consistent with the notion that structured visual information is processed more efficiently at early perceptual stages.
