## Reference :
https://chatgpt.com
# Data Augmentation Pipeline

This project implements a data augmentation pipeline for text, audio, image, and sensor data. 
The goal is to enhance the diversity of data through various augmentation techniques.

## Table of Contents

- [Installation](#installation)
- [Usage](#usage)
- [Configuration](#configuration)
- [Augmentation Techniques](#augmentation-techniques)
  - [Text Augmentation](#text-augmentation)
  - [Audio Augmentation](#audio-augmentation)
  - [Image Augmentation](#image-augmentation)
  - [Sensor Augmentation](#sensor-augmentation)


## Installation

1.Create the virtual environment:
```
conda create --name data_augmentation_env python=3.12

```
2.On windows, you can activate the virtual environment using :
```
conda activate data_augmentation_env
```
On mac, linux the command is :
```
source activate data_augmentation_env
```
3.Install the required dependencies:
    ```bash
    pip install -r requirements.txt
    ```
4.Ensure you have NLTK data:
    python
    # import nltk
    # nltk.download('wordnet')
    # nltk.download('punkt')
    

## Usage

To run the augmentation pipeline, use the following command:

```
Run the code cell in bhadani_sristi.ipynb
or 
joita_soham.ipynb

```

## Configuration
Use the provided JSON configuration file to specify the settings for data augmentation.
Below is an example configuration file:
```
{
    "text_data": {
        "file_path": "/path/to/text_data.csv",
        "sentiment_column": "label"
    },
    "data_augmentation": {
        "text_augmentation": {
            "output_path": "/path/to/augmented_text",
            "synonym_replacement": {
                "enabled": true,
                "top_n": 3
            },
            "add_noise": {
                "enabled": true,
                "noise_level": "low"
            },
            ...
        },
        "audio_augmentation": {
            "file_path": "/path/to/audio_file.wav",
            "output_path": "/path/to/augmented_audio",
            "sample_rate": 16000,
            ...
        },
        "image_augmentation": {
            "file_path": "/path/to/image_directory",
            "output_path": "/path/to/augmented_images",
            ...
        },
        "sensor_augmentation": {
            "script_path": "/path/to/sensor_data.csv",
            "output_path": "/path/to/augmented_sensor_data",
            ...
        }
    }
}
```
## Augmentation techniques
# Text Augmentation
    Synonym Replacement
    Add Noise
    Random Insertion
    Random Deletion
    Random Swap
    Correct Grammar
    BERT Augmentation
    Generation
    Back Translation
    Paraphrasing
    Style Transfer NMT
    Text Generation from Graph Structures
    Hierarchical Text Generation
    Conditional Text Generation
    Stochastic Text Generation
# Audio Augmentation
    Add Noise
    Reverse Audio
    Change Speed
    Slow Down Audio
    Add Echo
# Image Augmentation
    Random Horizontal Flip
    Random Rotation
    Grayscale
    Random Vertical Flip
    Color Jitter
    Random Affine
    Gaussian Blur
    Random Posterize
    Center Crop
    Random Perspective
    Elastic Transform
# Sensor Augmentation
    Gaussian Noise
    Uniform Noise
    DA Jitter
    DA Scaling
    Generate Random Curves
    Distort Timesteps
    DA Permutation