# Glaucoma Detection and Classification

Glaucoma is a condition of eye in which optic nerve is damaged due to abnormally high pressure in the eye. It is a chronic and irreversible disease. It is one of the leading diseases for blindness across the globe for people over the age of 60. There is no cure for glaucoma, but only we can detect it and prevent it by medical treatment. 

A goal of this project was to use deep learning architecture to build to detect and classify glaucoma by combining multiple deep features. We used publicly available database Drishti-GS1.

### Methodology:

This project was divided into two parts:

1. Glaucoma Detection
    
    First, we extracted ROI (Region of interest) which is an area where optic disc and cup are located in the center and blood vessels of the Glaucoma fundus images and then cup to disc ratio was calculated to classify that image is glaucomatous or normal.
    
2. Glaucoma Classification
     
     We used cup to disc ratio for glaucoma classification. We also classify glaucoma's severity from cup to disc ratio:
   * Mild ( CDR >0.3 and <0.5)
   * Moderate (CDR >=0.5 and <0.8)
   * Severe (CDR >=0.8)
