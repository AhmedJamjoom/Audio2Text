# Audio2Text


# 🎙️ AI Voice Demo (Python)

A simple Python project that demonstrates converting audio to text, generating an AI-based response, and turning that response back into realistic speech using OpenAI’s APIs.

---

## 🎯 Project Objectives

- 🎧 Transcribe audio files using OpenAI Whisper
- 💬 Generate AI responses using Large Language Models (LLMs)
- 🔊 Synthesize speech with OpenAI’s Text-to-Speech (TTS)
- 🔐 Secure API keys using environment variables
- 📦 Package a complete AI audio pipeline in a single script

---

## 🧱 What the Script Does

The `main.py` script provides a full pipeline:

1. **Transcription**: Converts any audio file (e.g., `.m4a`) to text using `whisper-1`.
2. **Response Generation**: 
   - You can choose between a static, humorous message, or
   - Let ChatGPT (e.g., `gpt-3.5-turbo`) generate a live response.
3. **Speech Synthesis**: Converts the response back to audio using OpenAI’s TTS (`tts-1`) and saves it as an `.mp3`.

---

## 🛠️ Technologies Used

- 🧠 OpenAI Whisper (`whisper-1`)
- 💬 GPT-3.5 Turbo (for AI responses)
- 🔊 OpenAI TTS (e.g., voice = `shimmer`)
- 🐍 Python 3.8+
- 📦 `openai` Python SDK
- 🖥️ Tested on Windows 11

---

## ⚙️ How It Works

### 1. Transcribe
```python
client.audio.transcriptions.create(...)
```
Converts the input audio to text using Whisper.

### 2. Respond
```python
client.chat.completions.create(...)
```
Generates a funny or intelligent reply using ChatGPT.

### 3. Speak
```python
client.audio.speech.create(...)
```
Generates an `.mp3` file using OpenAI’s realistic voice models.

---

## 👤 Author

> Created by **Ahmed Jamjoom**  
> 📅 Date: July 17, 2025
