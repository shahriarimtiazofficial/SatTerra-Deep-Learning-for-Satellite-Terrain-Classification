𝐎𝐯𝐞𝐫𝐯𝐢𝐞𝐰:

This project utilizes transfer learning and data augmentation to classify 5,631 RGB satellite images (224x224 pixels) from the Kaggle Satellite Image Classification Dataset. The dataset is ideal for climate studies, urban planning, and environmental monitoring.

𝐃𝐞𝐬𝐜𝐫𝐢𝐩𝐭𝐢𝐨𝐧:

The dataset (~21.5 MB) contains 1,500 cloudy, 1,131 desert, 1,500 green area, and 1,500 water images, split into 80% training (4,504), 10% validation (563), and 10% test (564). A CNN built with TensorFlow/Keras (Python 3.12, Colab T4 GPU) was trained using categorical cross-entropy with batch size 32. Data was shuffled, stratified, and batched for balanced training. The model achieved ~95% validation accuracy, with performance evaluated via predictions and confusion matrices. This work includes Grad-CAM visualizations and saliency maps for mobile/edge applications.

𝑨𝒖𝒕𝒉𝒐𝒓: 𝑴𝒅.𝑺𝒉𝒂𝒉𝒓𝒊𝒂𝒓 𝑰𝒎𝒕𝒊𝒂𝒛
