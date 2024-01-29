# TensorFlow-Stanford-Dogs-Classifier

This is a simple image classification project using TensorFlow and the Stanford Dogs dataset. The goal is to train a model to classify dog breeds from the dataset.

## Dataset
The project uses the Stanford Dogs dataset which consists of 20,580 images of 120 breeds.

Training Set: 12000 <br>
Test Set: 8580 <br>
Number of Classes: 120 <br>

## Model Architecture <br>
The model is based on MobileNetV2, a lightweight deep-learning model suitable for mobile and embedded vision applications. The top layers of the MobileNetV2 are frozen, and a custom classification head is added for fine-tuning on the Stanford Dogs dataset.

## Training <br>
The model is trained for 10 epochs with a batch size of 32. The training process is monitored using callbacks, including ModelCheckpoint, TensorBoard, and EarlyStopping.

## Evaluation <br>
After training, the model is evaluated on the test set and the **test accuracy of 83.92%** is reported.

## Visualization <br>
A function visualize_predictions is implemented to visualize predictions on a batch of test data. It shows the actual and predicted classes along with the images. <br>
![image](https://github.com/arqumk/TensorFlow-Stanford-Dogs-Classifier/assets/130319866/86e2398c-7e60-4042-b6c9-890486b49c93)


**How to Use** <br>
Clone the repository:

`git clone https://github.com/{username}/{repository}.git`

Install dependencies:

`pip install -r requirements.txt`


Feel free to adapt the code and experiment with different hyperparameters or models for further improvements.

**License**
This project is licensed under the MIT License - see the LICENSE file for details.
