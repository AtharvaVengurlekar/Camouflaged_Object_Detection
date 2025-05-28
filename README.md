# 🕵️‍♂️ Camouflaged Object Detection using YOLOv8

This project focuses on detecting camouflaged objects in images using the YOLOv8 object detection model. The goal is to accurately identify objects that blend into complex backgrounds.

## 📂 Project Structure

Camouflaged_Object_Detection_Project/
│
├── train/ # Training images
├── val/ # Validation images
├── test/ # Test images
├── runs/ # YOLO training results
│ └── detect/
│ └── train2/
│ ├── weights/ # Contains trained .pt files
│ ├── *.jpg, *.png # Visual results (metrics and samples)
├── dataset.yaml # Dataset configuration
├── requirements.txt # Python dependencies
├── test.ipynb # Main notebook for training & inference
├── yolov8n.pt # Pre-trained YOLOv8n weights
├── yolo11n.pt # Custom model weights (optional)
└── .gitignore

yaml
Copy
Edit

---

## Getting Started

### Step 1: Clone the Repository

```bash
git clone https://github.com/YourUsername/Camouflaged_Object_Detection_Project.git
cd Camouflaged_Object_Detection_Project
```

### Step 2: Set Python Environment
Ensure you are using Python 3.10.16 (recommended). You can use virtualenv or conda:

```bash
conda create -n camo_env python=3.10.16
conda activate camo_env
```

###Step 3: Install Requirements

```bash
pip install -r requirements.txt
```

###Download Dataset and Model
Option 1: From Kaggle
Download the dataset from Kaggle:
🔗 Kaggle Dataset Link
https://www.kaggle.com/datasets/rawsi18/military-assets-dataset-12-classes-yolo8-format

Option 2: From Google Drive
📁 Dataset: Drive Dataset Link : 

📦 Trained Model: Drive Model Link : 

After downloading, extract the dataset folders (train, val, and test) into the project directory. Also, place the trained model .pt file in a convenient location.

📒 Running the Notebook
Launch the notebook:

```bash
jupyter notebook test.ipynb
```

Then run the cells in order:
1)Install YOLOv8 via Ultralytics
2)Load the model
3)Train on your dataset
4)Inference on test images
5)Sample Results:
  a)Precision-Recall Curve
  b)F1 Curve
  c)Confusion Matrix
  d)Labeled Predictions
  e)Validation Batch Visualizations

All available under runs/detect/train/

###Model Used
##yolov8n.pt for initial training

##Custom-trained model (best.pt or last.pt) from runs/detect/train2/weights/
