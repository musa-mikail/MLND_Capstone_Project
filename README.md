Machine learning engineer nanodegree Capstone_Project

Malaria Diagnosis with AI – Capstone Project
Author: Musa Mikail
Program: Machine Learning Engineer Nanodegree
Date: July 2019

Project Overview
This project aims to develop i-mal, a Windows PC application that uses machine learning to assist in the diagnosis of malaria from microscopic blood smear images. The goal is to improve diagnostic accuracy and accessibility, especially in rural areas of northern Nigeria.

Domain Background
Malaria remains a major health challenge in Nigeria, with millions of cases and thousands of deaths annually. Traditional diagnosis relies on manual inspection of blood cells, which is labor-intensive and prone to human error. AI offers a scalable solution to enhance diagnostic precision.

Problem Statement
Develop a user-friendly application that:

* Detects malaria-infected cells using a CNN-based binary classifier.
* Counts total red blood cells using edge detection.
Calculates parasitemia (%P) to aid diagnosis.
🧪 Dataset
Source: U.S. National Library of Medicine
27,558 labeled PNG images (balanced: 13,780 parasitized, 13,780 uninfected)
75% for training, 25% for validation/testing
🛠️ Solution Approach
Preprocessing: Image scaling, rotation, augmentation
Model: CNN (VGGNet architecture), benchmarked against a vanilla ANN
Training: Amazon SageMaker
Deployment: PyQt-based GUI with OpenCV for edge detection
Output: % of infected cells (parasitemia)
📊 Evaluation Metrics
Binary Classifier Accuracy (Ab)
Edge Detection Accuracy (Ac)
Overall System Accuracy (A = Ac × Ab)
🧱 Project Design
CNN model built with TensorFlow & Keras
GUI for image upload, visualization, and inference
Separate evaluation of classifier and cell counter performance
📈 Benchmark
Compare CNN performance against a basic ANN
Use accuracy as the primary metric due to balanced dataset

Objective:
Develop and deploy a malaria diagnostic system based on a convolution neural network model.

Tool and libraries:
- Language: python 3.7
- Image processing: OpenCV
- GUI: pyQt
- Machine learning modelling: tensorflow/pytorch
- Visualization: pyplot.matplotlib
- Integration/ version control: github
- base model: VGGNet-Simonyan et al: https://arxiv.org/pdf/1409.1556.pdf?source=post_page
OpenCV algorithm for edge detection: Canny Edge Detector: https://docs.opencv.org/2.4/doc/tutorials/imgproc/imgtrans/canny_detector/canny_detector.html

Dataset
Malaria Dataset: https://ceb.nlm.nih.gov/repositories/malaria-datasets/

 — ---------------------------

