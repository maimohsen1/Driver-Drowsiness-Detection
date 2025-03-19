# 🚗🛑 **Driver Drowsiness Detection Using AI**  

## 📌 **Overview**  
This project aims to **detect driver drowsiness** using an AI model that combines **MobileNetV2** for feature extraction and **LSTM** for processing sequential image frames. The model analyzes a sequence of images from a video feed to determine whether a driver is awake or drowsy.  

---

## 📂 **Project Workflow**  
1️⃣ **Data Preparation** – Collect and preprocess images labeled as "Awake" and "Drowsy."  
2️⃣ **Model Development** – Build a deep learning model using MobileNetV2 and LSTM.  
3️⃣ **Training the Model** – Optimize the model using proper learning rate adjustments.  
4️⃣ **Image-Based Testing** – Test the model on individual images.  
5️⃣ **Real-Time Testing** – Use a webcam to detect drowsiness in real-time.  

---

## 📊 **1. Data Preparation**  
The dataset consists of two main folders:  
📁 **Train/** – Images used for training the model.  
📁 **Test/** – Images used for model validation.  

To ensure the model learns efficiently, image augmentation techniques are applied, and the images are resized to a smaller format to optimize performance.  

---

## 🤖 **2. Model Development**  
The model is designed as a hybrid of **MobileNetV2** and **LSTM:**  
- **MobileNetV2** extracts essential visual features from each image frame.  
- **LSTM (Long Short-Term Memory)** processes sequences of image frames to detect drowsiness patterns over time.  

To speed up training and improve efficiency, the MobileNetV2 model is **pretrained on ImageNet** and used as a feature extractor, while the LSTM layers analyze temporal dependencies.  

---

## 🎯 **3. Training the Model**  
- The model is trained using **binary classification** (Awake vs. Drowsy).  
- To prevent overfitting, techniques like **Early Stopping** and **Learning Rate Scheduling** are used.  
- Training is done in **mini-batches** to balance performance and speed.  
- The dataset is split into **training (80%)** and **validation (20%)**.  

---

## 🖼️ **4. Testing on Images**  
After training, the model is tested on individual images.  
- The image is resized and normalized.  
- The model analyzes the image sequence and predicts if the driver is awake or drowsy.  
- The result is displayed along with the image, showing the **classification label and confidence score**.  

---

## 🎥 **5. Real-Time Drowsiness Detection**  
To test the model in real-world scenarios:  
- A **webcam** continuously captures video frames.  
- The frames are processed into a sequence and passed to the model.  
- If drowsiness is detected, an **alert message** is displayed on the screen.  

  

---
