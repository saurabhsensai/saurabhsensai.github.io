---
title: "Hybrid Loss Functions in U-NET for Kidney Blood Vessel Segmentation in HiP-CT Images"
excerpt: "Short description of portfolio item number 1<br/><img src='/images/saurabh/unet/portfolio1.png'>"
collection: portfolio
---

This study focuses on improving kidney blood vessel segmentation using U-NET models with a custom hybrid loss function. High-resolution peripheral computed tomography (HiP-CT) images are used to train the segmentation model. A novel weighted loss function combining Log-Cosh Dice Loss and Binary Cross-Entropy is introduced to enhance segmentation performance. The model is compared with state-of-the-art architectures, including Vanilla U-NET, Attention U-NET, Recurrent Residual U-NET, LinkNet, and UNETR. The results demonstrate superior segmentation accuracy, Dice coefficient, sensitivity, and specificity for all tested kidney datasets.

Key Contributions:

-Preprocessing Techniques: Applied gamma correction and image partitioning to improve contrast and segmentation accuracy.

-Custom Loss Function: Combines Log-Cosh Dice Loss with Binary Cross-Entropy to balance segmentation performance and optimize Dice coefficient.

-Comparative Analysis: Evaluated multiple deep learning architectures, demonstrating that the proposed U-NET model with a hybrid loss function outperforms existing methods.

-Performance Metrics: Achieved high accuracy, Dice coefficient, and specificity, ensuring precise segmentation for different kidney types.


Architecture Used: 

<figure>
  <img src="/images/saurabh/unet/unet.png" alt="U-NET Architecture" width="600">
  <figcaption style="text-align: center;">Figure 1: U-NET Architecture used for segmentation</figcaption>
</figure>


<figure>
  <img src="/images/saurabh/unet/transformer.png" alt="UNETR Architecture" width="600">
  <figcaption style="text-align: center;">Figure 2: UNETR Architecture used for segmentation</figcaption>
</figure>

Results achieved: 

<figure>
  <img src="/images/saurabh/unet/results.png" alt="Results" width="600">
</figure>
