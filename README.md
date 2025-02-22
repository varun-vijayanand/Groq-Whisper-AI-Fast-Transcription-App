# Groq-Whisper-AI-Fast-Transcription-App

This Streamlit-based app allows users to transcribe audio files or YouTube videos using Groq Whisper API. It provides two main functionalities:

- Upload an MP3 file for transcription.
- Input a YouTube URL, download the audio, and transcribe it.

Features
- Audio Upload: Upload any MP3 file, re-encode it to OGG format to reduce file size, and transcribe it using the Groq Whisper API.
- YouTube Audio Download: Provide a YouTube link, download the audio, re-encode it to OGG, and get a transcription.
- Re-encoding: Uses ffmpeg to re-encode MP3 files to the Opus codec in OGG format, ensuring compatibility with Whisper's input limits (maximum 25MB).
- Audio Embedding: After re-encoding, the audio file is embedded in the Streamlit app with a player for users to listen to the audio directly.

Technologies Used
- Streamlit: Used for building the web interface.
- yt-dlp: To download YouTube videos and extract audio.
- pydub: Audio processing library.
- ffmpeg: Used for re-encoding the audio into OGG format.This compresses the audio significantly while retaining quality suitable for transcription.
- Groq Whisper API: Used for transcribing the audio.
- Python: Core programming language for the app.
