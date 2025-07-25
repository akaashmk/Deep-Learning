# Malaria Diagnosis Project

A deep learning-based image classification project to detect malaria-infected cells. The system uses Convolutional Neural Networks (CNNs) to classify cell images as either **"Parasite" (infected)** or **"Uninfected"**.

---

## Features

- Loads and preprocesses the malaria image dataset using TensorFlow Datasets.
- Splits the dataset into training, validation, and test sets.
- Includes image augmentation and normalization for better generalization.
- Builds CNN models using both **Sequential** and **Functional** APIs from Keras.
- Visualizes training/validation accuracy and loss.
- Evaluates model performance using accuracy, loss, confusion matrix, and ROC curve.
- Saves trained models in HDF5 format.
- Predicts and visualizes results on test images.

---

## Requirements

Ensure Python 3.x is installed, then install the required Python packages:

```bash
pip install tensorflow numpy matplotlib scikit-learn opencv-python seaborn tensorflow-datasets
```

---

## Project Structure

```
malaria-diagnosis-project/
├── malarie_diagonasis.ipynb   # Main Jupyter notebook
├── malaria_model.hdf5         # Saved trained model
├── README.md                  # Project documentation
```

---

## Usage

**Clone the Repository:**

```bash
git clone https://github.com/your-username/malaria-diagnosis-project.git
cd malaria-diagnosis-project
```

**Install Dependencies:**

```bash
pip install -r requirements.txt
```

**Run the Notebook:**
Open `malarie_diagonasis.ipynb` using Jupyter Notebook or JupyterLab and follow the code to train, evaluate, and test the CNN model.

---

## Dataset

This project uses the Malaria Cell Images Dataset provided through TensorFlow Datasets:

- 27,558 cell images labeled as “Parasitized” or “Uninfected”.
- Images have a consistent size of 128x128x3 pixels.

For more details, see [Malaria Dataset Documentation](https://www.tensorflow.org/datasets/catalog/malaria).

---

## Model Architecture

- Multiple Convolutional Layers for feature extraction
- Batch Normalization for training stability
- Max Pooling layers for spatial downsampling
- Fully-connected (Dense) layers for classification
- Final Sigmoid-activated output layer for binary classification

---

## Results

- Training and validation accuracy and loss are plotted during training.
- Performance metrics include:
  - Accuracy
  - Loss
  - Confusion Matrix
  - ROC Curve (optional)
- Visualization of test predictions shows classification results on sample images.

---

## GPU Support

This project includes automatic detection and usage of a GPU (if available), significantly speeding up model training when using compatible hardware (e.g., NVIDIA GPUs with CUDA support).
