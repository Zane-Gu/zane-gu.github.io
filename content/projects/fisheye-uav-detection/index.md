---
title: "Fisheye UAV Obstacle Detection"
date: '2023-09-01'
summary: "Segmentation-based training and knowledge distillation for fisheye UAV obstacle detection."
image:
  alt_text: "Schematic fisheye UAV view, segmentation masks, and object detections"
  caption: "Original schematic of the AirEyeSeg training and detection workflow; not an experimental image."
---

**MSc individual research project · Imperial College London · December 2022–September 2023**

Supervised by Professor [Krystian Mikolajczyk](https://profiles.imperial.ac.uk/k.mikolajczyk) at [MatchLab](https://www.imperial.ac.uk/matchlab/).

### Situation

Fisheye cameras give UAVs a wider field of view, but their radial distortion changes the appearance of people, vehicles, and other obstacles—especially near the image edge. Conventional detectors trained on perspective images can struggle with this geometry, while annotated fisheye UAV data are limited.

### Task

I set out to develop a real-time obstacle detector that could learn from fisheye imagery and generalize beyond a single camera setting. This required both suitable training data and a way to obtain useful segmentation labels without manually annotating every distorted image.

### Action

I constructed fisheye-formatted UAV datasets and investigated a teacher–student training strategy. The [Segment Anything Model (SAM)](https://github.com/facebookresearch/segment-anything) served as the segmentation teacher, producing masks for distorted training images; a YOLOv8-based student learned to detect and segment obstacles from those labels. In the [AirEyeSeg paper](https://doi.org/10.5220/0012388600003654), we compared this approach with ground-truth-based training and evaluated it across UAV datasets, including VisDrone, UAVid, DDOS, and a separate SEE test set.

### Result

The paper reports **88.6% mask mAP@0.5 for cars** on the combined VisDrone/UAVid evaluation and **84.5% box precision for people** on SEE. These are different metrics on different datasets, not a single overall accuracy figure. AirEyeSeg received the [Best Student Paper Award at ICPRAM 2024](https://icpram.scitevents.org/PreviousAwards.aspx#2024); my MSc project received a mark of 79.55%.

**Research outputs:** [AirEyeSeg publication](/publications/aireyeseg/) · [Project code](https://github.com/Zane-Gu/AirEyeSeg).
