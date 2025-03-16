# Medical-Image-DL-Classification

## Abstract

The medical image analysis field, traditionally attributed to clinical radiologists, has
also seen enormous advancements as a result of the recent Artificial Intelligence-
fuelled image analysis boom, with the introduction of advanced deep learning
models such as deep convolutional neural networks and vision transformers.
Here, we dive into some of the associated challenges of adopting such a new
technology in a clinical setting, including model interpretability and training of
such models. Various deep neural network models are proposed and trained on
chestMNIST, a publicly available dataset of chest X-Rays. Models are compared
to previously published benchmarks and results and implications are discussed.

Code is available in: https://colab.research.google.com/drive/1IuAH_wrK0HGx7tHjEmbbVJI4NgCApBT7?usp=sharing

## 1 Introduction

Deep learning (DL) models for image data analysis have been at the forefront of recent advancements,
with recent introduction of state-of-the-art architectures such as ResNet (He, 2016) and DenseNet
(Huang, 2017), which are both based on the traditional convolutional neural network (CNN) architec-
ture, and the more modern Vision Transformer (ViT, Dosovitskiy, 2021). However, the adoption of
such models has not been equally quick to spread across different domains, particularly in highly
regulated industries such as healthcare and clinical settings, which pose particular barriers for adop-
tion such as high reliability, safety, and regulatory compliance requirements. As stated by Chan et al.
in 2019, there have been numerous speculations about the future of radiologists as medical profes-
sionals given the impressive advancements in machine learning and Artificial Intelligence. However,
developing DL models capable of performing as good or better than trained clinical radiologists is no
easy task.

## 5 Conclusion

### 5.1 Summary of Findings

Deep learning models including deep CNN’s and Vision Transformers show great promise in chest
X-ray image analysis (and medical image analysis as a whole), but this comes with a unique set of
challenges, including trade-off between model complexity and interpretability, performance, and
clinical use adoption.
Among the different models of various complexities trained, the DenseNet architecture was found to
yield consistently solid performance (across the various depths), moderate training time compared to
other models, and achieve comparable performance to benchmarks found in literature.

### 5.2 Limitations and Future Work

One of the main constraints in this work has been computational resources, especially when compared
to the computational costs of model training. Furthermore, the choice of using 224 x 224 resolution
images rather than smaller sizes (smallest resolution available directly from data source is 28 x 28)
contributed to the long training times, but allowed models to learn from images which contain more
information. This has also contributed to a suboptimal hyperparameter tuning effort.
Future work would include performing more robust hyperparameter tuning for each model architecture
in order to find the optimal set of parameters required for best training. Likewise, effects of increased
training epochs on performance would be an interesting key aspect to study, with the hopes of
increasing all of accuracy, sensitivity, and specificity, in order to yield better overall predictive
capabilities.
