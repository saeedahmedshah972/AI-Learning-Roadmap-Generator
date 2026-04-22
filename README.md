# 📚 AI Learning Roadmap Generator (Gradio + Colab)

## 📌 Project Overview

The **AI Learning Roadmap Generator** is an AI-powered application built in Google Colab that generates personalized learning roadmaps based on user input. It uses the Groq API (LLM) to create structured learning paths from beginner to advanced level.

The project also provides a **Gradio-based user interface** for easy interaction and allows users to **download the generated roadmap as a PDF file**.

---

## 🚀 Features

* 🤖 AI-generated learning roadmaps using Groq API
* 📊 Structured step-by-step learning paths
* 🌐 Simple Gradio web interface
* 📥 Download roadmap as PDF
* ⚡ Fast response using LLM
* 🧠 Supports any skill/topic input

---

## 🧠 How It Works

1. User enters a skill or topic (e.g., AI, Python, Machine Learning)
2. Groq LLM processes the input
3. AI generates a structured roadmap
4. Output is displayed in Gradio UI
5. User can download roadmap as PDF

---

## 🛠️ Technologies Used

* Python 🐍
* Google Colab 📒
* Gradio 🌐
* Groq API 🤖
* ReportLab / PDF Generator 📄
* dotenv (for API key security)

---

## 📂 How to Run (Google Colab)

### 1. Open notebook in Google Colab

Run all cells step by step.

---

### 2. Install dependencies

```python id="colab_install"
!pip install gradio groq reportlab python-dotenv
```

---

### 3. Set API Key securely

```python id="colab_api"
import os

os.environ["GROQ_API_KEY"] = "YOUR_API_KEY"
```

---

### 4. Run Gradio App

```python id="colab_run"
import gradio as gr

def generate_roadmap(topic):
    # AI logic here (Groq API call)
    return "Generated roadmap for " + topic

interface = gr.Interface(
    fn=generate_roadmap,
    inputs="text",
    outputs="text",
    title="AI Learning Roadmap Generator"
)

interface.launch()
```

---

## 📥 PDF Download Feature

The project also allows users to download generated roadmaps as PDF files for offline use.

---

## 🎯 Example Use Cases

* Learn Python step-by-step
* Create AI/ML roadmap
* Plan Web Development learning path
* Prepare structured study plan

---

## 🔐 API Key Security

Always keep your Groq API key hidden and never upload it to GitHub.

---

## 📸 UI Preview

(Add Gradio screenshot here)

```md id="ui1"
![Gradio UI](assets/dashboard.png)
```

---

## 🚀 Future Improvements

* Add user history storage
* Improve roadmap personalization
* Add downloadable PDF templates
* Deploy as public web app

---

## 👨‍💻 Author

Muhammad Saeed Ahmed
BS Computer Science | AI Developer

---

## ⭐ Support

If you like this project, please give it a ⭐ on GitHub.
