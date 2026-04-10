# 📞 VoiceAgent-AI

An AI-powered voice agent built using **Python**, **Twilio**, and **Gemini API** that can handle voice calls, process user speech, and respond intelligently using AI.

This project demonstrates how to integrate telephony services with modern AI models to create automated voice assistants.

---
<img width="1132" height="758" alt="Screenshot 2026-04-10 at 6 42 31 AM" src="https://github.com/user-attachments/assets/8608a913-9e7b-4abd-a3cd-dd1d9ca7d5d0" />












## 🚀 Features

* 📞 Receive and handle incoming phone calls
* 🎙 Convert speech to text
* 🤖 Process user input using Gemini AI
* 🔊 Generate intelligent voice responses
* ☁️ Built using Twilio Voice API
* 🐍 Python-based backend
* ⚡ Real-time voice interaction

---

## 🧠 Tech Stack

* Python
* Twilio Voice API
* Gemini API
* Flask / FastAPI
* Ngrok

---

## 📁 Project Structure

```
VoiceAgent-AI/
│
├── main.py            # Entry point of the voice agent
├── requirements.txt   # Project dependencies
├── .gitignore         # Ignored files
├── .venv/             # Virtual environment
└── README.md          # Project documentation
```

---

## ⚙️ Installation

### 1. Clone the repository

```bash
git clone https://github.com/Adityatomar28/VoiceAgent-AI.git
cd VoiceAgent-AI
```

### 2. Create virtual environment

```bash
python -m venv venv
```

Activate environment:

Mac / Linux:

```bash
source venv/bin/activate
```

Windows:

```bash
venv\Scripts\activate
```

---

### 3. Install dependencies

```bash
pip install -r requirements.txt
```

---

## 🔑 Environment Variables

Create a `.env` file in the root directory:

```
TWILIO_ACCOUNT_SID=your_account_sid
TWILIO_AUTH_TOKEN=your_auth_token
TWILIO_PHONE_NUMBER=your_twilio_number

GEMINI_API_KEY=your_gemini_api_key
```

---

## ▶️ Run the Project

```bash
python main.py
```

---

## 🌐 Expose Local Server using Ngrok

```bash
ngrok http 5000
```

Copy the generated URL and paste it into:

```
Twilio Console → Phone Number → Webhook URL
```

---

## 🔄 How It Works (Flow)

```
User calls Twilio number
        ↓
Twilio sends webhook request
        ↓
Python server receives request
        ↓
Speech converted to text
        ↓
Text sent to Gemini AI
        ↓
AI generates response
        ↓
Response converted to voice
        ↓
Voice sent back to caller
```

---

## 🧪 Example Use Cases

* Customer support automation
* AI receptionist
* Voice-based chatbot
* Appointment booking assistant
* Call automation system

---

## 📦 Requirements

Typical dependencies:

```
flask
twilio
python-dotenv
google-generativeai
```

---

## 🔒 Security Notes

Never commit:

```
.env
API keys
Auth tokens
Secrets
```

Make sure `.gitignore` includes:

```
.env
venv/
__pycache__/
```

---

## 🧑‍💻 Author

**Aditya Singh Tomar**
AI & Backend Developer
B.Tech Artificial Intelligence

GitHub:
https://github.com/Adityatomar28

---

## 🚧 Future Improvements

* Add conversation memory
* Add database logging
* Multi-language support
* Deploy on AWS / Render
* Add Docker support
* Real-time streaming responses

---

## ⭐ Project Status

**Active Development**
