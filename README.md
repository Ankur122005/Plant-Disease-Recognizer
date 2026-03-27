Plant Disease Recognition System 🌿🔍
This project is a comprehensive Deep Learning solution designed to identify diseases in various plant species through image analysis. It leverages a Convolutional Neural Network (CNN) trained on the "New Plant Diseases Dataset" and features a user-friendly web interface built with Streamlit.

🚀 Features
Disease Detection: Identifies 38 different classes of plant diseases and healthy states across crops like Tomato, Potato, Apple, Corn, and more.

Interactive Dashboard: A Streamlit-based web application for easy image uploading and real-time prediction.

High Accuracy: The model achieves approximately 95% accuracy on the test dataset.

End-to-End Pipeline: Includes notebooks for data preprocessing, training, and model evaluation.

🛠️ Project Structure
main.py: The Streamlit application script containing the frontend and prediction logic.

Train_plant_disease.ipynb: Jupyter notebook used for building and training the CNN model.

Test_plant_disease.ipynb: Notebook for testing the model and generating classification reports.

trained_model.keras: The pre-trained Keras model file.

training_hist.json: Log of the training and validation accuracy/loss over epochs.

home_page.jpeg: Visual asset for the web application's landing page.

📦 Installation & Setup
Clone the Repository:

Bash
git clone https://github.com/your-username/plant-disease-recognition.git
cd plant-disease-recognition
Install Dependencies:
Make sure you have Python installed, then run:

Bash
pip install streamlit tensorflow numpy matplotlib pandas seaborn
Run the Application:

Bash
streamlit run main.py
🧬 Model Details
The system uses a Sequential CNN architecture with the following components:

Input Layer: Resizes images to 128x128 pixels.

Convolutional Layers: Multiple layers with ReLU activation for feature extraction.

Pooling Layers: Max-pooling to reduce spatial dimensions.

Dense Layers: Fully connected layers leading to a Softmax output representing the 38 classes.

Performance Summary
Based on training_hist.json, the model shows strong convergence:

Training Accuracy: ~96.7%

Validation Accuracy: ~95% (as seen in Train_plant_disease.ipynb classification report).

📖 How to Use
Launch the app via Streamlit.

Navigate to the Disease Recognition page via the sidebar.

Upload a clear image of a plant leaf.

Click Predict to view the identified disease/status.

📊 Dataset
The model was trained using the New Plant Diseases Dataset available on Kaggle, which consists of about 87,000 images of healthy and diseased crop leaves.
