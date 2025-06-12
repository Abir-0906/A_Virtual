🧠 AI Voice Assistant (MERN Stack + Gemini + Web Speech API)
A fully functional voice-controlled virtual assistant web application built using the MERN stack (MongoDB, Express, React, Node.js), integrated with Google Gemini API for intelligent response generation and powered by the Web Speech API for real-time speech recognition and speech synthesis.

🔥 Features
🎙️ Voice Commands: Uses SpeechRecognition to listen and SpeechSynthesis to reply.

🧠 Gemini AI Integration: Generates smart JSON responses based on user input.

🔐 Authentication: Secure login/signup system using JWT tokens and HTTP-only cookies.

🧾 User Session Storage: All user commands and assistant replies are stored in MongoDB.

🌐 Smart Intent Recognition:

General queries

Google/Youtube search or playback

Date, time, day, month responses

Opening apps like calculator, Facebook, Instagram

Weather inquiry support

🎨 Modern UI: Built using React and CSS with dynamic UI transitions.

🗃️ Backend: Robust Express server handling routes, authentication, and Gemini integration.

🛠️ Installation
1. Clone the Repository
bash
Copy
Edit
git clone https://github.com/your-username/ai-voice-assistant.git
cd ai-voice-assistant
2. Backend Setup
bash
Copy
Edit
cd server
npm install
# Add .env file
.env example:

env
Copy
Edit
PORT=5000
MONGO_URI=your_mongo_db_uri
JWT_SECRET=your_jwt_secret

GEMINI_API_URL=https://generativelanguage.googleapis.com/v1beta/models/gemini-pro:generateContent?key=your_api_key
bash
Copy
Edit
npm start
3. Frontend Setup
bash
Copy
Edit
cd client
npm install
npm run dev
🎤 Voice Assistant Behavior
✅ Sample Prompts
Command	Assistant Response
"What time is it?"	"type": "get-time"
"Search cats on Google"	"type": "google-search"
"Play Arijit song on YouTube"	"type": "youtube-play"
"Open calculator"	"type": "calculator-open"

🔐 Authentication
JWT tokens are used for session management.

HTTP-only cookies store tokens securely.

Login required to use the assistant.

📦 API Endpoints (Sample)
POST /api/auth/register - Register user

POST /api/auth/login - Login user

POST /api/gemini - Get assistant response

📸 Screenshots
You can add GIFs or images showing assistant listening, responding, and UI screenshots.

💡 Future Improvements
Add support for custom user-defined commands

Mobile PWA version

Language translation using Gemini

📜 License
This project is open-source under the MIT License.

