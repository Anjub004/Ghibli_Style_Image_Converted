# Ghibli Style Image Converter

**Description:**  
A CycleGAN-based Ghibli style converter that transforms photos into Ghibli-inspired artwork using a Gradio web interface. Designed for Google Colab GPU support for easy deployment.

## Overview

This repository implements a Ghibli-style image converter using a CycleGAN model. The project wraps the CycleGAN test phase into a Gradio interface that creates a temporary folder structure for single image inference, processing user-uploaded images into Ghibli-style outputs.

## Setup and Installation

1. **Clone the Repository:**
   ```bash
   git clone https://github.com/yourusername/ghibli-style-converter.git
   cd ghibli-style-converter
2. **Install Dependencies: Ensure you have Python 3.6+ and install required packages:**
    pip install -r requirements.txt
Your requirements.txt should include dependencies like PyTorch, torchvision, Gradio, OpenCV, etc.)

3.**CycleGAN Model:** Train your CycleGAN model using the pytorch-CycleGAN-and-pix2pix repository with two datasets:

- Domain A: Real photos.

- Domain B: Ghibli-style images.
Ensure your experiment name (e.g., ghibli_cyclegan) matches the configuration in the code.

* Usage
1. Run the Converter: Start the Gradio web interface by running:
  python app.py
This launches a local server (or shareable link in Colab) where users can upload an image.

2. Processing: The app creates a temporary folder structure, saves the uploaded image, runs the CycleGAN test script, and outputs the Ghibli-style transformed image.

* Notes
- Adjust folder paths and experiment names as needed to match your CycleGAN training configuration.
- For Google Colab, mount your drive if using stored datasets and ensure GPU is enabled.
