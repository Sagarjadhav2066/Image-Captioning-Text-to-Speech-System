# Image-Captioning-Text-to-Speech-System
📌 Image Captioning & Text-to-Speech (TTS) System
An AI-based accessibility tool for visually impaired users
This project transforms images and short video clips into descriptive captions and then converts those captions into speech audio, helping visually impaired users understand their surroundings.
Built using BLIP (Bootstrapping Language-Image Pretraining) for captioning and gTTS for audio synthesis.

🚀 Project Overview
✅ Image Captioning
Uses Salesforce/BLIP-image-captioning-base
Generates accurate captions for:
Single images
Multiple images
Extracted frames from short videos

✅ Video Support
Processes 2–5 second MP4 videos
Extracts frames using OpenCV
Generates caption per frame → creates a visual narrative

✅ Audio Generation

Caption text → spoken audio using gTTS
Automatically saves, plays, and deletes MP3 files
Includes sequential playback with delay for clarity

🌍 Supported Languages
| Code   | Language          |
|--------|-------------------|
| en     | English           |
| es     | Spanish           |
| fr     | French            |
| de     | German            |
| it     | Italian           |
| pt     | Portuguese        |
| zh-CN  | Chinese (Mandarin)|
| hi     | Hindi             |
| ru     | Russian           |
| ar     | Arabic            |


🎯 Goal:
To provide real-time scene understanding to visually impaired individuals through audio descriptions.


🛠️ Technologies & Libraries Used
| Purpose          | Library               |
| ---------------- | --------------------- |
| Image captioning | `transformers`        |
| Deep learning    | `torch`               |
| Image processing | `Pillow`              |
| Text-to-speech   | `gTTS`                |
| Audio playback   | `IPython.display`     |
| Video processing | `opencv-python (cv2)` |
| Utilities        | `os`, `time`          |


🧰 How It Works
1️⃣ Load BLIP Model
Loads processor and model from HuggingFace
Converts media to RGB
Tokenizes input

2️⃣ Generate Caption
Model predicts caption using vision-language encoding

3️⃣ Convert Caption → Speech
gTTS converts caption into MP3 audio
Audio is played using notebook display elements

4️⃣ Video Support
Extract frames using cv2.VideoCapture
Caption each frame
Generate a sequential speech narration

🔮 Future Enhancements
Real-time webcam captioning
Mobile app deployment (TFLite)
Offline TTS/ML model
Improved UI



