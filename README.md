#   R e t i n o p a t h y  D e t e c t i o n ## Diabetic Retinopathy Detector for Kaggle's Diabetic Retinopathy Detection Copetition
https://www.kaggle.com/c/diabetic-retinopathy-detection

## Tutorial

There are jupyter notebooks in `tutorial` documenting the process I followed to get a basic working model.

## Workflow

1. Explore Data

2. Get basic model (VGG16?) running with sample data

3. Set up pipeline for quick iteration
  - detect and crop eyes in images using blobdetection (opencv)
  - resize images to 3, 512, 512 while keeping ascpection ratio
  - experiment with different methods of denoising

4. Swap out and ensemble models
