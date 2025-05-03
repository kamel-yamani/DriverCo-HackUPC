# 🚗 DriverCo - HackUPC 2025

**DriverCo** is an AI-powered, real-time drowsiness detection and voice assistant system designed to make driving safer. Built at **HackUPC 2025**, this project combines computer vision, generative AI, and voice technologies to detect early signs of fatigue and engage drivers through natural conversation.

---

## 🌟 Features

- 👁️ **Real-time Drowsiness Detection** using fine-tuned YOLOv8 on eye and mouth cues (e.g. eye closure, yawning)
- 🧠 **Conversational Assistant** powered by Google Gemini API
- 🎙️ **Speech-to-Text & Text-to-Speech** interface for hands-free interaction
- 📊 **Custom Trained Model** on publicly available fatigue datasets (50 epochs)
- 🎥 **Live Webcam Inference** for testing and real-time simulation

---

## 📂 Project Structure

```bash
DriverCo-HackUPC/
│
├── driverco-model-training.ipynb     # Notebook for training the YOLOv8 model
├── DriverCo_VF.ipynb                 # Final system integrating detection + Gemini AI
├── README.md                         # You're here
````

---

## 🚀 Getting Started

### 1. Clone the repository

```bash
git clone https://github.com/yourusername/DriverCo-HackUPC.git
cd DriverCo-HackUPC
```

### 2. Install Dependencies

We recommend running on Google Colab. The main packages include:

* `ultralytics`
* `opencv-python`
* `google-generativeai`
* `edge-tts`
* `Pillow`, `numpy`, `matplotlib`

### 3. Train the Model (Optional)

Open `driverco-model-training.ipynb` to:

* Visualize dataset
* Fine-tune YOLOv8
* Save your custom model

> Note: We trained our model on a custom dataset for 50 epochs to optimize accuracy for drowsiness signs.

### 4. Run the Assistant

Open `DriverCo_VF.ipynb` to:

* Run real-time webcam detection
* Trigger conversational assistant when drowsiness is detected

---

## 🧪 Dataset

We used a **publicly available dataset** focused on drowsy driving signs. It includes labeled facial landmarks for eye and mouth states. The model was trained in YOLO format for compatibility.

---

## 🧠 Built With

* [YOLOv8](https://github.com/ultralytics/ultralytics) — Object detection
* [Google Gemini API](https://ai.google.dev) — Conversational GenAI
* [OpenCV](https://opencv.org) — Real-time computer vision
* [Edge-TTS](https://github.com/rany2/edge-tts) — Speech synthesis
* [Google Colab](https://colab.research.google.com) — Development environment

---

## 🎓 Team

Made with 💡 at **HackUPC 2025** by:

* **Kamel Yamani**
* **Marwa Nair**

---

## 📄 License

This project is open-source and available under the [MIT License](LICENSE).

