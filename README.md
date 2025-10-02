<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Satellite Image Classification</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      line-height: 1.6;
      background-color: #f4f7fc;
      margin: 0;
      padding: 0;
      color: #333;
    }
    header {
      background-color: #3c8dbc;
      color: white;
      padding: 15px 20px;
      text-align: center;
    }
    header h1 {
      margin: 0;
      font-size: 2.5em;
    }
    .content {
      max-width: 800px;
      margin: 30px auto;
      background-color: white;
      padding: 20px;
      box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
      border-radius: 8px;
    }
    h2 {
      color: #3c8dbc;
      font-size: 1.8em;
    }
    h3 {
      color: #3c8dbc;
      font-size: 1.4em;
    }
    ul {
      list-style-type: none;
      padding: 0;
    }
    ul li {
      padding-left: 20px;
      position: relative;
    }
    ul li:before {
      content: '•';
      position: absolute;
      left: 0;
      color: #3c8dbc;
      font-weight: bold;
    }
    .tech-stack, .results, .extensions {
      background-color: #e9f2f9;
      padding: 10px;
      margin-top: 20px;
      border-radius: 8px;
    }
    .footer {
      background-color: #3c8dbc;
      color: white;
      text-align: center;
      padding: 10px 0;
      position: relative;
      bottom: 0;
      width: 100%;
    }
    .footer p {
      margin: 0;
    }
  </style>
</head>
<body>

  <header>
    <h1>Satellite Image Classification with Deep Learning</h1>
    <p><strong>Author</strong>: Md. Shahriar Imtiaz</p>
  </header>

  <div class="content">
    <h2>Project Showcase</h2>
    <p>This project demonstrates the use of <strong>deep learning</strong> for classifying satellite imagery into environmental categories using <strong>Convolutional Neural Networks (CNNs)</strong>. The goal is to classify satellite images into 4 distinct environmental categories. The project covers <strong>data preparation</strong>, <strong>model training</strong>, and <strong>evaluation</strong> using <strong>TensorFlow</strong> on a <strong>Kaggle dataset</strong>.</p>

    <h2>Overview</h2>
    <p>This project utilizes <strong>transfer learning</strong> and <strong>data augmentation</strong> to classify 5,631 RGB satellite images (224x224 pixels) from the <strong>Kaggle Satellite Image Classification Dataset</strong>. The dataset is ideal for climate studies, urban planning, and environmental monitoring.</p>

    <h3>Classes Breakdown:</h3>
    <ul>
      <li><strong>Cloudy</strong>: 1,500 images</li>
      <li><strong>Desert</strong>: 1,131 images</li>
      <li><strong>Green Area</strong>: 1,500 images</li>
      <li><strong>Water</strong>: 1,500 images</li>
    </ul>

    <h3>Data Split:</h3>
    <ul>
      <li><strong>Training</strong>: 80% (4,504 images)</li>
      <li><strong>Validation</strong>: 10% (563 images)</li>
      <li><strong>Test</strong>: 10% (564 images)</li>
    </ul>

    <h3>Model:</h3>
    <ul>
      <li><strong>Architecture</strong>: TensorFlow/Keras CNN</li>
      <li><strong>Loss Function</strong>: Categorical Cross-Entropy</li>
      <li><strong>Batch Size</strong>: 32</li>
      <li><strong>Optimization</strong>: GPU-optimized</li>
    </ul>

    <div class="tech-stack">
      <h3>Tech Stack</h3>
      <ul>
        <li><strong>Python</strong>: 3.12</li>
        <li><strong>Libraries</strong>: TensorFlow/Keras, NumPy, Matplotlib</li>
        <li><strong>Tools</strong>: Kaggle API, Google Colab (T4 GPU)</li>
      </ul>
    </div>

    <h2>Project Structure</h2>
    <ul>
      <li><strong>`Satellite_Image_Classification.ipynb`</strong>: Dataset download, exploratory data analysis (EDA), and stratified splitting.</li>
      <li><strong>`Satellite_Image_HeatMap.ipynb`</strong>: Data loading, preprocessing, batch verification, and training setup.</li>
    </ul>

    <h2>How It Works</h2>
    <h3>1. Acquire & Explore</h3>
    <p>The dataset (~21.5 MB) is downloaded using the Kaggle API. The structure of the dataset is summarized to understand the data distribution.</p>

    <h3>2. Preprocess</h3>
    <p>The data is shuffled and split per class to ensure a balanced training set. The dataset is loaded as TensorFlow datasets, shuffled and batched for efficient training.</p>

    <h3>3. Train & Evaluate</h3>
    <p>A CNN model is trained using categorical cross-entropy loss. Validation accuracy is monitored, and predictions are visualized along with confusion matrices.</p>

    <h2>Example Batch</h2>
    <p><strong>Images Shape</strong>: (32, 224, 224, 3)</p>
    <p><strong>Labels Shape</strong>: (32, 4)</p>

    <div class="results">
      <h3>Results & Insights</h3>
      <ul>
        <li><strong>Validation Accuracy</strong>: ~90%+</li>
        <li><strong>Data Imbalance Handling</strong>: Stratified splits effectively manage class imbalance.</li>
      </ul>
    </div>

    <div class="extensions">
      <h3>Future Extensions</h3>
      <ul>
        <li><strong>Grad-CAM Heatmaps</strong> for visualizing class-specific regions of interest in the images.</li>
        <li><strong>TensorFlow Lite Deployment</strong> for mobile or edge device deployment.</li>
      </ul>
    </div>
  </div>

  <div class="footer">
    <p>&copy; 2025 Satellite Image Classification. All Rights Reserved.</p>
  </div>

</body>
</html>
