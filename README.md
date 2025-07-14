# Emotion Recognition from Facial Images using CNN

This project is a deep learning-based facial emotion recognition system developed using TensorFlow and Keras. The model is trained to classify facial expressions into 7 emotion categories using a custom dataset.

Features:
- Trained CNN model for emotion classification
- Uses data augmentation to improve model generalization
- Evaluates model on a separate test dataset
- Saves trained model for future use (`face_recognition.keras`)
- Predicts emotion from unseen facial images

Dataset Structure:
Place your dataset in the following folder structure:

train/
  ├── Angry/
  ├── Happy/
  ├── Sad/
  ├── Surprise/
  ├── Neutral/
  ├── Fear/
  └── Disgust/

test/
  ├── Angry/
  ├── Happy/
  ├── Sad/
  ├── Surprise/
  ├── Neutral/
  ├── Fear/
  └── Disgust/

Requirements:
Install the required Python libraries:

pip install tensorflow keras matplotlib

How to Run:
1. Place your dataset in the `train/` and `test/` folders.
2. Open the `face_recognition.ipynb` notebook in Jupyter Notebook or VSCode.
3. Run all cells to:
   - Load and preprocess the data
   - Train the CNN model
   - Visualize training and validation accuracy/loss
   - Evaluate on test data
   - Save model as `face_recognition.keras`
   - Predict emotion from a new image

Model Info:
- Input: 48x48 RGB images
- Architecture: 4 Conv2D layers, MaxPooling, Dropout, BatchNormalization
- Dense layers with softmax output
- Optimizer: Adam
- Loss: Categorical Crossentropy
- Output: 7 emotion classes

Outputs:
- Trained model: `face_recognition.keras`
- Model performance plots: accuracy & loss graphs
- Final evaluation: test accuracy and loss printed
- Predicted emotion shown for uploaded image
