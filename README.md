# Emotion Recognition AI

This repository contains an emotion recognition system that combines:

- A Connect Four AI using the minimax algorithm  
- A deep learning CNN model trained on the FER-2013 dataset for emotion classification  
- OpenCV-based face, eye, and smile detection with Haar cascades  
- Image preprocessing and visualization tools  

---

## Repository Structure

.
├── src/                  # Data preprocessing & training scripts
│   ├── data_prep.py      # Convert FER2013 CSV to structured dataset
│   ├── train_display.py  # CNN training & webcam emotion display
│
├── ConnectFourAI.py      # Minimax implementation for Connect Four
├── haarcascade/          # Haar cascades for face, eye, and smile detection
│   ├── haarcascade_frontalface_default.xml
│   ├── haarcascade_eye.xml
│   ├── haarcascade_smile.xml
│
├── imgs/
│   └── accuracy.png      # Model accuracy (left) and loss (right)
│
├── fer2013.csv           # Dataset file (not included, download separately)
├── requirements.txt      # Python dependencies
└── README.md

---

## Features

- Connect Four AI with recursive minimax and heuristic evaluation  
- Emotion Recognition CNN (trained on FER2013)  
- Webcam Integration: Detects faces and classifies emotions in real-time  
- Image Preprocessing: Circle detection, grid extraction, and color filtering  
- Haar Cascade Detection: Face, eyes, and smiles  

---

## Installation

Clone the repository and install dependencies:

git clone https://github.com/yourusername/emotion-recognition-ai.git
cd emotion-recognition-ai
pip install -r requirements.txt

---

## Usage

1. Preprocess the FER2013 dataset  
   python src/data_prep.py  

2. Train the CNN model  
   python src/train_display.py --mode train  

3. Run real-time emotion detection  
   python src/train_display.py --mode display  

4. Run Connect Four AI  
   python ConnectFourAI.py  

---

## Model Performance

Training performance is visualized in imgs/accuracy.png:

- Left graph: Model accuracy over epochs  
- Right graph: Model loss over epochs  

---

## Notes

- Requires Python 3.7 or later  
- Haar cascade XML files are included in the repo  
- The FER2013 dataset must be downloaded separately  

---

## License

This project is licensed under the MIT License.
