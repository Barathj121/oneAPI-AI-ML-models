# OneAPI-AI-ML-Models

Hey so here I have did 5 different problems that I developed it in Intel OneAPI.

i)Lane detection using hough transform method with a lane image

  This repository contains code to perform lane detection on an image using the Hough Transform method. Lane detection is a crucial component of many autonomous vehicles and driver assistance systems. The Hough Transform allows us to detect lines within an image, which is especially useful for identifying lane markings on the road.
  
  Steps Involved:
  ->Loading and Displaying the Image:
  
  We start by loading an image using the mpimg.imread function and displaying it using Matplotlib's imshow. This gives us a visual representation of the road scene we want to process.
  
  ->Converting to Grayscale:
  
  To simplify further processing, we convert the colored road image to grayscale using OpenCV's cvtColor function. Grayscale images contain only intensity information, making it easier to detect edges.
  
  ->Edge Detection using Canny Algorithm:
  
  The Canny edge detection algorithm is applied to the grayscale image. This algorithm highlights edges by detecting rapid changes in intensity. We use cv2.Canny to get the edge-detected image.
  
  ->Region of Interest Selection:
  
  Not all parts of the image are relevant for lane detection. We define a region of interest (ROI) using a polygon that covers the area of the road where lane markings are expected. The region_of_interest function is used to extract the edge-detected image within this region.
  
  ->Hough Transform for Line Detection:
  
  The Hough Transform is a technique to detect lines in an image. We apply the cv2.HoughLinesP function to detect lines in the region of interest. Parameters such as rho, theta, and thresholds are used to control the detection sensitivity.
  
  ->Drawing Detected Lines:
  
  The lines detected by the Hough Transform are drawn on the original road image. The draw_lines function takes care of this step, overlaying the detected lane lines on the road scene.
  
  ->Displaying the Final Result:
  
  Finally, we display the road image with the detected lane lines using Matplotlib's imshow. This gives us a visual representation of how well the lane detection algorithm performs.
  
  ->Usage:
  To use this lane detection method on your own images, follow these steps:
  
  Replace 'lane3.jpg' with the path to your input image.
  Adjust parameters like thresholds, line lengths, and gap sizes as needed.
  Then you will be good to go


ii)malaria deetction using cnn with cell images

iii)Anomaly detection using alibi detect in clothe materials

iv)cats vs dog using cnn with images

v)Predicting whether a customer will stay or not in bank based on csv data using ANN

# How OneAPI helped me
Using a windows laptop with a mx graphic card training the malaria dataset with 30K images would have been a tiring process but with intel oneAPI it saved really a lot of time and its almost equal to the time run in mac whcih makes worrying about my laptop hardware incompatibility reduntant.
