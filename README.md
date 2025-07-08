git clone https://github.com/danabr21285/comlex-question-generator.git

cd comlex-question-generator

---



**2. Set up a virtual environment and install dependencies**

python -m venv env

source env/bin/activate   # On Windows: env\Scripts\activate

pip install -r requirements.txt





3. Create a .env file with your own keys and credentials:

ini

Copy

Edit

OPENAI_API_KEY=your-openai-key

DATABASE_URL=your-postgres-connection-url

SECRET_KEY=your-secret-key



4. Start the FastAPI app

bash

Copy

Edit

uvicorn main:app --reload



5. Visit the frontend:

Go to http://localhost:8000 in your browser.



🧠 How It Works

The user registers and logs in.



They select a medical topic (e.g., "Renal Physiology").



The app uses GPT-4 to generate a new COMLEX question in JSON format.



The user submits an answer, and GPT-4 evaluates the response:



✅ If correct: Reinforces learning and clinical application.



❌ If incorrect: Provides constructive feedback and improvement strategies.



User progress is tracked, including:



Accuracy



Current and longest streaks



Points and leveling system



🗂️ File Structure

bash

Copy

Edit

comlex-question-generator/

├── main.py                # FastAPI backend

├── static/

│   └── index.html         # Frontend page

├── requirements.txt       # Python dependencies

├── .env                   # Environment variables (not committed)

├── README.md              # Project documentation

└── images/

    └── screenshot.png     # App screenshot



🔐 Security Notes

Passwords are hashed using bcrypt



JWT tokens handle secure user sessions



Environment variables are managed with .env



Keep your OPENAI_API_KEY and SECRET_KEY private



📬 About the Creator

Dana Brooks

👩‍💻 Executive Director of Admissions

📍 PCOM South Georgia

✉️ Email: danatallent@yahoo.com

🌐 LinkedIn- www.linkedin.com/in/dana-tallent-brooks-a15977a0 



📄 License

This project is for demonstration and personal use only.

Please contact the author for permission to reuse, publish, or deploy this software.
