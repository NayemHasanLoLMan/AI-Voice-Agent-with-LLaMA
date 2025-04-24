# 🗣️🦙 AI Voice Agent with LLaMA + Deepgram + ElevenLabs

This project is an **experimental AI voice assistant** built using a **locally hosted LLaMA model** for conversational logic, **Deepgram** for speech-to-text (STT), and **ElevenLabs** for text-to-speech (TTS).

The aim is to test the **viability and performance of local LLaMA models** as real-time voice agents, exploring responsiveness, latency, and conversational capability in audio-driven interactions.

---

## 🎯 Project Objectives

- 🔍 Test **LLaMA's performance** in voice-based real-time conversation
- 🗣️ Convert user speech to text using **Deepgram**
- 🔊 Convert chatbot responses back to audio using **ElevenLabs**
- 🔄 Create a seamless **voice input → text processing → voice output** pipeline
- 🧪 Experiment and measure latency and naturalness for use cases like virtual assistants

---

## 🧠 Tech Stack

| Component    | Technology Used                |
|--------------|--------------------------------|
| LLM Engine    | Local LLaMA Model (e.g. `llama.cpp`, `transformers`) |
| STT Engine    | Deepgram API                   |
| TTS Engine    | ElevenLabs API                 |
| Backend       | Python (FastAPI / Flask)       |
| Audio Control | `pyaudio`, `wave`, `ffmpeg`    |

---




## 🚀 Getting Started


1. Clone the Repository


        git clone https://github.com/yourusername/ai-voice-llama-agent.git
        cd ai-voice-llama-agent


2. Create Environment & Install Dependencies


        python -m venv env
        source env/bin/activate
        pip install -r requirements.txt


3. Setup Environment Variables


       cp .env.example .env


## 🎙️ How It Works

- 🎧 Listen – Captures audio input from the microphone
- 📝 Transcribe – Sends audio to Deepgram and receives transcript
- 🧠 Respond – Passes transcript into local LLaMA model for generating reply
- 🔊 Speak – Uses ElevenLabs to synthesize and play the response as speech



## 🔧 Environment Variables


    DEEPGRAM_API_KEY=your_deepgram_key
    ELEVENLABS_API_KEY=your_elevenlabs_key
    LLAMA_MODEL_PATH=path_to_your_local_llama_model



## 📊 Experimental Focus

🕒 Response time (input → output)
🗣️ Conversational fluency of local models
🔉 Voice quality and naturalness
📈 CPU/GPU performance benchmarks (optional)



## 🧪 Future Enhancements
 
 - Add wake word detection ("Hey Aria")
 - WebRTC support for browser-based mic interaction
 - Switchable voices in ElevenLabs
 - Multi-turn memory (conversation history)

## 🛡️ License

MIT License – Use freely for research or personal voice projects.

##🤝 Contributing

Want to help test with new local models or optimize latency? Feel free to fork, star, or PR.
