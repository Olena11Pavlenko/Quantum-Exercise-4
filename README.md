Soil Erosion Detection using CNN

This codebase contains the implementation of a Convolutional Neural Network (CNN) model for detecting soil erosion in satellite images.

Dataset

The model has been trained on a dataset of satellite images, which has been annotated for soil erosion regions.

Model

Model Architecture

The UNet model is defined in the build_unet function. The function takes an input image shape as a parameter and returns a Keras Model object. The architecture consists of a contraction path, which captures the context of the image, and an expansive path, which refines the segmentation. The final layer is a convolutional layer with a sigmoid activation function, which outputs a probability map for the segmentation.

Training

To train the model, you can use any dataset that has been annotated for segmentation. The model is trained using binary cross-entropy loss and the Adam optimizer. 

Testing

To test the trained model, you can use the predict method of the model object. The predict method takes an input image as a parameter and returns a probability map for the segmentation. You can threshold the probability map to obtain the final segmentation mask. 

Results

The trained model achieves an accuracy of 74,63% on the test dataset. It can be improved by increasing data for training. 