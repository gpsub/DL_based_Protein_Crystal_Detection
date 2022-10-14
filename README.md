# Deep Learning based Protein Crystal Detection

Deep learning model trained on the MARCO Protein Crystallization dataset. 

🖥️Work in Progress 

## Current Progress: 
- Created a new dataset of ~200 images labeled for segmentation by hand and trained a model which will extract only the "droplet" region from protein crystallization images. This will reduce computational load by eliminating useless pixels.  

- Using this new model I will inference and get the segmented mask for around 200,000 images, which can then by used for protein crystal recognition model training.

- Created a data preprocessing pipeline on Google Colab, where tfrecord files from [dataset](https://marco.ccr.buffalo.edu/download) are converted to jpg, zipped and stored in google drive(ImageExtraction.ipynb), the images are then unzipped in another colab file, inferenced using the custom trained model and the segmented output is stored in a new dataset folder back to google drive(DropSegmentation.ipynb). 

- Ongoing: Training various models on the new dataset after preprocessing it.

