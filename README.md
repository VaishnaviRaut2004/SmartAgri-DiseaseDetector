# SmartAgri-DiseaseDetector
An AI-driven system designed to identify plant diseases, aimed at fostering sustainable agricultural practices.
__________________________________________________________________________________________________________________________
Overview 
This project aims to harness deep learning to tackle a significant issue in agriculture: identifying plant diseases through images. By employing Convolutional Neural Networks (CNNs) and transfer learning with ResNet50, a well-regarded pre-trained model, the system detects diseases based on the visual symptoms present in plant images. The goal is to equip farmers and researchers with a quick and precise method for diagnosing plant health problems.
__________________________________________________________________________________________________________________________
Key Features and Benefits

Dataset Preparation:
The dataset consists of categorized plant images, each marked with a specific disease.
Preprocessing steps, including resizing and normalizing images, ensure that the model can effectively handle the data and achieve the best possible results.

Model Design and Training:
The foundation of the model is built on a CNN-based architecture, with ResNet50 enhancing performance through transfer learning.
Additional layers for Global Average Pooling and classification are added to tailor the model for plant disease detection.
Training employs techniques such as the Adam optimizer and categorical crossentropy loss function, promoting strong learning across multiple epochs.

Performance Metrics:
The model's learning journey is illustrated through training and validation accuracy/loss curves.
These insights are crucial for assessing how well the model generalizes to new data, ensuring reliable performance in practical applications.
__________________________________________________________________________________________________________________________
Practical Usage and Impact

Disease Prediction:
The model has been trained to predict diseases from new plant images. Users can receive immediate feedback on the disease identified in the input image by using the predict_disease(image_path) function, which also provides a visualization of the image.

Saving and Reusing the Model:
The trained model is stored as an .h5 file, making it easy to reuse and integrate into other systems. Although a pickle-based saving option is available, the Keras .h5 method is preferred for better compatibility.

Why It Matters:
Detecting plant diseases early can help save crops, minimize losses, and enhance agricultural productivity. This project showcases how AI can transform agriculture by providing an accessible and scalable tool for disease detection.
__________________________________________________________________________________________________________________________
Project Setup and Organization

Installation: To install dependencies, 
pip install -r requirements.txt

Training: Execute the training script to prepare the model:
python train_model.py

Prediction: To predict diseases, use:
predict_disease("path/to/plant_image.jpg")
__________________________________________________________________________________________________________________________
Conclusion
This project illustrates the potential of AI in addressing real-world challenges. By effectively utilizing ResNet50 and CNNs, it streamlines the intricate process of plant disease detection. Whether you are a researcher, farmer, or enthusiast, this system provides insight into how technology can positively impact agricultural practices.
