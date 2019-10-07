# Glaucoma Detection and Classification using Deep Learning

Glaucoma is a condition of eye in which optic nerve is damaged due to abnormally high pressure in the eye. It is a chronic and irreversible disease. It is one of the leading cause of blindness across the globe in people over the age of 60. There is no cure for glaucoma, but early detection and medical treatment can prevent from disease progression. 

A goal of this project was to use deep learning architecture to build a model to detect and classify glaucoma by combining multiple deep features. Keras was used to build the model. We used publicly available database Drishti-GS1. 

### Methodology:

This project was divided into two parts:

1. Glaucoma Detection
    
    First, ROI (Region of interest) which is an area where optic disc and cup are located in the center and blood vessels of the Glaucoma fundus images were extracted using U shape convolutional neural network and then cup to disc ratio was calculated to classify if the image was glaucomatous or normal. [This Paper](https://arxiv.org/abs/1805.07549) was used for ROI extraction and disc segmentation.
    
2. Glaucoma Classification
     
     Cup to disc ratio was used for glaucoma classification. VGG16 CNN model was used to distinguish between glaucoma and non-glaucoma related images from fundus images. Glaucoma severity can also be classified from cup to disc ratio:
   * Mild ( CDR >0.3 and <0.5)
   * Moderate (CDR >=0.5 and <0.8)
   * Severe (CDR >=0.8)
