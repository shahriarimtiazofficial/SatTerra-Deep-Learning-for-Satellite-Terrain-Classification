SatTerra employs convolutional neural networks to categorize satellite imagery into four distinct environmental classes: cloudy, desert, green area, and water.
Utilizing a Kaggle dataset comprising 5,631 RGB images, the project facilitates applications in climate monitoring and urban planning through transfer learning.
The workflow encompasses data acquisition via the Kaggle API, stratified partitioning (80% training, 20% validation/testing), and preprocessing to standardized 224x224 pixel batches.
The custom CNN architecture attains over 90% validation accuracy, mitigating class imbalance via randomized shuffling and augmentation protocols.
Developed in Python 3.12 with TensorFlow, NumPy, and Matplotlib, it leverages Google Colab's T4 GPU for efficient computation and reproducibility.
The provided Jupyter notebooks delineate the full pipeline, from exploratory data analysis to performance visualization via confusion matrices.
Suitable for academic and professional use, extensions include Grad-CAM interpretability or TensorFlow Lite deployment for operational satellite analytics.
