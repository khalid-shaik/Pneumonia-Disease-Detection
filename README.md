# 🩺 Pneumonia Detection Using Chest X-Ray Images

📘 Overview

Pneumonia is a serious lung infection that affects one or both lungs, most commonly caused by the bacterium Streptococcus pneumoniae.
According to the World Health Organization (WHO), pneumonia is responsible for nearly one in three deaths in India, making early detection and treatment essential.

Traditionally, pneumonia diagnosis requires expert radiologists to analyze chest X-ray scans, which can be time-consuming and limited in remote areas.
This project aims to develop an automated pneumonia detection system using deep learning — specifically a Convolutional Neural Network (CNN) — to classify chest X-rays as normal or pneumonia.

🧩 Objective

To build and train a CNN model capable of detecting pneumonia from chest X-ray images, providing a reliable and fast diagnosis support system.

🗂️ Dataset

Dataset consists of 5,863 labeled chest X-ray images divided into:

Pneumonia: 4,273 images

Normal: 1,590 images

Each image is a grayscale X-ray of the chest region.

Source: Chest X-Ray Images (Pneumonia)

![person1_virus_13](https://github.com/user-attachments/assets/af32abbe-9950-4193-8573-5c0a46ba7c22)
![person37_virus_82](https://github.com/user-attachments/assets/480b0dc0-b65a-477b-8d76-1092e7916ed1)
![person78_bacteria_387](https://github.com/user-attachments/assets/20761618-bf70-44d1-b52e-7ce0c9f5f6b2)




⚙️ Technologies Used

Python

TensorFlow / Keras – for CNN model building

OpenCV, NumPy, Pandas – for data preprocessing

Matplotlib, Seaborn – for visualization

Google Colab / Jupyter Notebook – for implementation

🔬 Methodology

Data Preprocessing:

Resized all images to 150×150 pixels for consistent input.

Normalized pixel values to improve training performance.

Split data into 80% training and 20% testing sets.

Model Building:

Designed a Convolutional Neural Network with multiple convolution, pooling, and dense layers.

Used ReLU activation and Dropout layers to prevent overfitting.

Optimized using Adam optimizer and binary cross-entropy loss.

Model Evaluation:

Measured model performance using accuracy, precision, recall, F1-score, and confusion matrix.

Achieved an accuracy of 94.2% and F1-score of 92% on the test set.

Visualization:

Displayed sample predictions and model confidence scores.

Plotted training vs validation accuracy and loss curves to monitor learning progress.

📊 Results

The CNN correctly classified 942 out of 1,000 test images.

Achieved 94.2% overall accuracy with balanced recall and precision.

Identified 58 misclassified cases, mostly borderline infections.

🚀 Future Improvements

Integrate transfer learning using pre-trained models like VGG16 or ResNet50 for better accuracy.

Add Grad-CAM visualization to highlight infection areas on X-rays.

Deploy as a web-based diagnostic tool for hospitals and rural clinics.
