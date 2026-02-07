# ISL Sign Language Translator 🇮🇳🤟

> A full-fledged product-oriented project to convert **Indian Sign Language (ISL)** into **real-time text** using a camera.

This project is being built step-by-step with a strong focus on:
- Real-time performance
- Clear system structure
- Team collaboration
- Future AI scalability

---

## 🎯 Project Goal

Enable a user to:
1. Open a web application  
2. Turn on the camera  
3. Perform Indian Sign Language  
4. See **live text subtitles** on the screen  

> ⚠️ Current phase uses **dummy AI output**.  
> Real AI models will be integrated in later phases.

---

## 🧠 Project Philosophy

- **Working system > perfect system**
- Build end-to-end first, then improve
- Each part is independent but connected via a fixed contract
- Team members work in isolation but integrate smoothly

---

## 📂 Folder Structure

```
isl-sign-language-translator/
│
├── frontend/ # Camera + UI + subtitles
├── backend/ # API server
├── ai_engine/ # Dummy / future AI logic
├── shared/ # Fixed contract between all parts
├── docs/ # Architecture and notes
└── README.md
```

---

## 👥 Team Roles (IMPORTANT)

Each person works **only in their assigned folder**.

### 🖥️ Frontend
- Camera access
- Live video display
- Subtitle text on screen

### 🧩 Backend
- API (`/predict`)
- Returns text + confidence (dummy for now)

### 🧠 AI Engine
- `predict()` function
- Dummy output for now
- Real model later

### 👑 Leader
- Controls structure
- Ensures contract is followed
- Handles integration

---

## 🔒 Shared Contract (DO NOT CHANGE)

All communication follows this file:

`shared/contract.json`

```json
{
  "request": {
    "frames": "array",
    "timestamp": "number"
  },
  "response": {
    "text": "string",
    "confidence": "number"
  }
}
``` 

>❗ This file is locked.
> Any change must be approved by the project leader.

## 🗓️ Week 1 Objective (MVP)

**By the end of Week 1:**

* Camera should turn on

* Text should appear on screen

* Dummy AI output is acceptable

> 🎉 If this works → Project is officially alive

## 🚧 Current Status

 * Project structure finalized

 * Team roles assigned

 * Frontend camera UI

 * Backend API

 * Dummy AI integration

## 🚀 Future Phases (Preview)

* Real ISL dataset integration

* Word-level sign recognition

* Sentence-level continuous recognition

* Real-time optimization

* Confidence-aware subtitles
