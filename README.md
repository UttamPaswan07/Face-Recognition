# Face-Recognition-for-attendance-tracking
This Python-based Face Recognition and Detection System uses OpenCV and machine learning.<br> It includes data collection, preprocessing, model training, and real-time face recognition.<br> Key components: collect_data.py, consolidated_data.py, recognize.py, haarcascade_frontalface_default.xml, and final_model.h5. Ideal for security and smart applications.

Face Recognition for Detection System
This project implements a robust Face Recognition and Detection System, leveraging Python, OpenCV, and machine learning techniques. It is designed to efficiently detect and recognize faces in images or real-time video streams. The system features modules for data collection, cleaning, and recognition, as well as pre-trained models for accurate facial analysis.
________________________________________
Project Overview
The system comprises multiple scripts and supporting files for end-to-end functionality, from data preparation to model deployment. The workflow involves:
1.	Data Collection: Capturing raw facial images for training.
2.	Data Preprocessing: Cleaning and organizing raw data to ensure high-quality inputs for model training.
3.	Model Training: Using processed data to train a neural network model.
4.	Face Recognition: Deploying the trained model to recognize faces in real-time or in static images.
________________________________________
Key Components
Scripts
1.	collect_data.py:
Captures facial images using a camera or dataset. The collected images are stored in the images folder and organized into labeled subdirectories for each individual or class.
2.	consolidated_data.py:
Preprocesses raw images by performing tasks such as:<br>
o	Cropping facial regions using Haar cascades.<br>
o	Resizing images for consistency.<br>
o	Normalizing pixel values.<br>
o	Saving the cleaned data in the clean data folder, structured for training, validation, and testing.<br>
3.	recognize.py:
Loads the trained model and performs face recognition using input from a webcam or static images.<br> It integrates:
o	Haar cascades (haarcascade_frontalface_default.xml) for face detection.<br>
o	Pre-trained .h5 models for recognition.<br>
________________________________________
Model Files
1.	final_model.h5 and final_model123.h5:
Pre-trained machine learning models saved in the HDF5 format. These models store:<br>
o	Architecture: The structure of the neural network.<br>
o	Weights: Learned parameters for facial recognition.<br>
o	Optimizer State: For further training or fine-tuning.<br>
These files eliminate the need for retraining and allow immediate deployment.
________________________________________
Supporting File<br>
•	haarcascade_frontalface_default.xml:<br>
A pre-trained Haar Cascade Classifier used for detecting frontal faces in images or video streams.
________________________________________
Folders
1.	Images Folder:<br>
o	Stores raw facial images collected during the data gathering phase.<br>
o	Organized into labeled subdirectories representing different individuals or classes.<br>
2.	Clean Data Folder:<br>
o	Contains preprocessed images ready for training.<br>
o	Data is cleaned, normalized, and divided into training, validation, and testing sets.<br>
o	Includes augmented images to enhance model robustness.<br>
________________________________________
How to Use
1.	Data Collection:
Use collect_data.py to capture facial images. Images will be stored in the images folder.
2.	Data Cleaning and Preprocessing:
Run consolidated_data.py to clean the raw images, normalize them, and save them in the clean data folder.
3.	Model Training:
Train a facial recognition model using the cleaned data. Pre-trained models (final_model.h5 and final_model123.h5) are included for immediate use.
4.	Face Recognition:
Execute recognize.py to load the trained model and perform real-time face recognition or analyze static images.
________________________________________
Applications
•	Attendance management systems.
•	Security and surveillance.
•	Personalized user experiences in smart devices.
________________________________________
Dependencies
•	Python 3.6+
•	OpenCV
•	TensorFlow/Keras
•	NumPy
