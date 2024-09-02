### This repository is created for submission of the Intermediate Level Problem Statement of hackathod "What the HACK" for induction of Machine Learning Club at Indian Institute of Technology, Gandhinagar. <br>
## Problem Statement:
Problem Statement: Develop a neural network that learns to apply the Sobel filter to images.
Tasks:
Dataset Preparation:
Use the provided dataset of images.
Apply the Sobel filter to the dataset using a standard image processing library.
Save the original and Sobel-filtered image pairs.
Model Development:
Design a neural network that takes an original image as input and produces a Sobel-filtered image as output.
Training:
Train your model using the prepared dataset.
Evaluation:
Evaluate your model's performance on a provided test set.

## Methodology Used 
1. Preparing the Training and Test Dataset by applying Sobel filter on dataset using OpenCV.
<br>
2. Training the Model on the dataset.<br>
    a. Model Architecture: I have used 3 Convolution Layers along with Max Pooling layers with ReLU activation Function to capture the edges in the image. Moreover, 3 Convolution Transpose Layers are used to restore the shape of the model output to Image size.
<br>
3. Testing the Model <br>The Model is tested on a 2500 images sampled randomly from the dataset.

### Results and Discussion
- Several different models were tried like CNN with different number of Convolutional layers, with and without dropouts, changing the kernel size and padding. THe best model till now is illustrated in the notebook
- The training loss decreased from initial value of 1 to 0.02 which suggests that model is able to recognize the patterns present in the dataset.
- By plotting the outputs and comparing with sobel filtered image, we can conclude that model is able to identify all major edges and a few minor edges. However, it cannot still get the very fine details of the image. This can be resolved by adding some Fully Connected Layers, or more Convolutional layers. However, due to limitation of computational resources, it is not done now.

  ![image](https://github.com/user-attachments/assets/502134b8-f209-440d-94fc-c61e4a129aca)
