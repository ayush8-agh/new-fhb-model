🌾 Wheat FHB Disease Detection App

This project is a Machine Learning-powered web app for detecting Fusarium Head Blight (FHB) in wheat images.
It uses a TensorFlow (Keras) deep learning model trained on wheat datasets to classify images into 3 categories:

✅ Healthy

🌱 FHB Mild

🌾 FHB Moderate

The app is built with Gradio, allowing users to upload a wheat image and instantly get predictions with confidence scores.

🚀 Features

Upload wheat crop images for disease detection.

Real-time predictions with confidence probabilities.

Simple, interactive web interface powered by Gradio.

Deployable to Render, Hugging Face Spaces, or any cloud service.

📂 Project Structure
wheat-fhb-app/
├── app.py                          # Gradio web app
├── final_wheat_multi_class_model.keras   # Trained deep learning model
├── requirements.txt                # Dependencies for deployment
└── README.md                       # Project documentation

⚙️ Installation & Running Locally

Clone the repo

git clone https://github.com/ayush8-agh/new-fhb-model.git
cd new-fhb-model


Create a virtual environment (recommended)

python -m venv venv
source venv/bin/activate   # (Linux/Mac)
venv\Scripts\activate      # (Windows)


Install dependencies

pip install -r requirements.txt


Run the app

python app.py


Open your browser at http://127.0.0.1:7860/ to use the app.

🌍 Deployment

You can deploy this app easily:

Render: Create a new Web Service, connect this repo, and Render will auto-install dependencies.

Hugging Face Spaces: Upload this repo to a Space (Gradio SDK) and it will run automatically.

🧠 Model Training (Summary)

Backbone: MobileNetV2 (ImageNet pre-trained)

Input Size: 224x224x3

Optimizer: Adam

Loss: Categorical Crossentropy

Metrics: Accuracy

Dataset: Wheat images split into train / valid / test directories

📜 License

This project is for educational and research purposes.
