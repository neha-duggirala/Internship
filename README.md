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
  <p>
<img src="https://github.com/neha-duggirala/Internship/blob/master/images/0.png" width="200" height="200" align="left">
<img src="https://github.com/neha-duggirala/Internship/blob/master/images/1.png" width="200" height="200" align="left">
<img src="https://github.com/neha-duggirala/Internship/blob/master/images/2.png" width="200" height="200" align="left">
</p>

<p align="left">
  <br><br><br><br><br><br><br><br><br>
<h2> Day 3: May 8,2019</h2>
<h3>Todays Learning:</h3>
Appling the find contours to the .tif format image to obtain the co-ordinates of the white masks
</p>


## Day 4: May 9,2019
### Todays Learning:
To even out the uneven surfaces i have learned about a new module in opencv called **GaussianBlur** and understood that is uses an algorithm called Douglas-Peucker algorithm. Used different sizes of kernals to know which really fits the data.


## Day 5: May 10,2019
### Todays Learning:
Digit Classification using Keras as higher level api of tensorflow.Testing the images on my own data. The accuracy of the model was 97% but when it came to own dataset which i have processed the images using the opencv tools(resizing the window, thresholding and normalizing)
