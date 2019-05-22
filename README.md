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

## Day 6: May 13, 2019
## Todays Learning:
The contours are scaled to fit into the layers of the maps on **QGIS**. They were correctly mapped on to the boundaries of the buildings and it was beautiful to see the output but there were a few reductant polygons formed inside the polygons.
These can be removed using a threshould area of polygon.

## Day 7: May 14, 2019
## Todays Learning:
Contour area is given by the function cv2.contourArea() and thus the unwanted contours is removed by deciding the best threshould. **Douglas-Peucker algorithm**-It approximates a contour shape to another shape with less number of vertices depending upon the precision we specify. Thus can reduce the number of vertices and optimize the vector function.

## Day 8: May 15, 2019
## Todays Implementation:
Implemented the above algorithm.

## Day 9: May 16, 2019
## Todays learning:
There is a library called **Shapely** used for geo spacial data. The function contains() returns True if there is a polygon inside a polygon and thus the redundant polygons can be removed. Due to the application of Douglas-Peucker algorithm there is usuful information lost because of the contour approximation and should be taken care of.

## Day 10: May 17,2019
## Problems faced and resolving the issues:
The **gdal** package started showing unknown errors just for the import statement in the program and nothing other than that. By the end got to realize that after installing the shapely package, it had downgraded a few dependencies for its need but that downgradation is not supported by the gdal and again after upgrading the gdal dependency everything worked fine.

## Day 11: May 20,2019
These are the beautiful outputs
<p align="middle">
<img src="https://github.com/neha-duggirala/Internship/blob/master/images/Screenshot%20from%202019-05-21%2020-42-04.png" width="200" height="200">
  </p>
  <p align="middle">
<img src="https://github.com/neha-duggirala/Internship/blob/master/images/Screenshot%20from%202019-05-21%2020-42-20.png" width="200" height="200">
  </p>
  <p align="middle">
<img src="https://github.com/neha-duggirala/Internship/blob/master/images/Screenshot%20from%202019-05-21%2020-42-28.png" width="200" height="200">
  </p>
