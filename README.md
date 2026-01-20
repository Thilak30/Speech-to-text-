# Speech-to-Text using OpenAI's Whisper

This project demonstrates how to perform speech-to-text transcription using OpenAI's powerful [Whisper](https://github.com/openai/whisper) model. It includes a Jupyter Notebook that serves as a step-by-step guide to installing the required libraries, loading the model, processing audio files, and generating transcriptions.

## 📝 Overview

The primary component of this project is the `Speech_to_text.ipynb` notebook. It covers the following steps:

1.  **Setup**: Installing necessary Python libraries and the Whisper package.
2.  **Model Loading**: How to load different versions of the Whisper model (e.g., tiny, base, medium).
3.  **Audio Processing**: Loading audio files, visualizing waveforms, and preparing audio for the model (padding/trimming).
4.  **Feature Extraction**: Computing the Log-Mel Spectrogram required by the model.
5.  **Transcription**: Decoding the audio features to produce the final text output.

## 🛠️ Prerequisites

To run this notebook, you will need:

*   **Python**: Version 3.9 or higher is recommended.
*   **Jupyter Notebook** or **Google Colab**: To open and execute the `.ipynb` file.

The notebook relies on the following key libraries:
*   `torch` (PyTorch)
*   `openai-whisper`
*   `librosa` (for audio processing)
*   `matplotlib` & `seaborn` (for visualization)
*   `numpy` & `pandas` (for data manipulation)

## 📦 Installation

The notebook includes cells to install dependencies directly. If you are running this locally, you can install the main requirements using pip:

```bash
# Core data science and audio libraries
pip install pandas numpy seaborn matplotlib scikit-learn librosa

# PyTorch (Visit https://pytorch.org/ for command specific to your system)
pip install torch

# OpenAI Whisper
pip install git+https://github.com/openai/whisper.git
```

## 🚀 Usage

1.  Open `Speech_to_text.ipynb` in Jupyter Lab, Jupyter Notebook, or Google Colab.
2.  Execute the cells in order.
3.  **Custom Audio**: By default, the notebook might point to a sample file (e.g., `/content/sample_video.mp4`). You can update the `file_path` variable to point to your own local audio file (e.g., `.mp3`, `.wav`, `.mp4`).

```python
# Example: changing the file path in the notebook
file_path = 'path/to/your/audio_file.mp3'
```

## 📊 Models

Whisper provides several model sizes offering a trade-off between speed and accuracy:

*   `tiny`
*   `base`
*   `small`
*   `medium`
*   `large`

The notebook demonstrates loading the `medium` model, but you can easily switch to others by modifying the `whisper.load_model()` call.

## 🤝 Contributing

Feel free to fork this project and submit pull requests if you have improvements or additional examples!
