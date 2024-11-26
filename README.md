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
  <img src="https://github.com/user-attachments/assets/8c5e301d-a5c2-48c7-9c47-537a1af8dbba" width="300" />
  <img src="https://github.com/user-attachments/assets/16fbf790-2b79-47a3-b20c-5b48e881eafb" width="300" />
</div>

### EfficientNet V2
<div style="display: flex; gap: 10px;">
  <img src="https://github.com/user-attachments/assets/9bdc0558-2307-4aee-97b9-035008479ccb" width="300" />
  <img src="https://github.com/user-attachments/assets/67bcd806-36cf-4d61-adf7-23fdbfa54e83" width="300" />
</div>

## Evaluation

<!-- Predictions, scores -->

## Running

Set up environment in kaggle / colab:
```sh
pip install requirements.txt
```
<!-- Import the following dataset in kaggle / colab: -->

## References

