Mental Health AI Assistant
This is a full-stack web application designed to provide empathetic chatbot support, mood tracking, journaling, and mental health resources. It leverages AI to offer conversational support and analyze mood trends, aiming to be a helpful companion for mental well-being.

Table of Contents
Project Goals

Tech Stack

Core Features

Folder Structure

Setup and Installation

Deployment

Project Goals
Provide empathetic chatbot support for guidance and companionship.

Offer relaxation techniques like meditation, journaling, and breathing exercises.

Track daily mood with an emoji slider or a 1–10 scale.

Display a dashboard with weekly mood analytics, including charts and trends.

Allow users to journal their thoughts with text and optional voice input.

Send reminders for daily mood check-ins.

Suggest mental health helpline resources when severe stress is detected.

Tech Stack
Frontend: React.js, Tailwind CSS, Recharts

Backend: Python, Flask

AI Layer: Google Gemini API, Hugging Face Sentence Transformers (for sentiment analysis)

Database: MongoDB Atlas

Authentication: JWT (JSON Web Tokens)

Core Features
User Authentication: Secure signup and login functionality using JWT.

AI Chatbot: Empathetic and responsive chatbot powered by the Google Gemini API.
-alyses chat messages to detect user sentiment.

Mood Tracking: Daily mood logging with historical data visualization.

Dashboard: Interactive charts displaying weekly mood trends and AI-generated summaries.

Journaling: A private space for users to write down their thoughts.

Crisis Detection: Identifies strong negative sentiment and provides local helpline information.

Folder Structure
mental-health-ai-assistant/
├── backend/
│   ├── app.py
│   ├── auth.py
│   ├── models.py
│   ├── services.py
│   └── requirements.txt
├── frontend/
│   ├── public/
│   ├── src/
│   │   ├── components/
│   │   ├── pages/
│   │   ├── utils/
│   │   ├── App.js
│   │   ├── index.css
│   │   └── index.js
│   ├── package.json
│   └── tailwind.config.js
└── README.md

Setup and Installation
Prerequisites
Node.js and npm

Python 3.8+ and pip

MongoDB Atlas account

Google API Key (for Gemini)

Hugging Face API Token

Backend Setup
Clone the repository:

git clone https://github.com/your-username/mental-health-ai-assistant.git
cd mental-health-ai-assistant/backend

Create a virtual environment:

python -m venv venv
source venv/bin/activate  # On Windows, use `venv\Scripts\activate`

Install dependencies:

pip install -r requirements.txt

Set up environment variables:
Create a .env file in the backend directory and add the following:

MONGO_URI=your_mongodb_atlas_connection_string
JWT_SECRET_KEY=your_jwt_secret_key
GEMINI_API_KEY=your_google_gemini_api_key
HF_TOKEN=your_hugging_face_api_token

Run the Flask server:

flask run

Frontend Setup
Navigate to the frontend directory:

cd ../frontend

Install dependencies:

npm install

Start the React development server:

npm start

The application should now be running on http://localhost:3000.

Deployment
Backend (Flask)
The Flask backend can be deployed to various platforms like AWS EC2, Heroku, or Google App Engine. For AWS EC2, you would typically use a Gunicorn WSGI server and configure Nginx as a reverse proxy.

Frontend (React)
The React frontend can be easily deployed to static hosting services like Netlify, Vercel, or AWS S3.

Build the production-ready code:

npm run build

Deploy the build folder to your chosen platform.
