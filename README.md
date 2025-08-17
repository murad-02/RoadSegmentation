# RoadSegmentation

This repository contains code for a road scene segmentation project using deep learning (YOLOv8 or other segmentation models).  

**Note:** The dataset is **not included** due to size. Please download it separately.

---

## Dataset

We use the **Cityscapes Depth and Segmentation** dataset by [Sakshay Mahna on Kaggle](https://www.kaggle.com/datasets/sakshaymahna/cityscapes-depth-and-segmentation).

**Steps to download:**

1. Go to the Kaggle dataset: [https://www.kaggle.com/datasets/sakshaymahna/cityscapes-depth-and-segmentation](https://www.kaggle.com/datasets/sakshaymahna/cityscapes-depth-and-segmentation)  
2. Download the dataset.  
3. Extract it and place it in the following folder structure:

```
RoadSegmentation/
├── data/
│   ├── train/
│   │   ├── image/
│   │   │   └── *.npy
│   │   ├── label/
│   │   │   └── *.npy
│   ├── val/
│   │   ├── image/
│   │   │   └── *.npy
│   │   ├── label/
│   │   │   └── *.npy
```

---

## Installation

Install all required Python packages with:

```
pip install numpy matplotlib opencv-python ultralytics tqdm pillow
```

---

## Usage

- All code and experiments are in the Jupyter notebook:  
  `NotebookFile/Segmentation.ipynb`

- The notebook covers:
  - Data loading and EDA (exploratory data analysis)
  - Visualization of images and masks
  - Preprocessing and conversion to YOLOv8 format
  - Training and evaluation with YOLOv8 segmentation

---

## Visualizations

The notebook provides:
- Image and mask previews
- Class distribution bar and pie charts
- Pixel value histograms
- Overlay of masks on images
- Grid of random samples
- Class-wise mask area boxplots

---

## Training

To train the YOLOv8 segmentation model, follow the steps in the notebook.  
You can adjust training parameters as needed.

---

## Inference

After training, you can run inference on new images using the trained model.  
See the last section of the notebook for example code.

---

## License

This project is for research and educational purposes.