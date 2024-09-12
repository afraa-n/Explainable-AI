## Assignment 2: Explainable AI - Adversarial Patches (Ice Cream Edition)

This project demonstrates the creation and application of adversarial patches using a pre-trained ResNet34 model. The goal is to design an adversarial patch that causes the model to incorrectly classify images as "ice cream." 

#### Overview

In this project, an adversarial patch is generated and tested on several images. The patch is designed to look like an ice cream scoop, aiming to fool the ResNet34 model into classifying the image as "ice cream," regardless of its actual content.

#### Steps Used

1. **Preparing the Model**:
   - A pre-trained ResNet34 model is loaded and set to evaluation mode for inference.
   - Target class "ice cream" is identified.
   - Image preprocessing transformations are defined to format input images for the ResNet34 model.

2. **Image Handling Helper Functions**:
   - Functions are created to load images from URLs and preprocess them.
   - A function is also included to display these images.

3. **Creating an Ice Cream Patch**:
   - An adversarial patch is created to resemble an ice cream scoop. The patch is initialized with a light cream color and a swirl texture to mimic ice cream.

4. **Generating the Adversarial Patch**:
   - The adversarial patch is generated through optimization. The patch is applied to various test images, and the model's predictions are evaluated to ensure the patch effectively causes misclassification.
   - The patch is updated based on the loss calculated from the model's predictions, with gradients managed to prevent instability.

5. **Testing**:
   - Multiple test images are loaded.
   - The generated adversarial patch is applied to the test images, and results are displayed, including the model's predictions and confidence scores.

### Results

The adversarial patch causes the ResNet34 model to misclassify various images as "ice cream." Below is an example of the generated adversarial patch:

![Adversarial Patch](https://github.com/user-attachments/assets/4ed89f1c-4a25-417e-83fe-aa073d5ee5a2)


### Credits

This was developed with assistance from Claude AI for optimizing the adversarial patch generation process.
