# Emotion Recognition AI

This repository contains an emotion recognition system that combines:

- A Connect Four AI using the minimax algorithm  
- A deep learning CNN model trained on the FER-2013 dataset for emotion classification  
- OpenCV-based face, eye, and smile detection with Haar cascades  
- Image preprocessing and visualization tools  

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
```bash
git clone https://github.com/yourusername/emotion-recognition-ai.git
cd emotion-recognition-ai
pip install -r requirements.txt
```
---

## Usage

1. Preprocess the FER2013 dataset  
```bash
   python src/data_prep.py  
```
2. Train the CNN model
   ```bash
   python src/train_display.py --mode train  
   ```
3. Run real-time emotion detection
   ```bash  
   python src/train_display.py --mode display  
   ```
4. Run Connect Four AI
   ```bash  
   python ConnectFourAI.py  
   ```
---

## Model Performance

Training performance is visualized here:

![Model Performance](imgs/accuracy.png)
---

## Notes

- Requires Python 3.7 or later  
- Haar cascade XML files are included in the repo  
- The FER2013 dataset must be downloaded separately  

---

## License

This project is licensed under the MIT License.
