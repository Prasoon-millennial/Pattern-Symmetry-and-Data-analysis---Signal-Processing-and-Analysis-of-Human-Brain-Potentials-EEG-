
🔍 Overview

This repository contains a project that examines how the human brain responds to visual patterns using electroencephalography (EEG).
The focus is on Event-Related Potentials (ERPs) — especially the early visual components P1 and N1, which reflect initial stages of sensory processing.
By comparing responses to symmetrical versus random visual stimuli, the project seeks to highlight differences in early visual processing and provide insights into perceptual and cognitive mechanisms.

🧩 Introduction

👁️ Visual perception is central to how humans interact with their surroundings.
⚡ EEG is a non-invasive technique that records electrical brain activity with high temporal precision, making it ideal for studying the timing of sensory and cognitive events.
📈 ERPs are time-locked responses within EEG signals that reveal how the brain reacts to specific events — here, visual stimuli that are symmetrical or random.

This study focuses on the P1 and N1 ERP components, as they indicate early stages of visual encoding and attention allocation.
By analyzing and comparing ERPs elicited by both stimulus types, the project advances understanding of how pattern regularity influences early cortical responses.

⚙️ Installation

To use the analysis code and reproduce results, clone the repository and install required dependencies.
The project assumes a Python 3 environment and uses standard scientific libraries for EEG data processing and visualization.

🪜 Steps:

🌀 Clone the repository and change into its directory

📦 Install dependencies listed in the requirements.txt file using pip

🧰 Required software:

🐍 Python 3.x

🧬 MNE-Python (for EEG preprocessing and ERP analysis)

🧾 Pandas (for data handling)

🔢 NumPy (for numerical operations)

📊 Matplotlib (for plotting and visualization)

🚀 Usage

Once the environment is ready, run the analysis script to:

Process raw EEG recordings 🧠

Perform preprocessing steps 🧹

Compute ERPs 📈

Generate visualizations 🎨

The main script automates standard EEG steps:

Filtering

Artifact removal

Epoching

Baseline correction

Averaging trials

Outputs include:

⏱️ ERP time-series plots

🗺️ Topographic maps of ERP amplitudes

These allow direct comparison of P1 and N1 components between symmetrical and random stimuli.

💻 Typical command:
python analyze.py

🧪 Methodology

The analysis pipeline follows established EEG/ERP standards to ensure quality and reproducibility.

🧼 Data acquisition and preprocessing:

EEG recorded during viewing of symmetrical and random visual patterns

Bandpass filtering (0.05–50 Hz) to retain relevant frequencies

Independent Component Analysis (ICA) for artifact removal (eye blinks, muscle noise)

Epoching data around stimulus onsets

Baseline correction relative to pre-stimulus intervals

📊 ERP computation and analysis:

Average trials per condition to compute evoked responses

Detect P1 and N1 peaks for amplitude and latency comparisons

Generate line plots and scalp topographies for spatial visualization

🧠 These steps ensure robust measures of how symmetry vs. randomness modulates early visual brain activity.

📈 Results

✨ The analysis revealed clear differences between responses to symmetrical and random patterns.
🔹 Symmetrical stimuli evoked stronger P1 and N1 amplitudes, suggesting enhanced early visual engagement.
🔹 These effects are reflected in both averaged waveforms and topographic maps, showing distinct temporal and spatial modulation of brain activity.

📚 Overall, the findings support the idea that structured visual information (like symmetry) is processed more efficiently in early perceptual stages.
