#   R e t i n o p a t h y  D e t e c t i o n ## Diabetic Retinopathy Detector for Kaggle's Diabetic Retinopathy Detection Copetition
https://www.kaggle.com/c/diabetic-retinopathy-detection

## Tutorial

There are jupyter notebooks in `tutorial` documenting the process I followed to get a basic working model.

## Workflow

1. Explore Data

2. Get basic model (VGG16?) running with sample data

3. Set up pipeline for quick iteration
  - detect and crop eyes in images using binary+otsu thesholding and conture finding (opencv) (done)
  - resize images to 3, 512, 512 while keeping ascpection ratio (working)
  - experiment with different methods of denoising (working):
    - relevant paper: http://www.ncbi.nlm.nih.gov/pmc/articles/PMC4335144/
  - set up generator pipeline from file
  - set up parallel processing for image preprocessing

4. Impliment ResNet-like model
- paper: http://arxiv.org/pdf/1512.03385v1.pdf , 5 

5. Swap out and ensemble models
  - weight cost function to deal with class imbalance as suggested by: http://gking.harvard.edu/files/0s.pdf
