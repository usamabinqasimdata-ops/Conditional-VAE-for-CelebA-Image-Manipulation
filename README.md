# Conditional VAE for CelebA Image Manipulation

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/usamabinqasimdata-ops/Conditional-VAE-for-CelebA-Image-Manipulation/blob/main/Conditional_VAE_for_CelebA_Image_Manipulation.ipynb)

## 📄 Table of Contents
1. [Project Overview](#1-project-overview)
2. [Features](#2-features)
3. [Installation and Setup](#3-installation-and-setup)
4. [Usage](#4-usage)
5. [Dataset](#5-dataset)
6. [Model Architecture](#6-model-architecture)
7. [License](#7-license)
8. [Contact](#8-contact)

---

## 1. Project Overview

This project demonstrates how to build and train a **Conditional Variational Autoencoder (CVAE)** model using **TensorFlow** and the **CelebA dataset**. The CVAE is a powerful generative model that can be used to:
*   Generate new images with specific, desired attributes (e.g., smiling, wearing glasses).
*   Modify existing images by changing their attributes (e.g., adding a beard).

This notebook provides a complete, end-to-end implementation of the CVAE architecture for image manipulation.

## 2. Features

*   **Conditional Image Generation:** Generate images conditioned on specific attributes.
*   **Image Attribute Manipulation:** Modify existing images by altering their latent representation based on attribute vectors.
*   **CVAE Implementation:** Custom implementation of the Conditional Variational Autoencoder using Keras.
*   **CelebA Dataset Integration:** Includes code for downloading, preprocessing, and handling the CelebA dataset.

## 3. Installation and Setup

### Prerequisites
*   Python 3.x
*   A machine with a GPU is highly recommended for training the CVAE model.

### Local Setup
1.  **Clone the repository:**
    ```bash
    git clone https://github.com/usamabinqasimdata-ops/Conditional-VAE-for-CelebA-Image-Manipulation.git
    cd Conditional-VAE-for-CelebA-Image-Manipulation
    ```
2.  **Install dependencies:**
    The required libraries are listed in `requirements.txt`.
    ```bash
    pip install -r requirements.txt
    ```

## 4. Usage

The entire project workflow is contained in the `Conditional_VAE_for_CelebA_Image_Manipulation.ipynb` Jupyter Notebook.

### Running the Notebook
1.  Start a Jupyter environment:
    ```bash
    jupyter notebook
    ```
2.  Open `Conditional_VAE_for_CelebA_Image_Manipulation.ipynb` and run the cells sequentially.

Alternatively, you can use the **"Open In Colab"** badge at the top of this README to run the notebook directly in Google Colab.

## 5. Dataset

The project uses the **CelebA (Large-scale CelebFaces Attributes) Dataset**. The notebook includes steps to download and prepare the dataset for training.

## 6. Model Architecture

The core of the project is the Conditional Variational Autoencoder (CVAE), which consists of:
*   **Encoder:** Maps the input image and desired attributes to a latent space distribution.
*   **Decoder:** Reconstructs the image from a sample drawn from the latent space and the conditioning attributes.
*   **Loss Function:** Combines a reconstruction loss (how well the image is reproduced) and a KL divergence loss (to ensure the latent space is well-structured).

## 7. License

This project is licensed under the **MIT License**. See the [LICENSE](LICENSE) file for details.

## 8. Contact

For any questions or suggestions, please contact the repository owner.
