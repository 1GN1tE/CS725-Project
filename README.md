# CS725-Project

<!-- About -->

## Evaluation

<!-- Predictions, scores -->

## Running

Set up environment in kaggle / colab:
```sh
pip install requirements.txt
```
<!-- Import the following dataset in kaggle / colab: -->

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

And lastly ensemble all the above models with averaging (geometric mean).

Our Model Architecture:
![image](https://github.com/user-attachments/assets/45a493e9-7234-4174-b8ff-0ae6ce680ef9)


## References

