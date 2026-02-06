# Face Recognition & Reconstruction via Auto-Encoders

## Overview
This project explores the use of **Convolutional Auto-Encoders (CAEs)** for facial recognition and image reconstruction. By compressing facial images into a lower-dimensional "latent space" and then reconstructing them, the model learns robust feature representations that are highly effective for identification tasks.

## Key Files
* **`Train_AutoEncoder.ipynb`**: The main Jupyter Notebook containing the data pipeline, model architecture, training loop, and visualization of results. **Click this file to view the full project.**
* **`utils.py`**: Helper script containing utility functions for data loading and preprocessing.

## Installation & Usage

### 1. Prerequisites
Ensure you have Python installed along with the necessary data science libraries. You can install them via pip:

```bash
pip install tensorflow numpy pandas matplotlib scipy jupyter
```

### 2. Running the Project
Since the core logic is contained in a Jupyter Notebook, you can run the project interactively:

1.  Clone the repository or download the files.
2.  Launch Jupyter Notebook:
    ```bash
    jupyter notebook
    ```
3.  Open **`Train_AutoEncoder.ipynb`**.
4.  Run the cells sequentially to train the model and visualize the reconstruction results.

## Methodology
1.  **Encoder:** A series of Convolutional and Pooling layers reduce the input image to a compressed representation.
2.  **Latent Space:** The bottleneck layer that holds the encoded features.
3.  **Decoder:** Transposed Convolutional layers reconstruct the image from the latent vector.
4.  **Training:** The model is trained to minimize the Mean Squared Error (MSE) between the original and reconstructed images.

## Tech Stack
* **Deep Learning:** TensorFlow / Keras
* **Data Processing:** NumPy, Pandas, SciPy
* **Visualization:** Matplotlib
