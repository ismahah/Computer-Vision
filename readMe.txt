This project implements human action recognition using a Vision Transformer (ViT) model, trained on a custom dataset of video frames to classify predefined actions.

Custom Dataset: Extracts frames from videos and applies preprocessing.
Vision Transformer: Employs patch embedding, positional encoding, and attention mechanisms for classification.
Training: Incorporates data augmentation, learning rate scheduling, checkpointing, and early stopping.
Validation & Testing: Tracks accuracy on validation and unseen test data.
Directory Structure
Dataset: Videos organized in folders by action labels.
Checkpoints: Stores trained model weights.

Workflow

Prepare Dataset: Organize videos by classes, extract frames, and preprocess.
Train Model: Train the ViT model with the specified dataset and configurations.
Validate & Test: Evaluate performance on validation and test data.
Hyperparameters
Batch Size: 64
Learning Rate: 0.0001
Epochs: 100
Optimizer: Adam with weight decay (0.0001)
Requirements
Python 3.x
PyTorch
torchvision
OpenCV
Matplotlib


How to Run
Organize Dataset: Place videos in class-specific folders. Ensure .avi format compatibility.
Update Dataset Path: Modify the dataset path in the script.
Train the Model.
Monitor Checkpoints: Use saved checkpoints for the best-performing models.