---
title: "Motion-Based Handwriting Recognition"
date: '2023-03-01'
summary: "An inertial sensing pen and machine learning models for recognizing handwritten lowercase characters."
image:
  alt_text: "Schematic sensor pen, inertial motion signal, and recognized handwritten character"
  caption: "Original schematic of motion-based handwriting recognition; not a photograph of the prototype."
---

**MSc team research project · Imperial College London · October 2022–March 2023**

### Situation

Handwriting is usually recognized from an image of the finished character. Our team instead explored whether the movement of a pen itself could provide enough information to recognize lowercase letters, without making a camera the primary sensing device.

### Task

We needed a portable way to record labeled pen movements and a classifier able to learn patterns from motion signals rather than static images.

### Action

I worked with the team on a 3D-printed pen prototype containing an inertial measurement unit (IMU) and a button for controlled recording. The button helped delimit and label writing samples. We investigated sequence and convolutional models—LSTM, bidirectional LSTM, GRU, and CNN—as well as a stacked ensemble for recognizing lowercase characters from the recorded signals.

### Result

The project produced a sensing prototype and a comparison of machine-learning approaches to motion-based character recognition. The team project received a mark of 91.7%. The related work was published as [*Motion Is All You Need*](https://doi.org/10.1109/ICMSP64464.2024.10867018) at ICMSP 2024.

**Related publication:** [Motion Is All You Need](/publications/motion-is-all-you-need/).
