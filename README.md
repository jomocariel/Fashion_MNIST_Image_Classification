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
4. What does an epoch mean in model training?
   ANS:One whole run of the training dataset through the neural network is referred to as an epoch.
The model was trained for ten epochs in your notebook, which means it saw all of the training data ten times.
6. Compare the predicted label and actual label for the first test image.
   ANS:
8. What could be done to improve the model’s accuracy?
