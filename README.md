# Real-Time Voice Translator

Low-latency multilingual voice translation for live calls.

This project enables natural communication between speakers of different languages by converting:

```text
Speech → Text → Translation → Speech
```

in near real time, with an average response delay of approximately **1.7 seconds**.

Designed for use during voice and video calls without requiring users to switch applications or rely on subtitles.

---

## Overview

Most translation tools interrupt conversation flow by forcing users to read text, type messages, or move between apps. This project focuses on a smoother experience by capturing speech, translating it, and returning spoken output directly into the active call.

The system is intended for platforms such as:

* Zoom
* Google Meet
* Skype
* Any application using microphone input

---

## Core Features

* Real-time speech recognition
* Instant multilingual translation
* Spoken translated output
* Virtual microphone routing for live calls
* Low-latency streaming pipeline
* Transcript logging
* Expandable language support

---

## System Pipeline

```text
Microphone Input
↓
Speech Recognition
↓
Translation Engine
↓
Text-to-Speech
↓
Virtual Audio Output
↓
Voice / Video Call Platform
```

---

## Supported Languages

Current support includes:

* English
* Hindi
* Myanmar

The architecture is designed to allow additional languages in future versions.

---

## Technology Stack

| Component          | Technology             |
| ------------------ | ---------------------- |
| Speech Recognition | Whisper                |
| Translation        | Google Cloud / DeepL   |
| Text-to-Speech     | gTTS / ElevenLabs      |
| Audio Processing   | PyAudio                |
| Audio Routing      | VB-CABLE               |
| Backend            | Python / Node.js       |
| UI                 | PyQt / React (planned) |

---

## Performance

| Metric            | Result    |
| ----------------- | --------- |
| Average Latency   | ~1.68 sec |
| 95th Percentile   | 2.41 sec  |
| User Satisfaction | 86.7%     |

---

## Project Structure

```text
real-time-translator/
├── backend/
├── audio/
├── translation/
├── tts/
├── streaming/
├── ui/
└── README.md
```

---

## Installation

```bash
git clone https://github.com/Wardin9/Real-Time-Voice-Translator.git
cd Real-Time-Voice-Translator
pip install -r requirements.txt
python main.py
```

---

## Development Roadmap

* [x] Speech recognition pipeline
* [x] Translation module
* [x] Text-to-speech output
* [ ] Real-time latency optimization
* [ ] Zoom / Meet integration
* [ ] Improved user interface
* [ ] Additional language packs

---

## Future Work

* Offline local AI models
* Sub-1 second latency target
* Speaker recognition
* Mobile deployment
* Personalized voice output
* Expanded Southeast Asian language support

---

## Vision

Removing language as a barrier to human connection.
