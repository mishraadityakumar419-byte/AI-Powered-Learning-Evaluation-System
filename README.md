Here’s a **single, clean, professional `README.md`** combining both your projects (Agentic AI Learning App + DSA Audio Logic Agents). It’s structured for **GitHub + recruiters + ATS** 👇

---

# 🚀 Agentic AI Learning & Evaluation System (Groq Powered)

This repository contains two AI-powered learning systems built using **Agentic AI workflows, Groq LLM, and Streamlit**:

* 🎥 **Agentic AI Learning App (Video-Based Evaluation)**
* 🎙️ **DSA Audio Logic Agents System**

Both systems focus on **automated learning evaluation, feedback generation, and personalized improvement** using AI.

---

# 📌 1. Agentic AI Learning App (Video Evaluation)

## 🔍 Overview

An AI-powered system that evaluates **student-recorded video answers** using:

* Speech-to-Text
* NLP-based semantic similarity
* AI-generated feedback

Built with a **multi-agent pipeline** powered by **Groq LLM**.

---

## ⚙️ Key Features

✔ Topic generation using Groq
✔ Live video recording (browser-based)
✔ Automatic video storage in database
✔ Speech-to-Text processing
✔ Word count + speaking speed (WPM) validation
✔ Accuracy evaluation (semantic similarity)
✔ AI-generated improvement suggestions
✔ Learning path recommendation

---

## 🔄 Workflow

```text
Field + Subject + Level
  → Topic Agent (Groq)
  → Live Video Recording (streamlit-webrtc)
  → Save Video in Database
  → Speech-to-Text (Whisper/Groq)
  → Word Count + WPM Validation
  → Accuracy Analysis

  → If Accuracy < 60%
        → Re-record / Re-upload Prompt

  → If Accuracy ≥ 60%
        → Improvement Suggestions
        → Corrected Answer
        → Learning Path
```

---

## 📊 Evaluation Logic

* **WPM Range Check** → Ensures natural speaking speed
* **Word Count Validation** → Avoids too short/long answers
* **Accuracy Threshold** →

  * `< 60%` → Reattempt required
  * `≥ 60%` → Feedback + improvement

---

## 🛠️ Tech Stack

* **Frontend/UI:** Streamlit
* **Live Recording:** streamlit-webrtc
* **LLM:** Groq API
* **Speech-to-Text:** Whisper
* **Embeddings:** SentenceTransformers
* **Database:** SQLite
* **Audio/Video Processing:** FFmpeg

---

## 📌 Notes

* Works best with **Python 3.11 / 3.12**
* Browser will request **camera + microphone access**
* No history page (optimized lightweight version)
* Optional knowledge context: `knowledge/101_reference.txt`

---

# 📌 2. DSA Audio Logic Agents System

## 🔍 Overview

An AI system that evaluates **spoken DSA solutions** and analyzes:

* Correctness of approach
* Edge cases
* Failure conditions
* Concept clarity

---

## ⚙️ Key Features

✔ AI-generated DSA questions (Groq)
✔ Audio answer recording (Streamlit)
✔ Speech-to-Text transcript generation
✔ Logic validation against stored question
✔ Edge case detection
✔ Failure condition analysis
✔ AI-generated explanation notes

---

## 🔄 Workflow

```text
Generate DSA Question (Groq)
   → Save Question (SQLite)
   → Record Audio Answer (st.audio_input)
   → Save Audio
   → Convert Speech to Text
   → Display Transcript
   → Analyze Logic vs Question
   → Identify:
        - Where solution works
        - Where it fails
   → Generate Learning Notes
```

---

## 🛠️ Tech Stack

* **Frontend/UI:** Streamlit
* **LLM:** Groq API
* **Speech-to-Text:** Whisper
* **Database:** SQLite
* **Audio Processing:** FFmpeg

---


## 📌 Notes

* Install **FFmpeg** (required for Whisper)
* Record audio **only after generating the question**
* Transcript appears automatically after recording

---

# 🧠 Core Concept: Agentic AI

Both systems follow an **Agent-based architecture**, where each step is handled by a specialized AI agent:

### 🤖 Agents Used

* Topic Generator Agent
* Speech-to-Text Agent
* Validation Agent (WPM + Word Count)
* Similarity/Accuracy Agent
* Feedback Agent
* Learning Path Agent

---

# 📊 Use Cases

* AI-based student evaluation systems
* EdTech platforms
* Interview preparation tools
* DSA practice assistants
* Personalized learning systems

---

# 🎯 Impact

✔ Automates evaluation of spoken/video answers
✔ Reduces manual grading effort
✔ Provides real-time personalized feedback
✔ Improves conceptual clarity and communication skills


