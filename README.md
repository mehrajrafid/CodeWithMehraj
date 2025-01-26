# XAI-Lung-CNN: Lightweight CNN with Explainable AI for Early Lung Cancer Detection

## Overview
This project implements a Lightweight Convolutional Neural Network (CNN) using EfficientNet-B3 architecture, integrated with Explainable AI (XAI) techniques like Grad-CAM and SHAP, to enhance early detection of lung cancer. The model aims to provide accurate predictions and improve interpretability for medical imaging data.

## Features
- **EfficientNet-B3**: Lightweight CNN architecture optimized for performance and efficiency.
- **Explainable AI**: Integrated Grad-CAM and SHAP for visualizing and understanding model predictions.
- **Medical Imaging Analysis**: Handles CT scan data to classify lung cancer as Positive or Negative.
- **Visualization Tools**: Confusion matrices, Grad-CAM overlays, and ROC curves for detailed evaluation.

## Tools and Frameworks
- **Programming Languages**: Python
- **Libraries**: PyTorch, TensorFlow, EfficientNet-PyTorch, SHAP, NumPy, Matplotlib, OpenCV
- **Platform**: Google Colab

## Dataset
- The project uses a lung CT scan dataset for binary classification: `Positive (Cancer)` and `Negative (Healthy)`.
- **Note**: The dataset is not included in the repository due to privacy concerns. Update `train` and `test` paths with your dataset location in the code.

## Implementation Highlights
1. **Data Preprocessing**:
   - Noise reduction, resizing, normalization, and data augmentation techniques.
   - Organized training and validation datasets with an 80/20 split.
2. **Model Architecture**:
   - Fine-tuned EfficientNet-B3 with a custom classifier for binary classification.
3. **Explainability**:
   - Grad-CAM heatmaps to visualize class activations.
   - SHAP for feature importance and interpretability.
4. **Evaluation Metrics**:
   - Accuracy, Precision, Recall, F1-Score, Confusion Matrix, and ROC-AUC Curves.

## How to Run
1. Clone this repository:
   ```bash
   git clone https://github.com/mehrajrafid/XAI-Lung-CNN.git
2. Upload the notebook to Google Colab.
3. Install dependencies (as needed):
pip install efficientnet_pytorch shap
4. Update paths to your dataset in the code:
train_path, test_path, and other dataset directories.
5. Run the notebook cells sequentially to preprocess data, train the model, and evaluate results.
## Results
Training Accuracy: Achieved up to 97.8% during training.
Validation Accuracy: Achieved up to 94.0% on validation data.
Explainability: Grad-CAM and SHAP visualizations highlight regions of interest in lung CT scans for predictions.
## Visualizations
Confusion Matrix: Displays the classification results.
Grad-CAM Heatmaps: Overlay activations on original images for better understanding.
ROC Curve: Shows model performance for varying classification thresholds.
## Future Work
Extend to Multi-Class Classification for different types of lung diseases.
Optimize the model further for real-time deployment in clinical settings.
Explore more advanced XAI techniques for improved transparency.
## Feedback
Feel free to raise issues or provide feedback! Contributions are welcome to enhance the project further.
