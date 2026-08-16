# 🎙️ Speech-To-Text ASR (Automatic Speech Recognition)

An end-to-end **Automatic Speech Recognition (ASR)** pipeline that converts speech audio into text using state-of-the-art deep learning models, with an interactive **Gradio** web interface for real-time transcription.

---

## 📌 Project Overview

This project demonstrates how to:
- Load and explore the **LibriSpeech** ASR dataset using HuggingFace `datasets` (streaming mode)
- Build an ASR inference pipeline with **NVIDIA Parakeet TDT 0.6B v3** model via HuggingFace `transformers`
- Deploy the model through a user-friendly **Gradio** web application supporting both file upload and microphone input

---

## 🛠️ Tech Stack

| Technology | Purpose |
|---|---|
| [HuggingFace Transformers](https://huggingface.co/docs/transformers) | ASR model pipeline |
| [NVIDIA Parakeet TDT](https://huggingface.co/nvidia/parakeet-tdt-0.6b-v3) | Pre-trained ASR model |
| [HuggingFace Datasets](https://huggingface.co/docs/datasets) | Dataset loading & streaming |
| [Gradio](https://www.gradio.app/) | Interactive web UI |
| [Librosa](https://librosa.org/) | Audio processing |
| [SoundFile](https://pysoundfile.readthedocs.io/) | Audio file I/O |

---

## 📂 Project Structure

```
Speech-To-Text-ASR/
├── Speech_To_Text_ASR.ipynb   # Main notebook with full pipeline
├── requirements.txt           # Python dependencies
├── .gitignore                 # Git ignore rules
├── LICENSE                    # MIT License
└── README.md                  # This file
```

---

## 🚀 Getting Started

### Prerequisites
- Python 3.8+
- pip package manager
- (Optional) Google Colab for GPU acceleration

### Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/<your-username>/Speech-To-Text-ASR.git
   cd Speech-To-Text-ASR
   ```

2. **Install dependencies**
   ```bash
   pip install -r requirements.txt
   ```

3. **Run the notebook**
   ```bash
   jupyter notebook Speech_To_Text_ASR.ipynb
   ```

### Running on Google Colab
You can also open the notebook directly in Google Colab — all installation commands are included in the first cell.

---

## 📖 Notebook Sections

| # | Section | Description |
|---|---------|-------------|
| 1 | Environment Setup | Install required libraries |
| 2 | Load Dataset | Stream LibriSpeech ASR data |
| 3 | Audio Playback | Listen to audio samples in-notebook |
| 4 | Build ASR Pipeline | Load NVIDIA Parakeet model |
| 5 | Run Inference | Transcribe sample audio |
| 6 | Gradio Web App | Deploy interactive transcription UI |

---

## 🎯 Model Details

- **Model**: `nvidia/parakeet-tdt-0.6b-v3`
- **Task**: Automatic Speech Recognition (ASR)
- **Architecture**: FastConformer with Token-and-Duration Transducer (TDT)
- **Parameters**: ~600M
- **Sampling Rate**: 16kHz

---

## 📝 License

This project is licensed under the MIT License — see the [LICENSE](LICENSE) file for details.

---

## 🤝 Contributing

Contributions, issues, and feature requests are welcome! Feel free to open an issue or submit a pull request.

---

## ⭐ Acknowledgments

- [HuggingFace](https://huggingface.co/) for the Transformers & Datasets libraries
- [NVIDIA NeMo](https://github.com/NVIDIA/NeMo) for the Parakeet ASR model
- [LibriSpeech](http://www.openslr.org/12/) for the open-source ASR dataset
- [Gradio](https://www.gradio.app/) for the web interface framework
