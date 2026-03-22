# 🌿 Plant Disease Detection using Custom CNN

## 📌 Overview

This project uses a **Custom Convolutional Neural Network (CNN)** to detect and classify plant diseases from leaf images.

A simple web interface is built using **Streamlit**, allowing users to upload a leaf image and receive the predicted disease.

---

## 🎯 Objective

To develop a deep learning-based system for accurate plant disease detection.

---

## 🧠 Model Details

* Model: Custom CNN (trained from scratch)
* Framework: TensorFlow / Keras
* Input: Leaf image
* Output: Disease prediction

---

## ⚙️ Project Pipeline

1. Data Collection
2. Data Preprocessing
3. Model Training
4. Model Saving
5. Prediction using Streamlit

---

## 🔄 Model Workflow

The following steps describe how the system works internally:

1. **User Input**

   * User uploads a plant leaf image through the Streamlit interface

2. **Image Preprocessing**

   * Image is resized to match model input size
   * Converted into array format
   * Normalized for better prediction accuracy

3. **Model Loading**

   * The trained CNN model is loaded from the `.keras` file

4. **Prediction**

   * Preprocessed image is passed to the model
   * Model predicts the disease class

5. **Output Display**

   * Predicted result is displayed on the screen

---

## 📂 Project Structure

```bash id="u7ntxk"
plant-disease-detection/
│
├── main.py
├── trained_plant_disease_model.keras
├── Train_plant_disease.ipynb
├── Test_plant_disease.ipynb
├── requirements.txt
└── README.md
```

---

## 🛠️ Requirements

Install all required libraries using:

```bash id="l3f8nl"
pip install -r requirements.txt
```

---

## ▶️ Run the Project

```bash id="2tb1ep"
streamlit run main.py
```

---

⚠️ Model Loading Configuration

The trained model is loaded inside main.py using the following line:

model = load_model("trained_plant_disease_model.keras")
Why this is important:

The application depends on this model file to make predictions.
If the file path is incorrect, the application will not be able to load the model and will result in an error.

When you need to update this:
If you move the model file into another folder (e.g., model/)
If you rename the model file
Example:

If the model is moved into a folder named model, update the code as:

model = load_model("model/trained_plant_disease_model.keras")

---

## 📸 Usage

* Run the application
* Upload a plant leaf image
* Click on predict
* View the detected disease

---

## 👨‍💻 Author

Developed by Neknar Naveen Kumar
