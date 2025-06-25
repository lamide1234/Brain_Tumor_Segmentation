**Brain Tumor Image Segmentation with nnU-Net**
This project implements an end-to-end pipeline for brain tumor image segmentation using the nnU-Net framework. It covers dataset preparation, preprocessing, model training, and evaluation, tailored for use with multi-modal MRI image data stored in .tif format.

📁 Directory Structure
```bash
├── Brain_Segmentation.ipynb       # Main notebook
├── images/                        # Original brain images (.tif)
├── masks/                         # Corresponding segmentation masks (.tif)
├── split_dataset/                 # Train-test split for nnU-Net
│   ├── images_training/
│   ├── labels_training/
│   ├── images_testing/
│   └── labels_testing/
├── nnUNet_raw/                   # nnU-Net raw data format
├── nnUNet_preprocessed/          # Preprocessed data
├── nnUNet_results/               # Model outputs
```

📂 Dataset
🔗 Google Drive- [.tif images](https://drive.google.com/drive/folders/1XBwvnhZrQQK5SXAWr2yTA4GOa9fgqQe7?usp=drive_link)
[nnUnet images format](https://drive.google.com/drive/folders/1Hs64C0FgBv5c638SLg20AKFmqWf4FwAy?usp=drive_link)

[Source](https://www.kaggle.com/code/abdallahwagih/brain-tumor-segmentation-unet-dice-coef-89-6/input) 

🔧 Features Implemented
-Image–mask integrity check (ensures correct pairing)

-Randomized dataset splitting into training and testing sets

-Conversion from .tif to .nii.gz format with RGB-channel separation

-Setup of nnU-Net-compliant folder structure

-Training a 3D Full Resolution nnU-Net model

-Model evaluation using nnU-Net prediction utility


 ***Results & Observations***
-Segmentation results are evaluated using Dice scores and qualitative overlays.

-Channel separation (RGB → modality) is necessary due to medical imaging structure.

-nnU-Net configuration automatically adapts to dataset properties.

***Note: I do not have access to a steady GPU, hence, the results are yet to be determined***
