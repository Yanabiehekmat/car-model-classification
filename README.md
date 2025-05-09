

# Car Model Classification Using EfficientNet and Stanford Cars Dataset

## Project Title

**Car Model Recognition for Smart Parking and Insurance Applications**

## Objective

The goal of this project is to accurately classify the make and model of cars from images. This system is designed for use in insurance systems and smart parking management, where identifying the exact car model can be crucial.

## Dataset

We used the **Stanford Cars dataset**, which contains 16,185 images of 196 classes (different car models). The dataset is split into 8,144 training and 8,041 testing images. All images are labeled with the make, model, and year.

## Model

The chosen architecture is **EfficientNet-B0**, which offers a good balance of performance and computational efficiency. The model was fine-tuned using PyTorch on the Stanford Cars dataset.

## Training Setup

* Epochs: 5
* Optimizer: Adam
* Learning Rate: 0.001
* Loss Function: CrossEntropyLoss
* Input Image Size: 224x224
* Batch Size: 32
* Preprocessing: Resize, Normalize (ImageNet mean and std)

## Evaluation

After training for 5 epochs, the model achieved the following results on the test set:

* **Best Validation Accuracy:** 92.85%
* Many car models achieved **over 90% accuracy**
* Some lower-performing classes still maintained above **70% precision and recall**
* Classification report includes precision, recall, and F1-score for each class

## Applications

* Insurance claim verification
* Smart parking systems
* Car dealership analytics
* Vehicle inventory classification

## Future Work

* Fine-tuning on local car datasets (e.g., Iranian car models such as Pride, Samand, Dena)
* Improving performance on low-accuracy classes
* Using advanced techniques like ensemble models or vision transformers

## Requirements

* Python 3.10
* PyTorch
* Torchvision
* scikit-learn
* Matplotlib

## How to Run

1. Clone the repository
2. Install dependencies
3. Run the training script
4. Evaluate results using the provided classification report

