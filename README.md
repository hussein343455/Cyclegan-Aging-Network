# Cyclegan-Aging-Network
Implemented a CycleGan model to transform young to old human faces and vice versa. Upon completing training, the network could effectively convert images between the two categories.
 
I used this database https://data.vision.ee.ethz.ch/cvl/rrothe/imdb-wiki/:
  1-WIKI faces only 1 GB: database contains 62,328 images. 
  2-imdb faces only 7 GB :database contains 460,724 images.
Data cleaning,Removeing unwanted images:
used a Face Detection model with two conditions 1--image with a one face  2-the face and it occupy most of the image.

Data preprocessing and 
1-Normalization of pixel values between 0 and 1 to reduce computational demand.
2-Resizing all images to a standard size
