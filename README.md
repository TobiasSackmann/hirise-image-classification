# hirise-image-classification
Mars orbital image (HiRISE) - Image Classification

# Introduction

This is a project to implement a image classification for the [HiRISE Dataset](https://data.nasa.gov/Space-Science/Mars-orbital-image-HiRISE-labeled-data-set-version/egmv-36wq/about_data)

# Content

The notebooks directory contains three jupyter notebooks. The deep learning architecture is taken from keras/tensorflow articles as documented in the notenook comments.

* **hirise_partial_dataset.ipynb** is basically for debugging. It will load the full dataset into memory, but will only use a small part of it (due to memory limitations). One small model will be trained.
* **hirise_full_dataset.ipynb** is a more serious attempt to create image classification model. In respect to memory limitations a generator is used to load the images during training phase. The full datset will be used. Two models will be trained.
* **hirise_coral_Xception.ipynb (under development)** is by far the biggest model. A generator will load the full dataset. Due to the size of the model, the required time to train the model exceeds everything I am willing to do to my hardware. Therefore I will amend it to be trained on a Google Coral TPU.