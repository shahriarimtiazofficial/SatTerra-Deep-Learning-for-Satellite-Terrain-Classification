𝐎𝐯𝐞𝐫𝐯𝐢𝐞𝐰
This project utilizes transfer learning and data augmentation to classify 5,631 RGB satellite images (224x224 pixels) from the Kaggle Satellite Image Classification Dataset. The dataset is ideal for climate studies, urban planning, and environmental monitoring.

𝑨𝒖𝒕𝒉𝒐𝒓: 𝑴𝒅.𝑺𝒉𝒂𝒉𝒓𝒊𝒂𝒓 𝑰𝒎𝒕𝒊𝒂𝒛

𝐂𝐥𝐚𝐬𝐬𝐞𝐬 𝐁𝐫𝐞𝐚𝐤𝐝𝐨𝐰𝐧:

Cloudy: 1,500 images

Desert: 1,131 images

Green Area: 1,500 images

Water: 1,500 images

𝐃𝐚𝐭𝐚 𝐒𝐩𝐥𝐢𝐭:

Training: 80% (4,504 images)

Validation: 10% (563 images)

Test: 10% (564 images)

𝐌𝐨𝐝𝐞𝐥:

Architecture: TensorFlow/Keras CNN

Loss Function: Categorical Cross-Entropy

Batch Size: 32

Optimization: GPU-optimized

Tech Stack

Python: 3.12

Libraries: TensorFlow/Keras, NumPy, Matplotlib

Tools: Kaggle API, Google Colab (T4 GPU)

How It Works
1. Acquire & Explore

The dataset (~21.5 MB) is downloaded using the Kaggle API.

The structure of the dataset is summarized to understand the data distribution.

2. Preprocess

The data is shuffled and split per class to ensure a balanced training set.

The dataset is loaded as TensorFlow datasets, shuffled and batched for efficient training.

3. Train & Evaluate

A CNN model is trained using categorical cross-entropy loss.

Validation accuracy is monitored, and predictions are visualized along with confusion matrices.

Example Batch

Images Shape: (32, 224, 224, 3)

Labels Shape: (32, 4)

Results & Insights

Validation Accuracy: ~90%+

Data Imbalance Handling: Stratified splits effectively manage class imbalance.

Future Extensions

Grad-CAM Heatmaps for visualizing class-specific regions of interest in the images.

TensorFlow Lite Deployment for mobile or edge device deployment.
