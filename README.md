# Plant Species Identification Using CNN


## Overview
This project focuses on identifying plant species using a Convolutional Neural Network (CNN). The dataset consists of images of 1800 plants belonging to 32 different classes. The images were resized to 64x64 pixels and normalized before training. Data augmentation was applied to improve the model's robustness.

## Dataset
- **Classes**: 32 plant species
- **Total Images**: 1800
- **Image Preprocessing**: Resized to 64x64 pixels, normalized

## Data Augmentation
- **Data Augmentation**: Applied using Keras' `ImageDataGenerator` to enhance the dataset by creating modified versions of images, which helps improve model generalization.

## Model Architecture
The Convolutional Neural Network (CNN) model used for this project consists of the following layers:
1. **Convolutional Layers**: Three convolutional layers with increasing filter sizes (32, 64, 128) and ReLU activation functions. These layers help in extracting features from the input images.
2. **Max Pooling Layers**: Three max pooling layers following each convolutional layer to downsample the feature maps and reduce dimensionality.
3. **Fully Connected Layers**: Two dense (fully connected) layers with 128 and 64 neurons respectively, using ReLU activation functions to learn complex patterns.
4. **Output Layer**: A dense layer with 32 neurons (one for each class) and a softmax activation function to output class probabilities.

## Results
The performance of the model was evaluated using accuracy and loss metrics, plotted alongside a confusion matrix and ROC curves for each class.

### Model Accuracy and Loss
- ![Accuracy](https://i.ibb.co/tmjgCJm/ma.png)
- ![Test Loss](https://i.ibb.co/hDGgcty/mb.png)
- ![Test Accuracy](https://i.ibb.co/hydrsVv/mc.png)
### Confusion Matrix
- ![Confusion Matrix](https://i.ibb.co/dLkdZDR/md.png)

### ROC Curve
- ![ROC Curve](https://i.ibb.co/6nmwZRR/me.png)
