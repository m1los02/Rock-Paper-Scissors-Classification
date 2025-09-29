# Rock-Paper-Scissors-Classification

This project implements a simple image classification system for the Rock–Paper–Scissors game using hand gesture images.
The goal was to test how well basic handcrafted features, using classical image processing, combined with simple classifiers can distinguish between classes.
The classification was based on only two features.

Two features were extracted from preprocessed binary images:
- White pixel percentage in the left section of the hand (from 1/7.5 to 1/2.5 of image width).
- Centroid ratio: centroid’s x coordinate divided by its y coordinate. Centroid was calculated afte distance transformation of binary image.

These features are computed after converting the image to HSV, applying binary thresholding, morphological operations, and cropping to remove the background.

Classification was done on 3 classes by Bayesian classifier (minimum error probability) and I achieved ~96% accuracy.

Also I experimented on classification of 2 classes (rock vs scissors), where I used linear classifier and achieved 100% accuracy.
