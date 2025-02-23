# Driver Drowsiness Detection Using CNN

## Overview
Driver drowsiness is a critical issue leading to accidents and fatalities. This project presents a non-intrusive, cost-effective drowsiness detection system utilizing a Convolutional Neural Network (CNN) to analyze eye closure and yawning using camera input.

## Features
- Detects drowsiness based on eye closure and yawning
- Uses CNN for real-time image classification
- Non-intrusive and cost-effective (requires only a camera)
- High accuracy and efficiency with optimized architecture

## Model Architecture
- **Input:** 145x145 RGB images
- **Convolutional layers:** 512, 512, and 256 filters (ReLU activation)
- **Max-pooling layers:** 2x2 to reduce spatial dimensions
- **Dropout:** 50% to prevent overfitting
- **Fully connected layers:** 128, 64 neurons
- **Softmax output:** Classification into yawn, no yawn, closed eyes, open eyes
- **Optimizer:** Adam
- **Loss Function:** Categorical Cross-Entropy

## Performance
- **Training Accuracy:** 96.21%
- **Testing Accuracy:** 96.54%
- **Weighted Average F1-Score:** 0.94
- **Weighted Average Recall (Sensitivity):** 94.10%
- **Weighted Average Specificity:** 97.95%

## Installation & Usage
### Clone the repository:
```bash
git clone https://github.com/nehalmahajan26/driver-drowsiness
cd driver-drowsiness-detection
```

### Install dependencies:
```bash
pip install -r requirements.txt
```

### Train the model:
```bash
python train.py
```

### Run real-time detection:
```bash
python detect.py
```

## Dataset
Augmented dataset with labeled images for yawn, no yawn, closed eyes, and open eyes.

## License
MIT License


