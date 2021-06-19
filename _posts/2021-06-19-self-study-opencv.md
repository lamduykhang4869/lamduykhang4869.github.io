---
layout: post
title: OpenCV Note
subtitle: From OpenCV Tutorial
cover-img: /assets/img/path.jpg
thumbnail-img: /assets/img/opencv.png
share-img: /assets/img/path.jpg
tags: [computer vision, opencv]
---

## Command line arguments

\# Import argparse library.  
import argparse  

\# Construct the argument parser and parse the arguments.  
ap = argparse.ArgumentParser()  
ap.add_argument("-i", "--input", required=True,
    help="path to input image")  
ap.add_argument("-f", "--features-db", required=True, 
    help="Path to the features database")   
args = vars(ap.parse_args())  

\# Access the value of args.  
args["input"]  
args["features_db"] (dash `-` turn into underscore `_`)  


## OpenCV basic knowledges

In OpenCV, color images in RGB(Red, Green, Blue) color space have a 3-tuple associated with each pixel: (B, G, R).  

To retrieve the value of an individual pixel in the image:  

\# Access the RGB pixel located at x=50, y=100, keeping in mind that OpenCV stores images in BGR order rather than RGB.    

(B, G, R) = image[100, 50]  

\# Keep in mind that the height is the number of rows and the width is the number of columns.  
