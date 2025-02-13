# EU Moths Dataset

This folder contains the EU moths dataset prepared for the evaluation
of fine-grained recognition approaches. If you use this dataset, please 
cite the corresponding paper:

Dimitri Korsch and Paul Bodesheim and Joachim Denzler. 
Deep Learning Pipeline for Automated Visual Moth Monitoring: Insect Localization and Species Classification
Fine-grained Recognition Datasets for Biodiversity Analysis. 
INFORMATIK 2021, Computer Science for Biodiversity Workshop (CS4Biodiversity). Pages 443-460. 2021.
DOI: [10.18420/informatik2021-036](https://dx.doi.org/10.18420/informatik2021-036)

For more details visit the website of the dataset:
https://inf-cv.uni-jena.de/home/research/datasets/eu_moths_dataset/

## Directory Information

- ``images/``
    This directory contains subdirectories named after the corresponding moth species and each subdirectory contains the sample images of that species

- ``images.txt``
    The filenames of the images relative to the images directory
    Each line contains a separate image.

- ``labels.txt``
    The class IDs for each image in images.txt in the range 0 to 199. 
    Each line in labels.txt corresponds to the image in the same line in images.txt

- ``tr_ID.txt``
    Proposed train-test-splits for each image in images.txt. 
    Each line in tr_ID.txt corresponds to the image in the same line in images.txt. 
    Values are integers ranging from 0 to 3 to and might indicate different test folds.
    For example, a value of 0 means, this image is used for testing, and a value different from 0 (1 to 3) means this image is used for training.
    
- ``class_names.txt``
    List of class names for the 200 moth species.
    They correspond to the subdirectory names in ``images/``
    
- ``subset1_class_names.txt`` and ``subset1_class_names.txt``
    Proposed subsets of species as in the paper (Korsch et al., 2021)
    
- ``eu_moths_downloads.csv``
    List of download links for retrieving additional training images for indicated species.
    Each line corresponds to a species name and an URL for an image separated by a comma
