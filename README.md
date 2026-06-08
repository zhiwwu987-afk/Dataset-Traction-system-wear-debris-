# Dataset-Traction-system-wear-debris-
A dataset of 1200 images for wire rope shedding detection.This repository provides the dataset, pre-trained models, and evaluation code for our research on wire rope shedding detection. It is designed to facilitate reproducibility and further research in industrial defect analysis.

## 📂 Repository Structure

Below is an overview of the core files included in this repository:

| File / Directory | Description |
| :--- | :--- |
| `environment.yml` | Conda environment configuration file for exact dependency reproduction. |
| `labeled_dataset.csv` | The core dataset containing extracted features (Area Ratio, IOD, Max Cluster, Core Ratio) and corresponding wear levels. |
| `rf_model.pkl` & `scaler.pkl`| The pre-trained Random Forest classifier and the standard scaler used for feature normalization. |
| `test.ipynb` | A Jupyter Notebook demonstrating how to load the model, process images, and visualize the detection results. |
| `never_see (*).jpg` | Sample unseen images provided directly in the root directory for quick testing and inference demonstration. |

## 🚀 Quick Start

Follow these steps to set up the environment and test the pre-trained model on the provided sample images.

### 1. Clone the Repository 
```bash
git clone (https://github.com/zhiwwu987-afk/Dataset-Traction-system-wear-debris)
```
### 2. Environment Setup （设置环境）
```bash
We provide an environment.yml file to easily recreate the exact Conda environment used for this project.

conda env create -f environment.yml
conda activate your_env_name
```
### 3. Run the Evaluation （测试，要建立一个文件夹存放没有见过的照片，将存放".csv"，".pkl"和"没见过的文件夹"路径设好）
```bash
Start Jupyter Notebook to run the evaluation script:

jupyter notebook test.ipynb

Execute the cells sequentially. The notebook will automatically load the never_see images, extract features using our illumination compensation algorithm, and output the predicted wear levels along with visualized bounding boxes.
```
## 📊 Dataset Overview 
```bash
- **Images**: 1200 raw images (`raw_images/`) and corresponding masks (`masks/`).
- **Models**: Pre-trained Random Forest model (`rf_model.pkl`) and scaler (`scaler.pkl`).
```
<img width="896" height="411" alt="image" src="https://github.com/user-attachments/assets/74374ab4-0c02-46a7-b680-836dada5d011" />

## 🚀 Download  （下载数据集）
```bash
Due to file size limits, the images and masks are hosted in the Releases section.
(通过网盘分享的文件：Dataset - Traction system (wear debris) 链接: https://pan.baidu.com/s/13A25bHm0P32XjAgOxSiLaQ?pwd=1436 提取码: 1436 --来自百度网盘超级会员v4的分享)**
```
## 💻 Usage
```bash
1. Download and extract the zip file into this repository folder.
2. Ensure your environment matches the required scikit-learn version for the `.pkl` files.
3. Read `labeled_dataset.csv` for bounding box/class information.
```
## 📝 Citation
```bash
We will post updated results soon
```
