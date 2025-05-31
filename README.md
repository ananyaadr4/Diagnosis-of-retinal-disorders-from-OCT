📌 Project Overview
Retinal diseases such as Choroidal Neovascularization (CNV), Diabetic Macular Edema (DME), and Drusen are leading causes of vision loss. Manual diagnosis through OCT scans can be time-consuming and subjective. This project aims to automate the classification of OCT images using Convolutional Neural Networks (CNNs) to support Computer-Aided Diagnosis (CAD).

🎯 Objectives
Build a CNN model to classify retinal images into four categories.

Improve diagnostic accuracy through advanced preprocessing and model optimization.

Deploy the model on a FastAPI-based web app hosted on AWS EC2 for real-time predictions.

🧠 Technologies & Tools
Languages: Python

Libraries: TensorFlow, Keras, Pandas, NumPy, OpenCV, Matplotlib, Seaborn

Modeling: Convolutional Neural Network (CNN)

Deployment: FastAPI, Uvicorn, AWS EC2

Others: Model Checkpointing, Data Augmentation

🗃️ Dataset
Source: Publicly available dataset containing OCT scan images of retina.

Classes:

CNV (Choroidal Neovascularization)

DME (Diabetic Macular Edema)

Drusen

Normal

Total Images: ~80,000

Format: .jpeg images labeled in separate directories per class

🧪 Model Development Pipeline
1. Data Ingestion
Load images from four folders corresponding to each disease class.

Resize images to 224x224 for uniform input size.

2. Data Preprocessing
Normalization

Data augmentation (rotation, flip, zoom, shift)

Train-test-validation split

3. Model Architecture
Built a CNN using Keras with:

Convolutional + MaxPooling layers

Dropout for regularization

Dense layers for classification

Softmax output layer for multi-class prediction

4. Training & Evaluation
Optimizer: Adam

Loss Function: Categorical Crossentropy

Metrics: Accuracy

Used ModelCheckpoint callback to save the best-performing model

Achieved ~88% accuracy on validation set

5. Deployment
Created a REST API using FastAPI

Deployed the application on AWS EC2

Allows users to upload an OCT image and receive a disease classification in real time
![image](https://github.com/user-attachments/assets/000709d1-2a43-4a29-8452-1857997096bb)
![image](https://github.com/user-attachments/assets/7fbbb7d1-924c-4f02-a28d-d225957ae813)

