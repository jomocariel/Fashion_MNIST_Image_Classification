# Fashion_MNIST_Image_Classification
Google Colab Link: https://colab.research.google.com/drive/1nez7MNjZrZAH9CE8JToEmwO1D4mitJxE#scrollTo=-lFrI1z_0STF
Questions: (February 8, 2026)
1. What is the Fashion MNIST dataset?
   ANS: A collection of tiny grayscale photos of apparel items, including as shirts, shoes, and bags, make up the Fashion MNIST dataset. Each 28x28 pixel image falls into one of ten fashion categories. It is frequently used to practice machine learning-based picture classification.
   
2. Why do we normalize image pixel values before training?
   ANS: The initial range of image pixel values was 0 to 255.
By dividing by 255, normalization scales these values to a range of 0 to 1.
This is beneficial:
Accelerate the training of models
Boost the stability of numbers
Give the neural network additional time to converge.

3. List the layers used in the neural network and their functions.
   ANS: Layer flattening creates a 1D array of 784 pixels from the 28x28 image.
Dense layer (ReLU activation, 128 neurons) gains knowledge of the image's key elements and patterns.
Ten neurons make up the dense output layer. Generates logits, or raw scores, for each of the ten clothing classes.

5. What does an epoch mean in model training?
   ANS: One whole run of the training dataset through the neural network is referred to as an epoch.
The model was trained for ten epochs in your notebook, which means it saw all of the training data ten times.

7. Compare the predicted label and actual label for the first test image.
   ANS: In the first test image, the model's prediction is directly compared to the label from the Fashion-MNIST dataset. This image's true label is "Ankle boot," which corresponds to the right category in the dataset. If the model also predicts "Ankle boot," it indicates that it accurately identified the image. If it forecasts a different class, this is considered a misclassification, indicating that the model's ability to distinguish between comparable clothing items need further refinement.
   
9. What could be done to improve the model’s accuracy?
   ANS: To improve the accuracy of the model, add more layers or neurons to allow it to learn more detailed information from the photos. Using strategies like as **dropout** and **data augmentation** can improve model generalization and prevent overfitting. Increasing the number of training epochs, adjusting the learning rate, or using a **convolutional neural network (CNN)** instead of a simple dense model can all dramatically improve performance, as CNNs are considerably better at recognizing patterns in images.
