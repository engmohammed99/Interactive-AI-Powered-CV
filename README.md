# 📝 Interactive AI-Powered CV  

An **AI-powered interactive CV** that lets users **chat with my résumé**, ask questions about my skills and experience, and automatically records user details or unanswered questions for follow-up.  

Built using **OpenAI**, **Gradio**, and **Pushover** to create a dynamic, conversational experience for visitors.  

---

## 🚀 Overview  

This project transforms a static résumé into an **interactive experience**.  
Visitors can:  
- 🗨️ **Ask questions** about my background, skills, and experience  
- 📩 **Provide contact information**, which is automatically recorded  
- 📝 **Log unanswered questions** for later review  

The system uses the OpenAI API to handle natural language queries, plus PDF/LinkedIn data for accurate answers.  

---

## 🗂️ Project Structure  

- `me/linkedin.pdf` – My LinkedIn profile content, extracted for context  
- `me/summary.txt` – A short summary of my background  
- `app.py` – Main Python app with Gradio UI  
- `record_user_details` – Tool to record email/name of visitors  
- `record_unknown_question` – Tool to log unanswered questions  

---

## ⚙️ Tech Stack  

- **Python 3.10+**  
- **OpenAI API** for natural language processing  
- **Gradio** for the web-based chat interface  
- **PyPDF** for extracting text from PDFs  
- **Pushover** for push notifications of leads and questions  

---

## 🏗️ How It Works  

1. **System Prompt** loads my résumé summary and LinkedIn profile.  
2. Users interact through a **Gradio ChatInterface**.  
3. The system calls functions to either:  
   - Record user details (email, name, notes)  
   - Record unanswered questions  
4. Everything is **logged** and sent to me instantly via Pushover.  

---

## 📦 Installation  

Clone the repo:  
```bash
git clone https://github.com/yourusername/interactive-cv.git
cd interactive-cv
