# Dataset-Traction-system-wear-debris-
A dataset of 1200 images for wire rope shedding detection.This repository provides the dataset, pre-trained models, and evaluation code for our research on wire rope shedding detection. It is designed to facilitate reproducibility and further research in industrial defect analysis.

## 📂 Repository Structure

Below is an overview of the core files included in this repository:

| File / Format | Description |
| :--- | :--- |
| `labeled_dataset.csv` | The core dataset containing extracted features (Area Ratio, IOD, Max Cluster, Core Ratio) and corresponding wear levels. |
| `rf_model.pkl` & `scaler.pkl`| The pre-trained Random Forest classifier and the standard scaler used for feature normalization. |
| `test.ipynb` | A Jupyter Notebook demonstrating how to load the model, process images, and visualize the detection results. |
| `never_see (*).jpg` | Sample unseen images provided directly in the root directory for quick testing and inference demonstration. |



## 📊 Dataset Overview
- **Images**: 1200 raw images (`raw_images/`) and corresponding masks (`masks/`).
- **Labels**: Detailed annotations in `labeled_dataset.csv`.
- **Models**: Pre-trained Random Forest model (`rf_model.pkl`) and scaler (`scaler.pkl`).

## 🚀 Download
Due to file size limits, the images and masks are hosted in the Releases section.
(通过网盘分享的文件：Dataset - Traction system (wear debris) 链接: https://pan.baidu.com/s/13A25bHm0P32XjAgOxSiLaQ?pwd=1436 提取码: 1436 --来自百度网盘超级会员v4的分享)**

## 💻 Usage
1. Download and extract the zip file into this repository folder.
2. Ensure your environment matches the required scikit-learn version for the `.pkl` files.
3. Read `labeled_dataset.csv` for bounding box/class information.

## 📝 Citation
We will post updated results soon

