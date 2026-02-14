# Code Samjhao AI – Design Document

## 1. System Overview
Code Samjhao AI is a web-based AI learning assistant that explains code in a simple, beginner-friendly way.  
The system follows a lightweight client–server architecture.

---

## 2. High-Level Architecture

Frontend (HTML/CSS/JS)
        ↓
Backend API (Flask)
        ↓
AI Model (OpenAI / Gemini API)
        ↓
Processed Explanation
        ↓
Frontend Display

---

## 3. System Components

### 3.1 Frontend
- Built using HTML, CSS, and JavaScript
- Provides:
  - Code input editor
  - Language selection dropdown
  - Explanation level selector
  - Output display section

### 3.2 Backend
- Built using Python and Flask
- Responsibilities:
  - Receive user input
  - Construct AI prompts
  - Call AI model API
  - Process and return explanation

### 3.3 AI Layer
- Uses Large Language Models (LLMs)
- Responsibilities:
  - Code understanding
  - Explanation generation
  - Error reasoning
  - Concept extraction

---

## 4. UI Design (Wireframe Description)

### Layout:
- Header: Project name and tagline
- Control bar:
  - Language dropdown
  - Explanation level dropdown
  - Explain button
- Code editor section
- Explanation output section

Design principles:
- Minimal
- Beginner-friendly
- Clean spacing
- Easy readability

---

## 5. Process Flow

1. User pastes code into editor
2. User selects programming language
3. User selects explanation level
4. User clicks "Explain Code"
5. Backend sends structured prompt to AI
6. AI returns explanation
7. Backend processes response
8. Explanation displayed on UI

---

## 6. Prompt Design Strategy
The system dynamically generates prompts based on:
- Selected language
- Selected explanation level
- Beginner-focused teaching tone

Prompt ensures:
- Line-by-line explanation
- Simple language
- Debug-focused guidance (if enabled)

---

## 7. Technology Stack

### Frontend:
- HTML5
- CSS3
- JavaScript

### Backend:
- Python
- Flask

### AI:
- OpenAI API / Gemini API

### Deployment (Prototype):
- Frontend: Vercel / Netlify
- Backend: Render / Railway

---

## 8. Scalability & Future Design
- Modular backend for easy expansion
- Support for additional languages
- Voice and chat-based interfaces
- Integration with LMS platforms
- Mobile and WhatsApp-based access

---

## 9. Design Philosophy
- Learning-first, not answer-first
- AI should be invisible, learning should be visible
- Built for Bharat’s beginner ecosystem
