# Alzheimer's Disease Classification and Prediction using CNN

## Introduction

Alzheimer's disease (AD) is the most prevalent form of dementia, caused by damage or death of nerve cells and their connections in the brain. This project presents a comprehensive investigation into Alzheimer's stages classification and prediction using the ADNI MRI dataset with Convolutional Neural Networks (CNN).

## Dataset

We utilized the Alzheimer's Disease Neuroimaging Initiative (ADNI) MRI dataset for this study. The dataset was resized to (100, 100) and converted to greyscale for processing. Preprocessing included zooming and recycling while keeping flips as false, considering the importance of orientation in MRI datasets.

## Data Splitting

The dataset was divided into training, testing, and validation sets in an 8:1:1 ratio.

## Model Architecture

Our CNN model consists of multiple convolutional layers, batch normalization layers, and dropout layers to control overfitting. The activation function used was leaky ReLU, and the model was compiled using the Adam optimizer and Categorical Cross Entropy loss function.

## Hyperparameter Tuning

We used Keras' random hyperparameter tuner in a loop with 5 trials, considering validation accuracy to obtain the best model.

## Results

- CN (Cognitively Normal): 97%
- EMCI (Early Mild Cognitive Impairment): 96.95%
- LMCI (Late Mild Cognitive Impairment): 99.99%
- MCI (Mild Cognitive Impairment): 99.23%
- AD (Alzheimer's Disease): 99.99%

The best model achieved an overall accuracy of 97.86%, with F1_scores ranging from 0.98 to 1.00. Evaluation was done using a confusion matrix and classification report, demonstrating better performance compared to other models developed using the ADNI dataset with CNN.




## Getting Started

### Prerequisites

- Python 3.7+
- TensorFlow
- Keras
- NumPy
- Pandas
- Scikit-learn
- Matplotlib

## Evaluation

Evaluation was performed using a confusion matrix and classification report. The results indicate a high accuracy and F1_score for different stages of Alzheimer's disease.

## Conclusion

This project demonstrates an effective method for classifying and predicting various stages of Alzheimer's disease using the ADNI MRI dataset with CNN. The model achieved a high accuracy of 97.86% and shows promise for early detection and diagnosis of Alzheimer's disease.

## References

- ADNI dataset: [ADNI](http://adni.loni.usc.edu/)
- Keras Documentation: [Keras](https://keras.io/)
- TensorFlow Documentation: [TensorFlow](https://www.tensorflow.org/)
- IEEEExplore Documentation: [PaperLink](https://ieeexplore.ieee.org/abstract/document/10797591/)

## Acknowledgements

We would like to thank the Alzheimer's Disease Neuroimaging Initiative (ADNI) for providing the dataset used in this study.

## Disclaimer

GNU AFFERO GENERAL PUBLIC LICENSE
                       Version 3, 19 November 2007

 Copyright (C) 2024  Rudra Prasanna Mishra

 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU Affero General Public License as published
 by the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.

 This program is distributed in the hope that it will be useful,
 but WITHOUT ANY WARRANTY; without even the implied warranty of
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 GNU Affero General Public License for more details.

 You should have received a copy of the GNU Affero General Public License
 along with this program.  If not, see <https://www.gnu.org/licenses/>.



