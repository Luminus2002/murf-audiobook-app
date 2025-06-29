# 🎧 Murf Audiobook Generator

This is a fullstack application that allows users to **convert any text or script into a high-quality audiobook** using the Murf.ai Text-to-Speech API. It features a responsive frontend built in React and a backend using Node.js, Express, and MongoDB.

---

## 🚀 Features

- 🔊 Convert input text to audio using Murf TTS API
- 📁 Upload `.txt` or paste script manually
- 🎙️ Choose between multiple voices (Natalie, Arjun, Harry, etc.)
- 🌑 Light / Dark mode toggle with modern UI
- 💾 Save audio files locally and optionally store metadata in MongoDB
- 🌐 Fully deployable to platforms like Render, Netlify, or Vercel

---

## 🛠 Tech Stack

| Frontend  | Backend      | External APIs  | Database |
|-----------|--------------|----------------|----------|
| React     | Node.js + Express | Murf.ai TTS API | MongoDB  |
| CSS       | dotenv + multer   |                | Mongoose |

---

## 📁 Project Structure

murf-audiobook-app/
├── backend/ # Express backend
│ ├── routes/ # API routes
│ ├── services/ # Murf API logic
│ ├── database/ # MongoDB connection
│ ├── audio/ # Output .mp3 files
│ └── app.js
├── frontend/ # React UI
│ ├── src/
│ │ ├── App.js
│ │ ├── App.css
│ │ └── components/
│ └── public/
└── README.md

---

## 🌐 Setup Instructions

### 🔧 Backend

1. Navigate to the backend folder:

   ```bash
   cd backend
Install dependencies:

npm install
Create a .env file and add:

PORT=5000
MONGO_URI=mongodb://localhost:27017/murf_audiobook
MURF_API_KEY=your_actual_murf_api_key

Run the server:
npm start
🎨 Frontend
Navigate to the frontend folder:
cd frontend

Install dependencies:
npm install

Start the React app:
npm start

The app will be available at http://localhost:3000

🚀 Deployment
🟣 Backend (Render)
Set Root Directory to backend

Build Command: npm install

Start Command: npm start

Add environment variables manually on Render

🟢 Frontend (Netlify or Vercel)
Root Directory: frontend

Build Command: npm install && npm run build

Publish Directory: build

Set REACT_APP_BACKEND_URL if needed in .env (for live API)

🧠 Future Enhancements
🗣 Voice preview before generation

🧾 Save and list previous generation history

📥 Download button for MP3s

📊 Dashboard analytics (usage stats, user accounts)

🙏 Credits
Murf.ai — for the powerful TTS API

OpenAI — development support

📜 License
This project is licensed under the MIT License.

Let me know if you'd like a shorter version, or one tailored for Netlify/Vercel-only frontend deployment
