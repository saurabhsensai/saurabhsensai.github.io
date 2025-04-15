---
title: "Decoding Brainwave Frequencies: EEG Signal Classification and the Cognitive Effects of Delta, Theta, Alpha, Beta, and Gamma Bands"
excerpt: "Saurabh P. Nale<br/><img src='/images/saurabh/eeg/main.png'>"
collection: portfolio
---

Electroencephalography (EEG) signal classification is a crucial area in neuroscience and brain-computer interface (BCI) research, as it enables the identification of cognitive states and mental activities. This study focuses on classifying EEG signals collected from the Mental Arithmetic Tasks Dataset, available on PhysioNet (https://physionet.org/content/eegmat/1.0.0/). The dataset consists of EEG signals recorded while subjects performed mental arithmetic tasks, making it suitable for exploring cognitive state (Rest vs Task) classification.

Analysis of EEG Bands and Their Significance:

- **Delta Band (0.5 - 4 Hz):**
  - Associated with deep sleep and unconscious brain activity.
  - Higher delta activity may indicate drowsiness or reduced cognitive engagement.

- **Theta Band (4 - 8 Hz):**
  - Linked to memory processing, learning, and relaxed wakefulness.
  - Elevated theta activity is often observed during deep focus and meditation.

- **Alpha Band (8 - 13 Hz):**
  - Related to relaxation and reduced cognitive load.
  - A decrease in alpha activity can indicate heightened mental effort or stress.

- **Beta Band (13 - 30 Hz):**
  - Associated with active thinking, problem-solving, and focus.
  - Increased beta activity is linked to higher cognitive workload and concentration.

- **Gamma Band (30 - 100 Hz):**
  - Involved in complex information processing and higher-order cognitive functions.
  - Often associated with states of heightened perception and consciousness.

Two deep learning models, **EEGNet** and **TSception**, were implemented and evaluated to determine their effectiveness in EEG signal classification.

### **EEGNet Performance:**
- **Test Accuracy:** 0.7976
- **Precision:** 0.7995
- **Recall:** 0.7976
- **F1-score:** 0.7975

### **TSception Performance:**
- **Test Accuracy:** 0.8333
- **Precision:** 0.8638
- **Recall:** 0.8333
- **F1-score:** 0.8305


<figure>
  <img src="/images/saurabh/eeg/1.png" alt="samples" width="600">
  <figcaption style="text-align: center;">Figure 1: Different Frequency bands.</figcaption>
</figure>

<figure>
    <img src="/images/saurabh/eeg/2.png" alt="architecture" width="600">
    <figcaption style="text-align: center;">Figure 2: Power Spectral Density</figcaption>
  </figure>
