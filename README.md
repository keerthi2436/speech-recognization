# speech-recognization
This project is a Python-based voice recognition tool that:

Captures speech from a microphone

Detects the spoken language

Translates the recognized text into a user-specified language

Converts the translated text into speech

Ideal for beginners exploring speech processing, language translation, and text-to-speech (TTS) systems.

🚀 Features
🎧 Real-time speech recognition using Google Speech Recognition

🌐 Language detection and translation via Google Translate

🔊 Speech synthesis using gTTS (Google Text-to-Speech)

🗃️ Saves translated audio to local .mp3 files

📦 Requirements
Install dependencies using pip:
pip install SpeechRecognition googletrans==4.0.0-rc1 gTTS
Additional requirement:

PyAudio (for microphone access)

Install it via:
pip install pyaudio
If that fails (especially on Windows), install it via wheels: https://www.lfd.uci.edu/~gohlke/pythonlibs/#pyaudio

🛠️ How It Works
The user is prompted to input a target language (e.g., Hindi, Tamil).

The script captures speech input via a microphone.

It uses speech_recognition to convert the audio to text.

The spoken language is automatically detected using googletrans.

The recognized text is translated into the target language.

The translated sentence is synthesized into speech using gTTS.

The output .mp3 is saved and automatically played.

🌍 Supported Target Languages
Language	Code
Hindi	hi
Telugu	te
Tamil	ta
Kannada	kn
Malayalam	ml
Bengali	bn

🧪 Usage
python voice recognization.py
Then:

Enter the target language.

Speak into the microphone when prompted.

Listen to the translated audio playback.

📝 Notes
Works best in a quiet environment for accurate speech recognition.

Ensure microphone permissions are granted.

This project requires an active internet connection.

📁 Output
All translated audio files are saved under the outputs/ directory as:

outputs/captured_voice_<Language>.mp3
