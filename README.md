# 🌱 SmartFarm AI: Intelligent Agriculture Assistant

![Python](https://img.shields.io/badge/Python-3.8%2B-blue)
![Streamlit](https://img.shields.io/badge/Framework-Streamlit-FF4B4B)
![PyTorch](https://img.shields.io/badge/Deep%20Learning-PyTorch-EE4C2C)
![ML](https://img.shields.io/badge/Machine%20Learning-Scikit--Learn-orange)

**SmartFarm AI** is a modern, responsive web application built entirely in Python using Streamlit. It uses Machine Learning and real-time weather data to help farmers maximize crop yield, treat diseases, and optimize fertilizer usage.

## 🚀 Live Demo
**https://smartfarm-app.streamlit.app**

---

## 🌟 Key Features

### 1. 🌾 Crop Recommendation AI
* **Input:** Soil nutrients (N, P, K, pH), rainfall, and the user's City.
* **Smart Integration:** Uses the **OpenWeatherMap API** to automatically fetch real-time temperature and humidity based on the selected city.
* **Model:** Random Forest Classifier.

### 2. 🧑‍🌾 Fertilizer Advice
* Analyzes the deficit between current soil nutrients and the ideal requirements for a specific crop.
* Provides actionable, dictionary-based recommendations to balance Nitrogen, Phosphorus, and Potassium levels safely.

### 3. 🍃 Plant Disease Detection
* **Input:** Upload an image of a plant leaf.
* **Model:** A custom **ResNet9 Convolutional Neural Network (CNN)** built with PyTorch, trained to identify 38 different disease classes.
* **Output:** Identifies the disease and provides immediate treatment advice and preventative measures.

---

## 🛠️ Tech Stack
* **Frontend/Backend:** Python, Streamlit
* **Machine Learning:** Scikit-Learn (Random Forest), PyTorch (ResNet9)
* **Data Handling:** NumPy, Pandas, Pillow
* **APIs:** OpenWeatherMap
* **Deployment:** Streamlit Community Cloud

---

## 💻 How to Run Locally

### 1. Clone the Repository
```bash
git clone https://github.com/sharathbandis/SmartFarm-Streamlit.git
cd SmartFarm-Streamlit

```

### 2. Set Up the Weather API Key

To use the real-time weather feature, you need an OpenWeatherMap API key.

1. Create a file named `config.py` in the root directory.
2. Add your key like this:
```python
weather_api_key = "YOUR_API_KEY_HERE"

```



### 3. Install Dependencies

```bash
pip install -r requirements.txt

```

### 4. Run the App

```bash
python -m streamlit run app.py

```

Open your browser and go to: `http://localhost:8501`

---

