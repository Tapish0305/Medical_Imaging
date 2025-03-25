  # Project Title
 This project focuses on detecting medical conditions from chest X-ray images using YOLOv5. It involves image preprocessing, data augmentation, model training, and performance evaluation to improve detection accuracy in radiology.
  # Dataset Overview
 This project utilizes three datasets for training and evaluation:
 1. Vinbigdata-512-Image-Dataset-
    
     Contains train and test directories, each holding medical images.
 3. VinBigData-YOLO-Labels-Dataset-
    
     Contains train and test directories, each holding corresponding labels.
     Covers 14 medical conditions detected in chest X-rays.
 4. YOLOv5-Official-v31-Dataset-
    
     The official YOLOv5 dataset used for benchmarking and model improvements.
 # Data Preprocessing
 The preprocessing pipeline includes:
 
1. Resizing Images: Original dataset images (2080x3010) resized to 512x512.
   
2. Bounding Box Scaling: Adjusting bounding box coordinates to match resized images.
   
3. Data Augmentation (Albumentations):
   
   a. Horizontal Flip
   b. Rotation
   c. Brightness Contrast
   d. Gaussian Noise
   e. Gaussian Blur

6. Splitting Data: Using Group K-Fold Cross-Validation to avoid data leakage.
 
  # Model Training
  
  Framework: YOLOv5
  
  Batch Size: 16
  
  Epochs: 30
  
  Optimization: Learning rate scheduling
  
  Loss Tracking: Monitored using loss curves

  # Model Evaluation
  Performance is analyzed using:
  a. Confusion Matrix
  b. F1 Score
  c. Correlogram
  d. Loss Maps
