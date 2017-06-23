CBIR
====

##Content Based Image Retrieval System

Due to the enormous increase in image database sizes, as well as its vast deployment in various applications, many Content Based Image Retrieval (CBIR) systems have been developed. The challenge, however, is in designing a system with the ability to retrieve best matches in case of having all kind of images as query. The power of such system highly depends on the features it employs to perform the matching process. 
In this project a CBIR system has been designed and developed. The [report](https://github.com/aminert/CBIR/blob/master/Report/FeazhAmineCBIR.pdf) outlines a description of some primitive features of image, which have been utilized in the presented system. These features are extracted and used as the basis for a similarity check between images. The algorithms used to calculate the similarity between extracted features, are then explained.
Final result was a Matlabapplication, with an image database, that utilized different features as the basis of comparison and retrieval. A GUI of the tool is illustrated below.

[Continue reading](https://github.com/aminert/CBIR/blob/master/Report/FeazhAmineCBIR.pdf)


![GUI](https://raw.github.com/aminert/CBIR/master/gui.png)

##Prerequiste tools
### Color Maps Generation
To be able to correctly use color histogram features, whether in RGB, HSV, or HMMD color spaces, we need to prepare colormaps that will be used as a feature space (i.e. histogram bins).
For each of the afromentioned color spaces we intend to extract a global color map that will be used to extract color histograms for all the images in the dataset. The following example reads an image in matlab and extracts an approriate color map, and then use it to generate a histogram represantation.
      
      
      file= ['images/1.jpg']; %Path to the image file
      rgb_image = imread(file); % Read the image
      double_image = im2double(rgb_image); % Convert image to double precision
      [indexed_image color_map] = rgb2ind(double_image,64); 


##License
( The MIT License )

Copyright (c) 2013 Amine Ben khalifa and Faezeh Tafazzoli

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE

