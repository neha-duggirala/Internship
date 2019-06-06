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
Every solution for a problem should be started by taking a very simple example. So to find the contours of the white masks in large satellite image, I have taken an image of the rectangle to find the contours and have obtained correct co-ordinates.

</br>
<h2> Day 3: May 8,2019</h2>
<h3>Todays Learning:</h3>
Appling the find contours to the .tif format image to obtain the co-ordinates of the white masks
</p>
<p align="middle">
<img src="https://github.com/neha-duggirala/Internship/blob/master/images/Contours.png" width="700" height="200">
  </p>
 <p>

## Day 4: May 9, 2019
### Todays Learning:
To even out the uneven surfaces I have learned about a new module in opencv called **GaussianBlur** and understood that it uses an algorithm called Douglas-Peucker algorithm. Used different sizes of kernels to know which really fits the data.


## Day 5: May 10,2019
### Todays Learning:
Digit Classification using Keras as higher level API of tensorflow.Testing the images on my own data. The accuracy of the model was 97% but when it came to own dataset which I have processed the images using the opencv tools(resizing the window, thresholding and normalizing)

## Day 6: May 13, 2019
## Todays Learning:
The contours are scaled to fit into the layers of the maps on **QGIS**. They were correctly mapped on to the boundaries of the buildings and it was beautiful to see the output but there were a few reductant polygons formed inside the polygons.
These can be removed using a threshold area of a polygon.

## Day 7: May 14, 2019
## Todays Learning:
Contour area is given by the function cv2.contourArea() and thus the unwanted contours are removed by deciding the best threshold. **Douglas-Peucker algorithm**-It approximates a contour shape to another shape with less number of vertices depending upon the precision we specify. Thus can reduce the number of vertices and optimize the vector function.

## Day 8: May 15, 2019
## Todays Implementation:
Implemented the above algorithm.

## Day 9: May 16, 2019
## Today's learning:
There is a library called **Shapely** used for geospatial data. The function contains() returns True if there is a polygon inside a polygon and thus the redundant polygons can be removed. Due to the application of the Douglas-Peucker algorithm, there is useful information lost because of the contour approximation and should be taken care of.

## Day 10: May 17,2019
## Problems faced and resolving the issues:
The **gdal** package started showing unknown errors just for the import statement in the program and nothing other than that. By the end got to realize that after installing the shapely package, it had downgraded a few dependencies for its need but that downgradation is not supported by the gdal and again after upgrading the gdal dependency everything worked fine.

## Day 11: May 20,2019
These are the beautiful outputs
<p align="middle">
<img src="https://github.com/neha-duggirala/Internship/blob/master/images/Screenshot%20from%202019-05-21%2020-42-04.png">
  </p>
  <p align="middle">
<img src="https://github.com/neha-duggirala/Internship/blob/master/images/Screenshot%20from%202019-05-21%2020-42-20.png">
  </p>
  <p align="middle">
<img src="https://github.com/neha-duggirala/Internship/blob/master/images/Screenshot%20from%202019-05-21%2020-42-28.png">
  </p>

## Day 12: May 21,2019
## New Task:
The task given is all about **Multi-Class Segmentation.**
The landscape of a place in switzerland and there is a division into 3 classes 
1. Lake
2. Green Farm
3. City
<p align="middle">
<img src="https://github.com/neha-duggirala/Internship/blob/master/images/original.PNG" width=s00 height=250>
  </p>
  
## Day 13: May 22,2019
The contours of the entire ground truth Label.
<p align="middle">
<img src="https://github.com/neha-duggirala/Internship/blob/master/images/Mask_full.png" width=s00 height=250>
  </p>
  
 ## Day 14: May 23,2019
 The very important point I have learnt is to train the deep learing model preprocessing of data is essential. And thus there are different steps to do so. Initially, the image dimensions are reduced by converting hem into a grayscale image.
 <p align="middle">
  <img src="https://github.com/neha-duggirala/Internship/blob/master/images/masked_gray.jpg" width=500 height=250>
  </p>

## Day 15: May 24,2019
The dimensions of the image are very large and can't be given as an input for the neural network. Thus tiling needs to be done and all the patches are stored in the folder.

## Day 16: May 27,2019
Background extraction is done from the ground truth and other image masks are created in such a way that each mask has only one object belonging to a single class.

## Day 17: May 28,2019
I have learned that we are a product based organization and are developing a product wherein which the user drops in a satellite image and then he can easily get the count of solar panels, the area under water, the area under farm and several other aspects. 

## Day 18-21: May 29,2019 - June 3,2019
The steps involved in multi-class Segmentation is data preprocessing the size of a single image is **24331 X 24402** and this cannot be given as input to the neural network. The image is divided into different patches. The Mask created which has the segments of three different classes. Now patches should be derived even to the different classes.

<p align="middle">
  <img src="https://github.com/neha-duggirala/Internship/blob/master/images/Files_directory.PNG" width=500 height=250>
  </p>
  
 ## Day 22: June 4, 2019
 I have faced a peculiar error, **[MemoryError](https://datascience.stackexchange.com/questions/31330/memoryerror-for-np-array)** for np.array. MemoryError is exactly what it means, I have run out of memory in my 8GB RAM for my code to execute. Instead of using np float64 dtype I preferred using numpys dtype as uint8. This cleared my error. The very important part of writing code is its reusability by any person. Thus I had to sort the code into classes and functions that are required to be integrated into the pipeline.


## Day 23: June 5,2019
Integrating the code is not an easy task and found minor bugs which became difficult for me to find. Created a label Mask, a very important training data where each and every pixel is classified among the given three labels. Ig the pixel doesn't belong to any class then its value is given as zero.

## Day 24: June 6, 2019
It is the last day of my internship but the learning never stops. I received very good guidance from my mentors. I promise myself to dive deeper into deep learning and continue my journey

