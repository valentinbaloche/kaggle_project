# KAGGLE_Project
We created this notebook, *with Google Colab*, in order to respond to the [Kaggle Project](https://www.kaggle.com/paultimothymooney/chest-xray-pneumonia).

The goal here was to **detect pneumonia in chest X-ray images using a deep learning approach**.

The dataset (*available online via the previous link or in the data folder of this repository*) is composed of **5856 chest X-ray images** from a retrospective cohorts of pediatric patients of 1 to 5 years old from Guangzhou Women and Children’s Medical Center. Theses images are divided in two folders : train and test. 

All the images were annotated with normal, bacterial pneumonia or viral pneumonia label by experts.

First we chose to train a CNN model to detect pneumonia among all the chest x-ray images (2 classes), then we tried to detect pneumonia and distinguish its cause : bacterial or viral (3 classes). Finally, we also used a transfer learning approach. 


> This notebook is divided in many parts :
> 1. Importing necessary packages : mainly keras from tensorflow for the machine learning process
> 2. Loading and preprocessing data : resizing, normalization, creation of a validation set
> 3. Building, training and evaluating a first CNN model to distinguish normal from pneumonia (2 classes)
> 4. Building, training and evaluating the same CNN model to distinguish between normal, bacterial pneumonia and viral pneumonia (3 classes)
> 5. Building, training and evaluating a pre-trained model (**Inception V3**) using a transfer learning approach to distinguish between normal, bacterial pneumonia and viral pneumonia (3 classes)
> 6. Building, training and evaluating a last CNN model pre-trained on a previous model to distinguish between normal, bacterial pneumonia and viral pneumonia (3 classes)


## Reference
- Kermany et al. Identifying Medical Diagnoses and Treatable Diseases by Image-Based Deep Learning / doi: [https://doi.org/10.1016/j.cell.2018.02.010](https://www.cell.com/cell/fulltext/S0092-8674(18)30154-5)


## Authors
- Camille AUCOUTURIER
- Valentin BALOCHE
