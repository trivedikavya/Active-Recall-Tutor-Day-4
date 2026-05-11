# Active Recall Tutor 🎓

Active Recall Tutor is an AI-powered voice application designed to help users master programming concepts through the science of active recall. The application acts as a personal coach, guiding users through different learning modes—Learn, Quiz, and Teach Back—using distinct AI voice personalities.

## 🚀 Features

* **Multi-Mode Learning**:
* **Learn**: The tutor provides clear, concise explanations of core topics.
* **Quiz**: Test your knowledge with targeted questions based on the course content.
* **Teach Back**: Explain a concept in your own words, and the tutor will grade your explanation and provide feedback.


* **Voice Personalities**: Each mode features a unique voice powered by Murf AI:
* **Matthew (Learn)**: A clear, educational voice.
* **Alicia (Quiz)**: An engaging, inquisitive voice.
* **Ken (Teach Back)**: A supportive, evaluative voice.


* **Intelligent Reasoning**: Powered by Google Gemini 2.0 Flash to understand user intent, track state, and provide contextually relevant educational support.
* **Seamless Voice Interface**: Uses AssemblyAI for high-accuracy speech-to-text transcription.

## 🛠️ Tech Stack

### Backend

* **Framework**: FastAPI.
* **LLM**: Google Gemini 2.0 Flash.
* **STT**: AssemblyAI.
* **TTS**: Murf AI.
* **Dependencies**: `python-dotenv`, `requests`, `python-multipart`.

### Frontend

* **UI**: HTML5, Tailwind CSS (Outfit font).
* **Logic**: Vanilla JavaScript (ES Modules).
* **API Client**: Axios.

## 📂 Project Structure

```text
├── backend/
│   ├── main.py                # FastAPI server configuration
│   ├── routes.py              # API endpoints and tutor logic
│   ├── day4_tutor_content.json # Course data (Variables, Loops)
│   ├── models.py              # Pydantic data schemas
│   └── requirement.txt        # Backend dependencies
├── frontend/
│   ├── index.html             # Main dashboard UI
│   ├── index.js               # Frontend state and audio logic
│   └── package.json           # Frontend dependencies
└── .env                       # API keys (Google, AssemblyAI, Murf)

```

## ⚙️ Setup & Installation

### Backend

1. Navigate to the `backend` directory.
2. Install dependencies:
```bash
pip install -r requirement.txt

```


3. Configure your `.env` file with the following keys:
```env
GOOGLE_API_KEY=your_key
ASSEMBLYAI_API_KEY=your_key
MURF_AI_API_KEY=your_key

```


4. Start the server:
```bash
python main.py

```



### Frontend

1. Navigate to the `frontend` directory.
2. Install Axios:
```bash
npm install

```


3. Open `index.html` via a local server (e.g., Live Server in VS Code).

## 📖 How to Use

1. **Start Class**: Click the "Start Class" button to begin your session.
2. **Select Topic**: Tell the tutor whether you want to learn about **Variables** or **Loops**.
3. **Choose Mode**: Switch between modes by telling the tutor you want to "Learn," "Quiz," or "Teach back".
4. **Interact**: Use the microphone button to speak. The tutor will respond with audio and update your current learning state and feedback on the screen.
