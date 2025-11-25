# 🌌 NovaKB — Intelligent AI Workspace  

NovaKB is a **modern AI-powered workspace** designed for intelligent document interaction. It provides a **beautiful chat interface**, **real-time AI assistance**, and **knowledge base management** in a single lightweight web app.

---

## 🚀 Features  

### 💬 Smart AI Chat  
- Chat with an AI assistant using a real-time streaming interface.  
- Dynamic message rendering with Markdown and sanitization.  
- Typing indicators for a natural conversation flow.  

### 📁 Knowledge Base Integration  
- Upload `.pdf`, `.docx`, `.txt`, `.md`, or `.xlsx` files.  
- Automatically connects to your backend AI for knowledge ingestion.  
- Manage or clear stored knowledge base data in one click.  

### 🌓 Light & Dark Modes  
- Sleek glassmorphic design with TailwindCSS.  
- Smooth transitions between *Dark Mode* and *Pure White Light Mode*.  
- Consistent visual clarity for all themes.  

### 📤 Export Chat  
- Export entire conversations as **beautiful PDFs** using `html2canvas` and `jsPDF`.  
- Includes stylish flash animation for a polished user experience.  

### ⚙️ System Controls  
- Minimize, maximize, and close window animations (macOS-style).  
- Reopen app and dock behavior for seamless multitasking.  
- Real-time system uptime display.  

---

## 🧠 Architecture Overview  

**Frontend Technologies**
- `HTML5` + `TailwindCSS` for responsive, modern UI.  
- `JavaScript (ES6+)` for interactivity and API communication.  
- `Font Awesome` for icons and UI enhancement.  
- `Google Fonts (Inter & JetBrains Mono)` for clean typography.  

**Libraries Used**
| Library | Purpose |
|----------|----------|
| `marked.js` | Markdown rendering for chat messages |
| `DOMPurify` | Prevents XSS attacks in message rendering |
| `html2canvas` | Captures chat DOM for export |
| `jsPDF` | Converts chat screenshots to PDF |
| `TailwindCSS` | Styling and layout |
| `Font Awesome` | Icon library |

**Backend Requirements**
- A running API server accessible at `http://192.168.7.90:8000`  
  with endpoints:
  - `/chat` — Chat with AI model  
  - `/upload` — Upload documents  
  - `/clear_kb` — Reset knowledge base  

---

## 🧩 Project Structure  

NovaKB/
│
├── index.html # Main web app
├── /assets # (optional) Fonts, images, icons
└── README.md # You’re reading it!

yaml
Copy code

---

## ⚡ How It Works  

1. **Launch the app** — Open `index.html` in your browser.  
2. **Upload files** — Click *Upload Docs* to send files to your AI backend.  
3. **Chat intelligently** — Ask questions, summarize documents, or write code.  
4. **Switch modes** — Toggle between dark and light themes anytime.  
5. **Export** — Save the conversation as a PDF report.  

---

## 🖼️ Screenshots  

| Dark Mode | Light Mode |
|------------|------------|
| ![Dark Mode UI](https://via.placeholder.com/400x250?text=NovaKB+Dark) | ![Light Mode UI](https://via.placeholder.com/400x250?text=NovaKB+Light) |

---

## 🧑‍💻 Local Development  

### 1️⃣ Clone the Repository  
```bash
git clone https://github.com/yourusername/NovaKB.git
cd NovaKB
2️⃣ Serve Locally
Use any live server (VS Code extension or Python):

bash
Copy code
python3 -m http.server 8000
Then open http://localhost:8000 in your browser.

3️⃣ Configure Backend
Update the API_URL constant in the <script> section of index.html:

js
Copy code
const API_URL = 'http://your-server-ip:8000/chat';
🎨 Design Philosophy
NovaKB is built with three key goals in mind:

Beauty — Elegant glassmorphic design inspired by macOS aesthetics.

Simplicity — Minimal code footprint, easily extendable.

Performance — Optimized DOM handling and smooth animations.

📚 Future Enhancements
 User authentication

 Multi-document summarization

 Real-time collaborative editing

 Integration with cloud-based AI APIs (e.g., OpenAI, Anthropic)

💖 Credits
Frontend Design: TailwindCSS + Inter Font

Libraries: Marked.js, DOMPurify, jsPDF, html2canvas

Developer: [Your Name or Team]

License: MIT
