# Cellular-Composition-Prediction-with-CNN-Transfer-Learning

In this project, we develop Machine Learning regression models with 1) Classical Machine Learning methods, 2) Kernel Support Vector Regression (SVR), and 3) Convolutional Neural Networks (CNN), to predict the number of six different types of cells, as well as the total number of cells, in a given histological image patch. The counts of different types of cells in a given image patch is known as the cellular composition.

In particular, we first perform Exploratory Data Analysis (EDA) and feature extractions on our dataset, following by image pre-processing. We then train our baseline models with classical Machine Learning methods including i) Ordinary Linear Regression, and ii) Support Vector Regression, which are implemented with the Python sklearn package. Finally, we harness the power of CNN transfer learning by finetuning a pretrained ResNet model on our dataset and compare its performance with our baseline models.
