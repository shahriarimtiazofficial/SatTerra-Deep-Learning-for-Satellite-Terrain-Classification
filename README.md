Author: Md. Shahriar Imtiaz

Project Showcase: A deep learning-based project for classifying satellite imagery into environmental categories using convolutional neural networks (CNNs). This demonstrates end-to-end data preparation, model training, and evaluation with TensorFlow on a Kaggle dataset.

Overview
This project uses transfer learning and data augmentation to classify 5,631 RGB satellite images (224x224 pixels) from the Kaggle Satellite Image Classification Dataset. Ideal for climate studies and urban planning.
Classes Breakdown:

Cloudy: 1,500 images
Desert: 1,131 images
Green Area: 1,500 images
Water: 1,500 images

Split: 80% train (4,504), 10% val (563), 10% test (564).
Model: TensorFlow/Keras CNN with categorical loss; batch size 32; GPU-optimized.
Tech Stack

Python 3.12 | TensorFlow/Keras, NumPy, Matplotlib | Kaggle API, Google Colab (T4 GPU)

Project Structure

Satellite_Image_Classification.ipynb: Dataset download, EDA, and stratified splitting.
Satellite Image HeatMap.ipynb: Data loading, preprocessing, batch verification, and training setup.

How It Works

Acquire & Explore: Download ~21.5 MB dataset via Kaggle API; summarize structure.
Preprocess: Shuffle/split per class; load as TF datasets (shuffled, batched).
Train & Evaluate: CNN with cross-entropy; monitor val accuracy; visualize predictions/confusion matrices.

Example batch:

Images: (32, 224, 224, 3) | Labels: (32, 4)
Results & Insights

~90%+ val accuracy; stratified splits handle imbalance.

Extensions: Grad-CAM heatmaps, TensorFlow Lite deployment.
