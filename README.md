# DCGAN_celeba# Deep Convolutional Generative Adversarial Network (DCGAN) - CelebA

## 📖 Project Overview
This project implements a **Deep Convolutional Generative Adversarial Network (DCGAN)** to generate realistic human faces using the **CelebA** dataset. The implementation follows the paper:  
[**"Unsupervised Representation Learning with Deep Convolutional Generative Adversarial Networks"**](https://arxiv.org/abs/1511.06434) by Radford et al.

## 📂 Dataset - CelebA
The **CelebA (Large-scale CelebFaces Attributes Dataset)** contains over 200,000 images of celebrity faces with various attributes. The dataset is used for training the DCGAN model.

### 🔹 **Dataset Preprocessing Steps**
1. **Download the Dataset**  
   - Get the **CelebA dataset** from Kaggle: [CelebA Dataset](https://www.kaggle.com/datasets/jessicali9530/celeba-dataset)  
   - OR from Google Drive:  
     ```
     https://drive.google.com/uc?id=0B7EVK8r0v71pZjFTYXZWM3FlRnM
     ```
   
2. **Upload to Google Colab or Extract Locally**  
   If using Google Colab, first upload the dataset to **Google Drive**.

3. **Extract the Dataset**  
   Run the following command to extract:
   ```python
   import zipfile

   zip_path = "/content/img_align_celeba.zip"
   extract_path = "/content/img_align_celeba"

   with zipfile.ZipFile(zip_path, 'r') as zip_ref:
       zip_ref.extractall(extract_path)

   print("Dataset Extracted!")


