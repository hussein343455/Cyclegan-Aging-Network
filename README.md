# Cyclegan-Aging-Network
Implemented a CycleGan model to transform young to old human faces and vice versa. Upon completing training, the network could effectively convert images between the two categories.

database:
I used this database https://data.vision.ee.ethz.ch/cvl/rrothe/imdb-wiki/:
  1-WIKI faces only 1 GB: database contains 62,328 images. 
  2-imdb faces only 7 GB :database contains 460,724 images.
the image's name includes both the date of birth and the year the image was taken, By subtracting the date of birth from the year the image was taken, I can calculate the age of the person in the image

Data cleaning and removal of unwanted images:
All images were input into a Face Detection model. However, images that did not meet the following conditions were removed:1-There is only one face in the image. 2-The face occupies most of the image.
-grayscale images ware removed.
-corrupted images with shape of 1x1
Some Deleted images:

![xa](https://user-images.githubusercontent.com/57813196/212475127-a4a25cb3-06e4-4080-977a-34ecbf8efe9c.PNG)

Data preprocessing and 
1-Normalization of pixel values between -1 and 1 to reduce computational demand.
2-Resizing all images to a standard size

Classes:
1. young images: people under 23.
2. Older images: for people over 65

![young](https://user-images.githubusercontent.com/57813196/212475255-cd489767-daab-4b18-9a2b-0321a9a50094.png)
![old](https://user-images.githubusercontent.com/57813196/212475257-a7ca7283-4ba1-494c-a550-f8f5a1b16319.png)
