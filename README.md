# 🤖 AI-CASHIER (The Smart kiosks_)

This repository is a pre-built prototype of a **Smart Kiosk** powered by **LLM (Large Language Models)**. It provides an intelligent, interactive system that can engage in human-like conversations and perform kiosk-related functions seamlessly.

---

## 🧠 Overview

The AI-CASHIER system simulates a smart customer assistant integrated into kiosk systems. It uses speech-to-text (STT), natural language processing, and text-to-speech (TTS) to understand users, process their requests, and respond in a natural and human-like way.

---

## 🚀 Features

- 💬 AI-powered smart conversations using `LLM`
- 🎨 Clean and responsive UI integration (planned or partial)
- 🎤 Voice input and 🎧 output using speech components
- 🔄 Modular and extendable pipeline for adding new kiosk tasks

---

## 📁 Repository Structure

### `artifacts/`
Contains all data-related files and records.

- `raw_dataset/` — Raw, unprocessed data collected for development.
- `dataset/` — Cleaned and preprocessed dataset used for training/testing.

---

### `all_trials/`
Houses logs, scripts, or notebooks from various experiments and trials performed during model development and tuning.

---

### `config/`
Configuration and parameter management.

- `config.py` — Core configuration file (e.g., paths, flags).
- `params.py` — Hyperparameters and constants required throughout the codebase.

---

### `main/`
Main application logic and components.

#### `components/`
Each folder here is a module representing different kiosk functionalities:
- `speech_recognition/` — Handles audio input (STT).
- `text_to_speech/` — Converts text responses to speech output.
- `menu_manager/` — Manages and handles menu-related logic.
- `llm_engine/` — Manages LLM interaction and response generation.
- `data_preprocessing/` — Preprocess the conversation data 
- `Intent_recognition/` - Extracting intent from sentences using NLP 

#### `functions/`
Contains shared utility functions used across components (e.g., file handling, logging).

#### `pipelines/`
Defines modular pipeline objects for various components (e.g., STT-to-response flow).

#### `predifine/`
Predefined, hardcoded functions or templates (e.g., greeting, fallback responses).

---

### `models/`
Includes saved base and fine-tuned models required for prediction and inference (e.g., Whisper, TTS models, LLM weights).

---

### `nltk_data/`
Local storage for **Natural Language Toolkit (NLTK)** resources (e.g., tokenizers, stopwords).

---

## ✅ Getting Started

### 🔧 Installation
Make sure you have Python 3.8+ installed. Then set up your virtual environment:

```bash
python -m venv myenv
source myenv/bin/activate  # or myenv\Scripts\activate on Windows
pip install -r requirements.txt
```


## 📈 Code Flow Diagram
![AI-CASHIER Diagram](docs/Architecture.png)
