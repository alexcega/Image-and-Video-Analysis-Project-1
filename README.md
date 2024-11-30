# Image-and-Video-Analysis-Project-1
Source code for the Project 1 of Image and Video Analysis class from UIB on detecting and counting humans in images taken at a beach using traditional computer vision techniques. The goal is to automate human detection in a beach environment, which could be useful for tasks such as occupancy monitoring and safety management.

# Overview
The project involves:

- Dataset Creation: Annotating a small dataset of beach images to create a ground truth for evaluation.
- Image Preprocessing: Applying techniques such as background subtraction, grayscale conversion, and binary mask generation to highlight human-like shapes.
- Human Detection: Using morphological operations and contour detection to refine masks and identify humans in various positions (standing, lying, swimming).
- Evaluation: Measuring the accuracy of the detection using metrics such as precision, recall, and F1-score.
Features
Detects humans in different positions on the beach: standing, lying on the sand, or swimming in the ocean.
Uses traditional image processing techniques without deep learning models.
Handles environmental challenges like illumination changes and background similarity.
Dataset
8 Images with humans present in various positions and environments (sand, ocean).
2 Control Images of the empty beach for background subtraction.
# Methodology
## Preprocessing:

Background subtraction using control images.
Conversion to grayscale for simplified processing.
Application of binary masks to highlight regions of interest.
## Human Detection Approaches:

- Approach 1: Binary mask generation, followed by morphological operations.
- Approach 2: Contrast enhancement using CLAHE and refined binary mask creation.
## Evaluation Metrics:

* Precision 
- Recall
- F1-Score.
- Mean Squared Error (MSE)
# Results
* The detection system achieved moderate accuracy, with a focus on detecting standing and lying individuals on the sand.
* Detection of swimmers was partially successful due to the limited visibility of their bodies on approach 1.
* False positives were observed near umbrellas and shaded areas.
## Challenges
* Illumination Variations: Images were taken from morning to evening, leading to inconsistent lighting.
* Background Similarity: Similar colors between sand, mountains, ocean, and sky caused false detections.
* Non-Human Objects: Umbrellas and other accessories were sometimes misclassified as humans.
#
Installation & Usage
Clone the Repository:

bash
Copiar código
`git clone https://github.com/alexcega/Image-and-Video-Analysis-Project-1.git
cd Image-and-Video-Analysis-Project-1`

Install Dependencies: Ensure you have Python and necessary libraries installed:


`pip install -r requirements.txt`

Run the Detection: Execute the main script to process images and count humans:

To see approach one see take 2 file:
`take2.ipynb`

To see approach 2 see:
`Crowd_cound.ipynb`

Evaluate Results: The output will include detected humans, precision, recall, and F1-score for each image.
