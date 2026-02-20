


# Convolutional Neural Networks

## Authors

Manish Kumar Panday – [[GitHub link here]()]  
Anne Valvezan – [[GitHub link here](https://github.com/coffeedrunkpanda)]

## Project Overview
This project investigates the performance differences between locally constructed Convolutional Neural Networks (CNNs) and transfer‑learning models when applied to the CIFAR‑10 dataset (32×32×3 images).
Key areas explored include:

The design and behaviour of custom CNN architectures.
A conceptual breakdown of CNN components (included in the accompanying presentation).
How pretrained models perform when forced to operate on extremely low‑resolution images.
The influence of selectively unfreezing layers within transfer‑learning models.

The experiments reveal how architectural choices and trainable‑layer configurations impact accuracy, often in unexpected ways, and suggest avenues for further study.

- A small side note: The use of older deprecated methodolgy in terms of tensorflow and keras, which limited some image augmentation methods. Further efforts will use more modern layer base approaches.

## Summary of Experiments

Across the project, 13 models were developed and trained. These models varied in:

- Custom-built vs. transfer‑learning architectures
- Input resolution
- Number and placement of unfrozen layers in transfer models

A central conclusion is that transfer learning is computationally efficient only when the pretrained architecture aligns with the target task. Repurposing large, high‑resolution models for inappropriate datasets can be unnecessarily resource‑intensive and yield limited benefits.

## Key Findings

Well‑designed custom CNNs can perform competitively on CIFAR‑10.
Transfer‑learning models often underperform when forced to process undersized images.
The choice of which layers to unfreeze has a significant — and sometimes surprising — effect on performance.
There are clear opportunities for further experimentation in architecture design, different data augmentation methods, and layer‑freezing strategies.
