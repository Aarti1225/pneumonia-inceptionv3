# pneumonia-inceptionv3
Transfer Learning with InceptionV3 for Pneumonia Detection
Pneumonia Detection using InceptionV3
Objective

Fine-tune a pretrained InceptionV3 model to classify chest X-ray images as Normal or Pneumonia.
Dataset

    Source: PneumoniaMNIST
    Format: .npz with train/val/test splits
    Input resized to 299x299, normalized

Model & Training

    Pretrained model: InceptionV3
    Final layer: 2-class output
    Loss: Weighted CrossEntropyLoss (to handle class imbalance)
    Optimizer: Adam
    Epochs: 5
    Batch size: 32
    Metrics: Accuracy, F1-Score

Evaluation Results
Metric 	Score
Accuracy 	83%
F1 Score (Normal) 	0.78
F1 Score (Pneumonia) 	0.86
Macro Avg F1 	0.82
Repo Contents

    MNIST_Aarti.ipynb: notebook for training & evaluation
    inception_pneumonia.pt: saved trained model
    requirements.txt: Python dependencies
    Pneumonia_MNIST.pptx: PPT slides for submission

How to Run

pip install -r requirements.txt
# Run all cells in the notebook
