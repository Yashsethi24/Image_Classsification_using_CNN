# CIFAR-10 and CIFAR-100 Model Training and Transfer Learning

Overview

This project involves training deep learning models on CIFAR-10 and CIFAR-100 datasets using convolutional neural networks (CNNs). It explores training CIFAR-10 from scratch and applying transfer learning to fine-tune a CIFAR-100 model.

Model Training Details

CIFAR-10: Trained from scratch using the best hyperparameters, achieving a final validation accuracy of 91.93% after 50 epochs.

CIFAR-100 (Transfer Learning): Initialized with CIFAR-10 trained weights and fine-tuned, achieving a final validation accuracy of 68.48% with early stopping.

CIFAR-100 (Trained from Scratch): The highest validation accuracy obtained was 67.80% (refer to PPar-3_Hyper-parameter-tuning-CIFAR-100.ipynb).

Key Findings

Transfer learning from CIFAR-10 to CIFAR-100 resulted in higher accuracy (68.48%) compared to training CIFAR-100 from scratch (67.80%).

Visualizations of feature maps from different layers show how feature extraction varies between trained models.

Dataset Information

CIFAR-10: Contains 60,000 images across 10 classes (6,000 per class), split into 50,000 training and 10,000 test images.

CIFAR-100: Contains 60,000 images across 100 classes (600 per class), with the same train-test split.

Setup Instructions

Prerequisites

Ensure you have Python installed along with the required libraries.

pip install torch torchvision matplotlib numpy

Running the Code

Clone the repository:

git clone https://github.com/Yashsethi24/Image_Classsification_using_CNN.git
cd Image_Classsification_using_CNN

Train the CIFAR-10 model:

python train_cifar10.py

Fine-tune CIFAR-100 with transfer learning:

python fine_tune_cifar100.py

View feature maps:

python visualize_feature_maps.py

Results and Analysis

The trained models, evaluation metrics, and visualizations can be found in the results/ directory.

Check the Jupyter notebooks for detailed experiments and hyperparameter tuning logs.

License

This project is licensed under the MIT License - see the LICENSE file for details.

