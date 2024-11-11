# Bone Fracture Detection in Pediatric Wrist Trauma X-ray Images

This project focuses on detecting bone fractures in pediatric wrist trauma X-ray images using the state-of-the-art YOLOv8s model. By leveraging advanced image processing techniques and a carefully curated dataset, we aim to improve detection accuracy and support healthcare professionals in early fracture diagnosis.

---
<img src="https://github.com/AymanAitAhmed/bone-fracture-detection-grazpedwri-dx/blob/main/images/bone%20fracture%20cover.jpg" >

## Overview

Pediatric wrist fractures are among the most common injuries, and rapid, accurate detection is crucial for effective treatment. This project explores the application of deep learning to assist in fracture detection using X-ray images, with a focus on performance optimization and model accuracy.

## Dataset

- **Dataset Used**: The [GRAZPEDWRI-DX]([https://www.kaggle.com/datasets/jasonroggy/grazpedwri-dx]) dataset, a specialized collection of pediatric wrist X-rays, was used in this study. The dataset includes various cases of fractures and non-fractures, providing a robust basis for training and testing the model.

## Model

- **YOLOv8s**: A pre-trained YOLOv8s model was selected for this project due to its efficiency in object detection and high accuracy in medical image applications.
- The model was fine-tuned specifically for fracture detection in pediatric wrist X-rays, allowing it to adapt to the unique characteristics of pediatric bone structures.

## Image Preprocessing

To maximize model performance and enhance the visibility of fracture details, we applied various image transformations, including:
- **HE** (Histogram Equalization)
<img src="https://github.com/AymanAitAhmed/bone-fracture-detection-grazpedwri-dx/blob/main/images/wrist_xray_HE.png">

- contrast limited adaptive histogram equalization(CLAHE):
<img src="https://github.com/AymanAitAhmed/bone-fracture-detection-grazpedwri-dx/blob/main/images/wrist_xray_CLAHE.png">

### Libraries Used

The following libraries were critical for implementing image transformations and model training:

- **[Albumentations](https://albumentations.ai/)**: Used for advanced image augmentations and transformations to improve the model’s robustness and performance.
- **[OpenCV](https://opencv.org/)**: Utilized for image processing tasks, including CLAHE and HE transformations.

## Results and Observations

The model's performance was analyzed using various metrics, such as confusion matrix, mAP50 and mAP95. The impact of each image transformation method on these metrics was carefully evaluated, offering insights into optimal preprocessing techniques for pediatric wrist X-rays.

---

Feel free to explore the project and adapt the provided methods to similar applications. For more details, please refer to the code and documentation in each module.

