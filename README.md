# IMAGE-CLASSIFICATION-SONG-PLAYER

## Overview

**IMAGE-CLASSIFICATION-SONG-PLAYER** is a Python-based project that combines **Image Classification** and **Music Playback Automation** using **Machine Learning**.  
The model classifies input images into predefined categories and automatically plays a specific **song** corresponding to the detected class.

This project showcases how computer vision and automation can work together in a fun and creative way — classifying images and responding with audio feedback.

---

## Objectives

* Build a simple **image classification model** using deep learning.
* Classify test images into **predefined categories** (e.g., Class 1: 🔺, Class 2: ⚪).
* **Automate song playback** based on the classification result.
* Demonstrate the integration of **TensorFlow/Keras** and **Python-VLC** for multimedia interaction.

---

## Key Features

* **Image Classification:**  
  Trains a CNN model on labeled image datasets (two classes).

* **Automated Song Playback:**  
  Plays different songs based on predicted class results.

* **Training & Testing Workflow:**  
  - Load and preprocess images.  
  - Train and save the model (`.h5`).  
  - Test new images and play mapped songs.

* **Extensible Architecture:**  
  Easily add new classes or modify the song mappings.

---

## Technologies Used

| Category             | Tools / Libraries     |
| -------------------- | --------------------- |
| Programming Language | Python                |
| Deep Learning        | TensorFlow / Keras    |
| Data Handling        | NumPy, Pandas         |
| Image Processing     | OpenCV, Pillow        |
| Audio Playback       | Python-VLC / Playsound|
| Environment          | Google Colab          |

---

## Dataset

The dataset consists of two folders representing **different image classes**:

* `Folder1/` — Class 1 images (e.g., triangles)
* `Folder2/` — Class 2 images (e.g., circles)

Each folder contains multiple training images for its class.

> You can replace or expand these with any custom dataset (e.g., animals, logos, or objects).

---

## Project Workflow

1. **Data Preparation**
   * Organize image data in separate folders per class.
   * Resize and normalize images for model compatibility.

2. **Model Training**
   * Use a **Convolutional Neural Network (CNN)** to train on the dataset.
   * Save the trained model as `classifier.h5`.

3. **Model Testing**
   * Load a new test image (`test1`, `test2`, etc.).
   * Predict its class using the trained model.

4. **Automated Song Playback**
   * Map each class to a predefined song.
   * Automatically play the corresponding song based on prediction.

---

## Example Mapping

| Class  | Folder     | Description | Song Played |
| ------- | ----------- | ------------ | ------------ |
| Class 1 | Folder1     | Triangle  | Song of **Talha Anjum** |
| Class 2 | Folder2     | Circle    | Song of **AP Dhillon** |

---

## Sample Results

| Test Image | Predicted Class | Song Played         |
| ----------- | ---------------- | ------------------- |
| `test1.jpg` | Class 1          | Talha Anjum Song    |
| `test2.jpg` | Class 2          | AP Dhillon Song     |

---

## Directory Structure
IMAGE-CLASSIFICATION-SONG-PLAYER/
├── data/
│ ├── Folder1/ # Training images for Class 1
│ └── Folder2/ # Training images for Class 2
│
├── models/
│ └── classifier.h5 # Trained CNN model
│
├── songs/
│ ├── class1_song.mp3 # Song for Class 1
│ └── class2_song.mp3 # Song for Class 2
│
├── src/
│ ├── train.py # Model training script
│ ├── infer_and_play.py # Testing + song playback
│ ├── utils.py # Helper functions
│
├── requirements.txt
└── README.md

---

## License
This project is licensed under the MIT License.
You are free to use, modify, and distribute it with attribution.

## Author
Developed By Harsh Arora

