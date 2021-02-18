# Drowsy-Driver-Detection

### Abstract

Automobiles are the largest means of transportation these days. And with the updating technologies there have been many new and upgraded features installed in vehicles. However, we are unable to control the accidents that cost a lot of lives. In most of the cases, it occurs due to the driver drowsiness and distraction conditions. This could happen due to late or long shifts at work, a long and monotonous drive for the holidays or distracted using your smartphone while driving. This, not only cost the lives of such drivers, but also a huge risk to fellow passengers and other vehicles on the road.

### Objective

To build an application that can scan the drivers face and alerts the driver and the fellow passengers if the driver feels sleepy. The goal of my project is a try to help save lives and reduce the accidents due to drowsy/sleepy drivers. 

### About the dataset

In order to acquire the data set, I have recorded videos of people mimicking on an external camera and divided into frames.
<ul>
 <li>It currently contains 3 different labelled pictures in the dataset. (eyes open, eyes closed, Look away)
 <li>The dataset is less than 1 GB and the images are 13-15 kb each
 <li>The dataset has 15171 images of a person with tree different postures: open eyes, closed eyes and looking away from the camera
<ul>

### Methodology
<ul>
    <li>Take video input through a webcam
    <li>Cut the videos to frames and label the data
    <li>Label the data and eliminate all images with incorrect data labels
    <li>Create a Region of Interest(ROI) and detect the face of the person
    <li>Identify the face and eyes of the driver using OpenCV
    <li>Try using Convolution Neural Network (CNN) to identify if the driver is feeling drowsy by detecting if the eyes are open or closed, or if the driver is looking away
    <li>When the score for number of frames the driver looks drowsy reaches the threshold, it sounds an alarm to alert the driver
<ul>
