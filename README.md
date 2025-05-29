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
jupyter notebook main.ipynb
```

Then run the cells in order:
- **Install YOLOv8 via Ultralytics**
- **Load the model**
- **Train on your dataset**
- **Inference on test images**
  
## Sample Results:
  - **Precision-Recall Curve** : Shows the trade-off between precision (how many detected objects were correct) and recall (how many actual objects were detected). A good model will have a curve closer to the top right.
  - **F1 Curve** : Displays the F1 score (harmonic mean of precision and recall) across different confidence thresholds. It helps determine the threshold at which the model performs best overall.
  ![Image](https://github.com/user-attachments/assets/99bc5b5f-55bf-4230-8eb7-33fc534b82c1)
  
  - **Confusion Matrix** : A visual representation of predicted vs actual classes. It shows where the model made correct predictions and where it misclassified, helping identify specific problem areas.
  ![Image](https://github.com/user-attachments/assets/c83cbf42-1642-4097-ad2a-ec0c4830c042)


  - **Labeled Predictions** : Images showing the model's predictions (bounding boxes and class labels) on unseen test data. These help you visually assess the model's accuracy and performance.
  - **Validation Batch Visualizations** : Samples from the validation dataset with both ground truth and predicted labels shown. Useful to compare the model's output directly with the expected results.

All available under results/weights

##  Model Used
- **yolov8s.pt for initial training**
- **Custom-trained model (best.pt or last.pt) from results/detect/weights/**
