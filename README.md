# 🧠 AI-Code-Reviewer

AI-Code-Reviewer is a **multi-language automated code review platform** that combines  
✔️ **Linting** (Python, JavaScript, C/C++)  
✔️ **Complexity analysis**  
✔️ **AI-powered review** (Java, Go, Python)  
✔️ **PDF report generation**  

It is built with a **FastAPI backend** and a **Streamlit frontend**.  
The project can be run locally or deployed on **Render** for cloud access.

---

## 📌 Project Idea

Developers often spend time fixing style issues, handling code smells, and  
checking complexity before a proper review. This tool automates those steps.

👉 You paste/upload your code → The backend runs linters & AI analysis →  
Frontend displays results (lint, complexity, AI suggestions) → You can download  
a **professional PDF review report**.

This makes code reviews **faster, consistent, and AI-assisted**.

---

## ⚙️ Features

- 🔍 **Linting**: Python (`pylint`), JavaScript (`eslint`), C/C++ (`cpplint`)  
- 📊 **Complexity**: Python (`radon`), JS/Go (`gocyclo`), C++ (`lizard`)  
- 🤖 **AI Review**: Uses AI prompts for deeper feedback (Java, Go, Python)  
- 📄 **PDF Reports**: Generates downloadable reports for sharing with teams  
- 🎨 **Modern UI**: Streamlit + custom CSS styling  
- ☁️ **Deployment Ready**: Works on Render (backend + frontend)

---

## 🛠️ Tech Stack

- **Backend**: [FastAPI](https://fastapi.tiangolo.com/), Python, Linting Tools  
- **Frontend**: [Streamlit](https://streamlit.io/), Custom CSS  
- **AI Review**: Integrated with LLM (AI prompts for code analysis)  
- **Complexity**: `radon`, `lizard`, `gocyclo`  
- **Deployment**: [Render](https://render.com/)  

---

## 🚀 How It Works

1. **User Input**  
   - Paste code in textarea OR upload a file (`.py`, `.js`, `.cpp`, `.java`, `.go`).  

2. **Backend Processing**  
   - Chooses appropriate toolset based on language.  
   - Runs linters & complexity analyzers if available.  
   - If AI-only language → sends code to AI reviewer service.  

3. **Results**  
   - Lint warnings (style, unused vars, missing semicolons, etc.)  
   - Cyclomatic complexity & metrics  
   - AI feedback with suggestions  
   - Option to generate/download a **PDF report**  

4. **Frontend**  
   - Streamlit UI displays results in clean sections.  
   - Download button lets user save PDF locally.  

---

## 🖥️ Local Development

### 1. Clone Repository
```bash
git clone https://github.com/Krishna-S-27/AI-Code-Reviewer.git
cd AI-Code-Reviewer
2. Backend Setup
cd backend
python -m venv venv
source venv/bin/activate   # On Windows: venv\Scripts\activate
pip install -r requirements.txt
uvicorn main:app --reload
Backend will run on → http://127.0.0.1:8000

3. Frontend Setup
bash
Copy code
cd ../frontend
pip install -r requirements.txt
streamlit run app.py
Frontend will run on → http://localhost:8501

🌐 Deployment (Render)
Backend
Push project to GitHub.

On Render → Create New Web Service → Connect repo → Select backend/.

Build Command:

pip install -r requirements.txt

Start Command:

uvicorn main:app --host 0.0.0.0 --port 10000
Frontend

Create another Render Web Service → point to frontend/.

Build Command:

pip install -r requirements.txt
Start Command:

streamlit run app.py --server.port 10000 --server.address 0.0.0.0
✅ Now you can open the frontend Render URL → enter backend Render URL in sidebar → Start reviewing code!

## 📸 Screenshots  

### Main UI  
![Main UI](https://github.com/user-attachments/assets/c7c380c4-fd6f-4ed2-8249-b9885a1629f9)

### Example AI Review  
![AI Review 1](https://github.com/user-attachments/assets/8582e736-ae7a-47bb-89ea-9c2aaf1d0b3b)  
![AI Review 2](https://github.com/user-attachments/assets/ee75be8f-a0f7-4f1c-ba15-977fae90e14d)  
![AI Review 3](https://github.com/user-attachments/assets/e20c848b-310b-478d-96f3-1183469a6b83)  
![AI Review 4](https://github.com/user-attachments/assets/ea324270-87f4-40ae-9f98-1648c7aa865a)  
![AI Review 5](https://github.com/user-attachments/assets/e101fe6b-eb1e-437f-bba1-6cbbb143f460)

Credits
Built by Krishna Shalawadi with  using FastAPI, Streamlit, and AI.
[GitHub](https://github.com/Krishna-S-27)
[Linkedin](https://linkedin.com/in/krishnashalawadi)
