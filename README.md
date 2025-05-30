# Studdy-Buddy

**Studdy Buddy** is a real-time drowsiness and yawn detection tool that helps students stay alert while studying. It uses your webcam and computer vision techniques to detect when you're closing your eyes for too long or yawning and plays an alert sound to snap you back into focus!

---

## 🔍 Features

- 👁️ Detects prolonged eye closure using facial landmarks.
- 😮 Detects yawning based on mouth openness.
- 💻 Runs in real-time using your webcam.

---

## Dataset 

This project utilizes the [Yawn Eye Dataset New](https://www.kaggle.com/datasets/serenaraju/yawn-eye-dataset-new) from Kaggle.
The dataset comprises:
- **Images** labeled for:
  - **Eye state**: Open or Closed
  - **Mouth state**: Yawning or Not Yawning

## How It Works

This project uses a Convolutional Neural Network (CNN), based on MobileNetV2, trained on the Yawn Eye Dataset New from Kaggle.

- The dataset contains labeled facial images indicating two classes:

    Eye status: Open or Closed

    Mouth status: Yawning or Not Yawning

- The model performs multi-label classification, predicting both the eye and mouth state from a single input image.

- During inference, the model processes an image and outputs two predictions:

  If eyes are closed and a yawn is detected, the system considers this a sign of drowsiness.

This approach allows early detection of fatigue symptoms from visual data and can be adapted to webcam input for real-time monitoring

---

## Requirements

Make sure you have **Python 3.7+** installed.

Install the dependencies:

```bash
pip install opencv-python mediapipe pygame
