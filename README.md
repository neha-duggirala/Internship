# Internship

## Day 1: May 6,2019
### Todays Learning:
:star: Image classification - List of objects in the image </br>
:star: Object detection - Localization and bounding boxes </br>
:star: Semantic segmentation - Coloring the similar objects with same colors</br>
:star: Instance segmentation - Each object can be distinguished</br>
````
Problem statement:Need to get the vectors(pixel coordinaites of a polygon where the first and last are the same) out of the black(negative) and white mask(positive). Contour in opencv might be helpful.
````
[contour in opencv](https://docs.opencv.org/3.1.0/d3/d05/tutorial_py_table_of_contents_contours.html)

</br></br>
## Day 2: May 7,2019
### Todays Learning:
Every solution for a problem should be started by taking a very simple example. So to find the contours of the white masks in large satellite image, I have taken an image of the rectangle to find the contours and have obtained the following results.
#### Original image: 
<p align="middle">
<img src="https://github.com/neha-duggirala/Internship/blob/master/images/original.png" width="200" height="200">
  </p>
<img src="https://github.com/neha-duggirala/Internship/blob/master/images/0.png" width="200" height="200" align="left">
<img src="https://github.com/neha-duggirala/Internship/blob/master/images/1.png" width="200" height="200" align="left">
<img src="https://github.com/neha-duggirala/Internship/blob/master/images/2.png" width="200" height="200" align="left">


</br></br>
## Day 3: May 8,2019
### Todays Learning:
Appling the find contours to the .tif format image to obtain the co-ordinates of the white masks
