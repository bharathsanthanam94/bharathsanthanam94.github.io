---
title: "Traffic sign data augmentation using CycleGAN"
excerpt: " Deployed a CycleGAN model that takes a standard version of traffic signs and performs style transfer to make them look like ones captured in real-life scenarios.<br/><img src='/images/CycleGAN_sample.png'>"
collection: portfolio
---
### Overview

Data imbalance is a critical problem in deep learning where some classes have fewer examples than others. This issue is particularly noticeable in traffic sign datasets, where imbalanced data can cause classifiers to perform poorly during inference.  We have developed a method for more realistic data augmentation of underrepresented classes using a style-transfer approach. Our method uses a CycleGAN model that takes prototype German traffic signs as input and transforms them to look like real-life signs captured on roads. These generated images are then added to the dataset and used to train a more robust classification model.

### Key steps

- Take prototype images of traffic signs from this [link](https://en.wikipedia.org/wiki/Road_signs_in_Germany)
- Perform perspective transformation to the signs and pass it to the CycleGAN model, it translates the sign to look like a real-life traffic sign.

### Evaluation

- We evaluate the generated images using Frechet Inception Distance (FID)[ link](https://arxiv.org/pdf/1706.08500)
- We also augment these generated images to the existing datasets and check for classifier accuracy


![GAN](/images/GAN_flowchart.png)
