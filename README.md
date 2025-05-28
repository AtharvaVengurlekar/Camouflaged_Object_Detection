# Camouflaged Object Detection using YOLOv8

This project focuses on detecting camouflaged objects in images using the YOLOv8 object detection model. The goal is to accurately identify objects that blend into complex backgrounds.

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

### Step 3: Install Requirements

```bash
pip install -r requirements.txt
```

## Download Dataset and Model
Option 1: From Kaggle
Download the dataset from Kaggle:
### Kaggle Dataset Link
https://www.kaggle.com/datasets/rawsi18/military-assets-dataset-12-classes-yolo8-format

### Download train model from drive:
https://drive.google.com/drive/folders/10Ix66f7V6jSYYLV6CvGWce_IioBrEjWD?usp=drive_link

After downloading, extract the dataset folders (train, val, and test) into the project directory. Also, place the trained model .pt file in a convenient location.

Running the Notebook
Launch the notebook:

```bash
jupyter notebook test.ipynb
```

Then run the cells in order:
- **Install YOLOv8 via Ultralytics**
- **Load the model**
- **Train on your dataset**
- **Inference on test images**
  
## Sample Results:
  - **Precision-Recall Curve**
  - **F1 Curve**
  - **Confusion Matrix**
  - **Labeled Predictions**
  - **Validation Batch Visualizations**

All available under results/weights

##  Model Used
- **yolov8s.pt for initial training**
- **Custom-trained model (best.pt or last.pt) from results/detect/weights/**
