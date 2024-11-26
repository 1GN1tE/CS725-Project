# CS725-Project

<!-- About -->
## About Project

Objective of our project is to classify 25 distinct Indian bird species using machine learning techniques.

The dataset that we have used is Indian-Birds-Species-Image-Classification.
It consist of 25 bird species found in India,
Each species has 1,500 images in the dataset.
The dataset contains a total of 37,500 images split into train and validation sets in an 80:20 ratio, with 30,000 images in the training set and 7,500 images in the test set.

As there are 25 Bird species in the dataset we have label encoded the images(0 to 24).

We have splitted the data into train, test and validation sets with the sizes 64%, 16% and 20% where each set has equal number of samples for each label.
Passed the training data through an augmentation layer which randomly flips and resizes the images.

Training a full neural network from scratch is time consuming. So, we used some pretrained CNNs and applied two layers on it. We used a variety a pretrained CNNs and showed their results.

Models:
ResNet 50 (Trainable params: 1,186,841)
EfficientNet V2 B0 (Trainable params: 793,625)
MobileNet V2 (Trainable params: 793,625)
Vision Transformer (Trainable params: 531,481)

And lastly ensemble all the above models with averaging (geometric mean and Linear mean).

## Our Model Architecture:
![image](https://github.com/user-attachments/assets/45a493e9-7234-4174-b8ff-0ae6ce680ef9)

## Results

### ResNet 50
<div style="display: flex; gap: 10px;">
  <img src="https://github.com/user-attachments/assets/8c5e301d-a5c2-48c7-9c47-537a1af8dbba" width="300" height="300" />
  <img src="https://github.com/user-attachments/assets/16fbf790-2b79-47a3-b20c-5b48e881eafb" width="300" height="300" />
</div>

### EfficientNet V2
<div style="display: flex; gap: 10px;">
  <img src="https://github.com/user-attachments/assets/9bdc0558-2307-4aee-97b9-035008479ccb" width="300" height="300" />
  <img src="https://github.com/user-attachments/assets/67bcd806-36cf-4d61-adf7-23fdbfa54e83" width="300" height="300" />
</div>

### MobileNet V2
<div style="display: flex; gap: 10px;">
  <img src="https://github.com/user-attachments/assets/954c2a58-7108-4f24-b287-9255661371c4" width="300" height="300" />
  <img src="https://github.com/user-attachments/assets/ea8aead9-5e4f-4d26-a9df-1ceb9be9ce0a" width="300" height="300" />
</div>

### ViT B32
<div style="display: flex; gap: 10px;">
  <img src="https://github.com/user-attachments/assets/053d6e0a-8966-4e83-9de4-a0c326254ffa" width="300" height="300" />
  <img src="https://github.com/user-attachments/assets/e7316503-f9d6-4fef-b5b3-cb2e330ed47d" width="300" height="300" />
</div>

### Performance Metric

<img width="543" alt="pm" src="https://github.com/user-attachments/assets/3c58fe9c-d6bb-49f0-8303-027acfd6ff2d">

## Analysis

EfficientNetV2 gives better accuracy than ResNet50 even with lesser parameters.
EfficientNet also outperformed ViT-b32.
Ensemble gives the best accuracy with the highest Mathews Correlation Coefficient (MCC) so it will also generalize to unseen samples.

## Evaluation

<!-- Predictions, scores -->

## Running

Set up environment in kaggle / colab:
```sh
pip install requirements.txt
```
<!-- Import the following dataset in kaggle / colab: -->

## References

