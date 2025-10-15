JARVIS - Voice-Activated Virtual Assistant

**Jarvis** is a Python-based voice-activated virtual assistant capable of performing tasks such as web browsing, playing music, fetching news, and responding to user queries using **OpenAI's GPT-3.5-turbo model**.  
It mimics the behavior of popular assistants like **Alexa** or **Google Assistant**, but is fully custom-built.

---

🚀 Features

🎙️ Voice Recognition
- Utilizes the `speech_recognition` library to listen for and recognize user voice commands.  
- Activates upon detecting the wake word **"Jarvis"**.

🗣️ Text-to-Speech
- Converts text to speech using **pyttsx3** for offline voice output.  
- Uses **gTTS (Google Text-to-Speech)** and **pygame** for smooth, natural voice playback.

🌐 Web Browsing
- Opens popular websites such as:
  - Google  
  - YouTube  
  - Facebook  
  - LinkedIn  
- Triggered by simple voice commands like *"Open Google"* or *"Open YouTube."*

🎵 Music Playback
- Interfaces with a custom `musicLibrary` module.  
- Plays songs using stored web links through the browser.

📰 News Fetching
- Fetches the latest news headlines from **NewsAPI**.  
- Reads them aloud using the assistant’s text-to-speech engine.

🧠 OpenAI Integration
- Uses **OpenAI’s GPT-3.5-turbo** model to handle complex user queries.  
- Responds conversationally and intelligently like a real AI assistant.



⚙️ Workflow

1. **Initialization**  
   - Greets the user with: *"Initializing Jarvis..."*
2. **Wake Word Detection**  
   - Listens continuously for the wake word *"Jarvis"*.  
   - Acknowledges activation by replying: *"Ya."*
3. **Command Processing**  
   - Recognizes and interprets voice commands.  
   - Determines action type:
     - Open website  
     - Play music  
     - Fetch news  
     - Query OpenAI
4. **Response Generation**  
   - Executes the appropriate action.  
   - Provides output using either **pyttsx3** or **gTTS** voice engine.



🧰 Libraries Used

| Library | Purpose |
|----------|----------|
| `speech_recognition` | To capture and recognize voice commands |
| `webbrowser` | To open websites programmatically |
| `pyttsx3` | Offline text-to-speech conversion |
| `musicLibrary` | Custom module for music link storage |
| `requests` | To call NewsAPI and other APIs |
| `openai` | For GPT-based intelligent responses |
| `gTTS` | Google Text-to-Speech for natural voice output |
| `pygame` | To play the generated MP3 speech |
| `os` | File and system-level operations |

---

## 🧩 How It Works

```text
User Speaks  →  Speech Recognized  →  Command Interpreted  →  Action Executed  →  Voice Response
