# Electronic-Component-Identification-with-AI

This project uses a fine-tuned YOLOv8 model to identify and locate common electronic components in real-time.

---
## Components Identified
* Resistors
* Capacitors
* Diodes
* LEDs
* LDRs
* Buttons

---
## Quick Start

### 1. Setup
Clone this repository and install the necessary packages.

```bash
git clone [https://github.com/USOman21/Electronic-Component-Identification-with-AI.git](https://github.com/USOman21/Electronic-Component-Identification-with-AI.git)
cd Electronic-Component-Identification-with-AI
pip install ultralytics
```

2. Run a Prediction

Use the following Python script to run the model on your own image.

```
from ultralytics import YOLO

# Load the trained model
model = YOLO('./runs/detect/train/weights/best.pt')

# Run inference on an image and display the results
results = model('path/to/your/image.jpg', save=True)
```
The resulting image with bounding boxes will be saved in a runs/detect/predict folder.
