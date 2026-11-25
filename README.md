# Simran AI – Your Personal Voice Assistant

**Your laptop. Your voice. Your personal AI assistant.**

Simran AI is an AI-powered personal desktop voice assistant designed for Debian Linux. It understands natural voice commands in **English and Telugu**, interacts with your laptop, launches applications, manages files, plays music, assists with food discovery and ordering, and helps manage everyday tasks.

The goal of Simran is to create a smart, personalized AI agent that makes everyday computer interactions easier through natural voice conversations.

## ✨ Key Features

### 🎙️ Voice Interaction
- Natural voice-based conversations.
- English and Telugu language support.
- Wake-word activation using "Hey Simran".
- Speech-to-text and text-to-speech.
- Voice responses and conversational interaction.

### 💻 Desktop Automation
- Open desktop applications using voice commands.
- Launch folders, files, and development projects.
- Open websites and browser pages.
- Control supported desktop functions.
- Execute approved automation tasks.

### 🎵 Smart Music Assistant
- Search songs by name or artist.
- Play music based on mood or preference.
- Play, pause, resume, and skip tracks.
- Control media playback through voice commands.

### 🍔 Food Assistant
- Discover food and restaurants.
- Search available menu items.
- Compare food options and prices.
- Prepare shopping carts.
- Support order placement with user confirmation.

### 📅 Personal Productivity
- Create reminders and daily tasks.
- Manage personal notes.
- Maintain conversation history.
- Remember user-approved preferences.
- Assist with everyday activities.

### 🧠 AI Intelligence
- Understand natural-language instructions.
- Identify user intent.
- Select appropriate tools to complete tasks.
- Maintain conversational context.
- Provide natural voice responses.

## 🏗️ Architecture

Simran follows a modular architecture:

```text
                 USER
                   |
             Voice Command
                   |
             Voice Processing
                   |
               AI AGENT
                   |
             Intent Detection
                   |
               TOOL ROUTER
                   |
       +-----------+-----------+
       |           |           |
    Desktop      Music        Food
    Control     Assistant   Assistant
       |           |           |
       +-----------+-----------+
                   |
          Permission & Safety
                   |
            Task Execution
                   |
          Voice Response
                   |
                  USER
```

## 🛠️ Technology Stack

| Component | Technology |
|---|---|
| Programming Language | Python |
| AI Intelligence | OpenAI API |
| Agent Framework | OpenAI Agents SDK |
| Voice Processing | OpenAI Realtime API / Audio APIs |
| Backend | FastAPI |
| Desktop Interface | PySide6 |
| Wake Word | openWakeWord |
| Database | SQLite |
| Browser Automation | Playwright |
| Testing | Pytest |
| Operating System | Debian Linux |

## 📂 Project Structure

```text
simran-ai/
├── app/
│   ├── agent/
│   ├── voice/
│   ├── tools/
│   ├── safety/
│   ├── memory/
│   ├── api/
│   ├── config.py
│   └── main.py
├── desktop/
│   ├── pages/
│   ├── components/
│   └── window.py
├── tests/
├── data/
├── docs/
├── .env.example
├── .gitignore
├── requirements.txt
└── README.md
```

## 🚀 Getting Started

### Prerequisites

- Debian Linux
- Python 3.11 or later
- Git
- OpenAI API key
- Working microphone and speakers

### 1. Clone the repository

```bash
git clone https://github.com/YOUR_USERNAME/simran-ai.git
cd simran-ai
```

### 2. Create a virtual environment

```bash
python3 -m venv .venv
source .venv/bin/activate
```

### 3. Install dependencies

```bash
python -m pip install --upgrade pip
pip install -r requirements.txt
```

### 4. Configure environment variables

Create a `.env` file:

```env
OPENAI_API_KEY=your_openai_api_key
```

Keep your API key private. Never commit `.env` to GitHub.

### 5. Run Simran

```bash
python -m app.main
```

*Note: Setup and execution instructions will be updated as the implementation progresses.*

## 🗺️ Development Roadmap

- [ ] Project foundation and desktop interface
- [ ] Voice input and output
- [ ] English and Telugu voice support
- [ ] Wake-word detection
- [ ] OpenAI agent integration
- [ ] Conversational memory
- [ ] Desktop application control
- [ ] File and folder management
- [ ] Music assistant
- [ ] Food discovery and ordering workflow
- [ ] Reminders and productivity tools
- [ ] Permission and confirmation system
- [ ] Testing and error handling
- [ ] Final dashboard and documentation

## 🔐 Security and Privacy

Simran is designed with a local-first execution approach.

- Desktop operations are executed locally.
- API credentials are stored in environment variables.
- Sensitive actions require user confirmation.
- File deletion and arbitrary terminal commands are restricted by default.
- Food orders and payments require explicit approval.
- User preferences and stored information should remain under user control.

Voice data sent to cloud AI services may be processed externally according to the selected provider's policies.

## 🎯 Project Vision

The vision of Simran AI is to build more than a voice chatbot.

It aims to become a personal AI agent that understands the user's intentions, interacts with the desktop environment, performs useful tasks, and makes everyday digital activities easier through natural communication.

**Talk to Simran. Let your voice control your digital world.**

## 📜 License

This project is intended to be open source. A license will be added when the repository's licensing terms are finalized.

## 👩‍💻 Author

Developed as a personal AI agent project exploring voice technology, AI agents, desktop automation, and intelligent task execution.
