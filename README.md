# CIFAR-10 & CIFAR-100 Model Training and Transfer Learning

## Overview
This project explores model training and transfer learning using the CIFAR-10 and CIFAR-100 datasets. The CIFAR-10 model was trained from scratch, and its learned weights were used to fine-tune a CIFAR-100 model. Performance comparisons were conducted with and without transfer learning.

## Datasets
- **CIFAR-10**: Contains 60,000 images across 10 classes (e.g., airplanes, cars, birds).
- **CIFAR-100**: Contains 60,000 images across 100 classes (more fine-grained categories).

## Model Training and Performance
### **CIFAR-10 Model**
- Trained from scratch using optimized hyperparameters.
- **Final validation accuracy**: **91.93%** after 50 epochs.

### **CIFAR-100 Model**
- Initialized using **pretrained CIFAR-10 weights** and fine-tuned.
- **Final validation accuracy**: **68.48%** (early stopping applied).

### **Comparison with Non-Transfer Learning**
- A CIFAR-100 model was also trained **from scratch**.
- **Best accuracy achieved**: **67.80%**  
  *(Refer to `Part-3_Hyper-parameter-tuning-CIFAR-100.ipynb` for details.)*

## Visualizations
The following visualizations were generated during the experiments:
- **Feature maps** from different convolutional layers.
- **Class activation maps** highlighting important regions for classification.
- **Prediction visualizations** showing model performance on test images.

## Setup & Installation
To run this project locally, follow these steps:

1. Clone the repository:
   ```bash
   git clone https://github.com/Yashsethi24/Image_Classsification_using_CNN.git
   cd Image_Classsification_using_CNN
   ```
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
3. Train the model:
   ```bash
   python train.py
   ```
4. Evaluate the model:
   ```bash
   python evaluate.py
   ```

## Results & Insights
- Transfer learning significantly improved **CIFAR-100 performance**.
- **Feature maps comparison** showed better generalization using pretrained weights.
- **Early stopping and hyperparameter tuning** played a crucial role in model convergence.

## References
- CIFAR-10 & CIFAR-100 datasets: [https://www.cs.toronto.edu/~kriz/cifar.html](https://www.cs.toronto.edu/~kriz/cifar.html)
- Research on Transfer Learning: [https://arxiv.org/abs/1606.09275](https://arxiv.org/abs/1606.09275)

## Author
👤 **Yash Sethi**  
📧 [yash.sethi@mail.mcgill.ca](mailto:yash.sethi@mail.mcgill.ca)  
🔗 [GitHub Profile](https://github.com/Yashsethi24/)
```


Let me know if you want any modifications before adding it to GitHub! 🚀
