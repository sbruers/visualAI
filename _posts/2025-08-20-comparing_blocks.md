---
title: "CNN Block Architecture Comparison"
layout: single-project
category: CNN
image: /assets/images/blocks_with_skips.png
description: "A visual comparison of popular convolutional blocks used in CNN architectures, highlighting the different types of building blocks (convolutions, skip connections, and activation functions)."
permalink: /projects/cnn-block-comparison/
---

This project provides a **visual overview of various convolutional neural network (CNN) blocks**. 

The figure compares the following blocks:

- **Inception (2014)** – multiple convolutional paths concatenated.  
- **Residual Block (2015)** – classic skip connections with basic convolutions.  
- **Bottleneck Block (2015)** – expanded channel dimension with pointwise convolutions.  
- **SqueezeNet & Squeeze-and-Excite (2016–2017)** – efficient network design with excitation mechanisms.  
- **MobileNet v1 & v2 (2017–2018)** – depthwise separable convolutions for efficiency without and with skips 
- **MobileNet v3 (2019)** – improved nonlinearities (Hardswish) and pooling. 
- **ConvNext v1 & v2 (2022–2023)** – modern transformer-style normalization and scaling.  

The visualization uses **color coding** for convolution types, activation functions, pooling, and other operations. Skip connections, concatenations, and additions are clearly indicated to show how information flows through each block.

![CNN Block Comparison]({{site.baseurl}}/assets/images/blocks_with_skips.png)

