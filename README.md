# 📧 SmartMail-AI – AI-Powered Email Reply Assistant

SmartMail-AI is a full-stack project that generates **AI-powered email replies** with a professional, casual, or friendly tone.  
It consists of three parts:
1. **React Frontend** – User interface for drafting and generating replies.  
2. **Spring Boot Backend** – Connects with Gemini AI API to generate responses.  
3. **Chrome Extension** – Directly integrates into Gmail with an **AI Reply** button.  

---

## ✨ Features
- 📝 Generate context-aware replies for any email.  
- 🎭 Choose a reply **tone** (Professional, Casual, Friendly).  
- 📋 Copy replies easily with one click.  
- ⚡ Gmail integration via Chrome Extension.  
- 🔗 Backend powered by **Spring Boot** and **Gemini API**.  

---

## 🛠️ Tech Stack
**Frontend (React):**
- React + Vite  
- Material UI (MUI)  
- Axios  

**Backend (Spring Boot):**
- Spring Boot (REST API)  
- WebClient for API calls  
- Lombok + JSON Processing  

**Chrome Extension:**
- Manifest V3  
- Content Scripts (Gmail toolbar injection)  
- Fetch API  

---

## 🚀 Getting Started

### 1. Clone the Repository
```bash
git clone https://github.com/Bhaskar692/SmartMail-AI.git
cd SmartMail-AI
# SmartMail-AI
```
### 2. Backend Setup (Spring Boot)
cd email-writer-sb
- mvn clean install
- mvn spring-boot:run
- By default, the backend runs on:
- http://localhost:7076/api/email/generate

Set the following in application.properties:
```
gemini.api.url=https://generativelanguage.googleapis.com/v1beta/models/gemini-pro:generateContent?key=
gemini.api.key=YOUR_API_KEY
server.port=7076
```
### 3. Frontend Setup (React)
```bash
cd email-writer-react
npm install
npm run dev
```
Runs locally at:
http://localhost:5173

### 4. Chrome Extension Setup
  Open Chrome → chrome://extensions/.

  Enable Developer Mode.

  Click Load unpacked.

  Select the email-writer-ext folder.

  Open Gmail → You’ll see a new AI Reply button in the compose window.

  📸 Screenshots
  
  <img width="1522" height="946" alt="image" src="https://github.com/user-attachments/assets/b917ba97-660e-4ff0-9c61-dc0446aa1895" />
  
  Chrome Extension
  
  <img width="1162" height="487" alt="image" src="https://github.com/user-attachments/assets/4731a3e5-188a-4bcc-b539-a57c46e4df45" />

  <img width="1112" height="645" alt="image" src="https://github.com/user-attachments/assets/86b2694e-33c5-43f3-8c14-92456b1a900f" />


###⚡ API Endpoint
  -  POST /api/email/generate

   Request Body:
   ```
   json
    {
  "emailContent": "Hi, can we reschedule our meeting to tomorrow?",
  "tone": "professional"
}
```
### 
   Response:
   ```
    json
    "Sure, I’d be happy to reschedule our meeting for tomorrow. Please let me know a time that works best for you."
```
### 📂 Project Structure
```
SmartMail-AI/
├── email-writer-react/     # React frontend
├── email-writer-sb/        # Spring Boot backend
├── email-writer-ext/       # Chrome extension
└── README.md               # Project documentation
```
👨‍💻 Author

Bhaskar
🔗 GitHub(https://github.com/Bhaskar692) | LinkedIn( linkedin.com/in/karamala-bhaskar)

📜 License

MIT License – feel free to use, modify, and share.
```

---

Would you like me to also make this **resume/portfolio friendly** (with a "Highlights" section like *Built full-stack AI-powered Gmail extension using React, Spring Boot, and Gemini API*) so you can directly use it in your CV?
```
