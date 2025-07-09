# 🧠 COMLEX Question Generator (Prototype)

This is a prototype web application built using FastAPI, OpenAI, PostgreSQL, and HTML that generates COMLEX-style board questions for osteopathic medical students. It supports secure login, real-time question generation, AI-driven feedback, and user progress tracking.

> ⚠️ **Note:** This project is not currently deployed or in production use. It was built as a prototype to demonstrate AI-driven support for medical exam preparation. This project is for **personal, non-commercial, and academic demonstration** only.  
You may not reuse, reproduce, or publish this code or concept without explicit permission from the author.

© 2025 Dana Brooks. All rights reserved.

---

## 🧰 Tech Stack

- **Language**: Python  
- **Framework**: FastAPI  
- **Frontend**: Static HTML  
- **Database**: PostgreSQL  
- **ORM**: SQLAlchemy  
- **Authentication**: OAuth2 & JWT  
- **AI Model**: GPT-4 via OpenAI API  
- **Environment Management**: dotenv  

---

## 🚀 Features

- 🔐 User authentication with secure password hashing  
- 🧪 GPT-4 generated COMLEX-style clinical vignette questions  
- ✅ Auto-evaluation of answers and correctness tracking  
- 💬 AI-generated personalized feedback using metacognitive strategies  
- 📊 Progress tracking including correct/incorrect totals, streaks, and levels  

---

## 🛠️ Installation

```bash

python -m venv env
source env/bin/activate  # On Windows: env\Scripts\activate
pip install -r requirements.txt 


Create a .env file with the following: 
OPENAI_API_KEY=your-openai-key  
DATABASE_URL=your-postgres-connection-url  
SECRET_KEY=your-secret-key  
Start the FastAPI app:


Start the FastAPI app: 
uvicorn main:app --reload
Visit the frontend:
http://localhost:8000
```

# 🧠 How It Works
The user registers and logs in

They select a medical topic (e.g., "Renal Physiology")

The app uses GPT-4 to generate a new COMLEX question

The user submits an answer, and GPT-4 evaluates the response:

✅ If correct: Reinforces learning and clinical application

❌ If incorrect: Provides constructive feedback and improvement strategies

User progress is tracked, including:

Accuracy

Current and longest streaks

Points and leveling system

# 🗂️ File Structure

comlex-question-generator/
├── main.py                # FastAPI backend  
├── static/  
│   └── index.html         # Frontend page  
├── requirements.txt       # Python dependencies  
├── .env                   # Environment variables (not committed)  
├── README.md              # Project documentation  


# 🔐 Security Notes
Passwords are hashed using bcrypt

JWT tokens handle secure user sessions

Environment variables are managed with .env

Keep your OPENAI_API_KEY and SECRET_KEY private


# 📬 About the Creator
# Dana Brooks
👩‍💻 Executive Director of Admissions
✉️ Email: danatallent@yahoo.com
🔗 LinkedIn www.linkedin.com/in/dana-tallent-brooks-a15977a0
