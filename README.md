# Cellular-Composition-Prediction-with-CNN-Transfer-Learning

In this project, we develop Machine Learning regression models with 1) Classical Machine Learning methods, 2) Kernel Support Vector Regression (SVR), and 3) Convolutional Neural Networks (CNN), to predict the number of six different types of cells, as well as the total number of cells, in a given histological image patch. The counts of different types of cells in a given image patch is known as the cellular composition.

In particular, we first perform Exploratory Data Analysis (EDA) and feature extractions on our dataset, following by image pre-processing. We then train our baseline models with classical Machine Learning methods including i) Ordinary Linear Regression, and ii) Support Vector Regression, which are implemented with the Python sklearn package. Finally, we harness the power of CNN transfer learning by finetuning a pretrained ResNet model on our dataset and compare its performance with our baseline models.

## Discussion

With limited computational resources and time give, we believe that, at this stage, it is virtually impossible to accurately predict the number of Cell Type 1 and Cell Type 5 (at least, not by minimizing MSE between actual counts and predicted counts), due to its 'rareness' in the pictures we train the model on. The overfitting suggests that the models failed to capture the characteristics of these two cells, but instead, blindly memorize the map between the inputs and the outputs. We suggest the use of segmentation and classification (e.g. HoverNet-based architecture) to better tackle this problem, but we are currently unable to perform such training here in this project.

## Conclusions 

We demonstrated how manual feature extractions and classical machine learning methods (e.g. OLS, SVM) struggle to capture the meaning in predicting total number of cells in a given image patch, and how CNN transfer learning overcomes this problem.

We also demonstrate the power of CNN transfer learning to predict the cellular composition, which is partially successful. We noticed the limitation of our models taking the whole image as an input in some predictions with smaller target values (i.e. rarer cells) and suggested the use of more advanced methods like segmentation in future appraoches.

