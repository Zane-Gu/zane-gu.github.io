---
title: "Planetary Gearbox Fault Diagnosis"
date: '2022-06-01'
summary: "Adaptive energy-ratio analysis and machine learning for vibration-based gearbox fault diagnosis."
image:
  alt_text: "Schematic planetary gear set and highlighted vibration-spectrum sidebands"
  caption: "Original schematic of planetary gears and sideband analysis; not experimental data."
---

**BEng final-year research project · Tianjin University of Technology · June 2020–June 2022**

Supervised by Professor [Mian Zhang](https://me.tjut.edu.cn/info/1060/1786.htm).

### Situation

Planetary gear faults can appear as modulation sidebands in vibration spectra. A conventional sideband energy ratio (SER) uses a fixed number of sidebands and a fixed frequency bandwidth, chosen empirically; those settings may not remain informative across different operating conditions.

### Task

I investigated how to adapt the frequency-domain indicator so that sun-gear and planet-gear faults could be distinguished under varying conditions.

### Action

I developed a **dynamic sideband energy ratio (DSER)** scheme. For each operating condition, the method constructs an SER matrix over candidate sideband counts and bandwidths. Deep neural network and support vector machine classifiers turn this matrix into a fault-classification accuracy map; the best-performing parameter pair is selected to define the DSER, then applied to the remaining gearbox data. My project also used MATLAB-based Fourier and wavelet analysis to inspect vibration signals.

### Result

The [published experiments](https://doi.org/10.1088/1361-6501/ac0701) reported better diagnosis of sun- and planet-gear faults than fixed-parameter SER across the tested operating conditions. The work was recognized with the Best Undergraduate Thesis Award, and my thesis received a grade of 93%.

**Related publication:** [Intelligent fault diagnosis of a planetary gearbox based on dynamic frequency energy ratio scheme](/publications/dynamic-frequency-energy-ratio/).
