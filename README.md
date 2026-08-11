# 🎙️ Local 24/7 Voice AI Assistant

A privacy-focused, local-first voice assistant that runs 24/7 on your machine. It acts as an autonomous productivity partner—tracking your daily to-dos, monitoring your active workflow (VS Code, Terminals, Browsers) with your explicit permissions, conducting morning stand-ups and evening wrap-ups, and managing your personal knowledge base entirely offline.

## 🚀 Key Features

*   **100% Local & Private:** Runs entirely on your hardware. No data leaves your machine.
*   **Proactive Voice Interface:** Real-time Speech-to-Text (STT) and Text-to-Speech (TTS) with wake-word support for natural voice interaction.
*   **Autonomous Workflow Tracking:** Background daemons monitor permitted development environments and browsers to contextually track task completion.
*   **Proactive Routines:** Automatically triggers morning planning, periodic check-ins, and midnight log summaries.
*   **Vector RAG Memory:** Indexes daily logs, habits, and user context locally using vector search for long-term memory.
*   **Background Task Queue:** Asynchronous workers handle indexing, system polling, and routine scheduling without slowing down your machine.

---

## 🛠️ Architecture & Tech Stack

*   **Voice AI:** `faster-whisper` (STT), `Kokoro`/`Piper` (TTS), `Ollama` / Local LLMs (Brain).
*   **Backend & API:** `FastAPI` (Python).
*   **Background Workers:** `Celery` with `Redis`.
*   **Storage:** `SQLite`/`PostgreSQL` (Relational) + Local Vector DB (Semantic/RAG).
*   **System Tracking:** OS-level background hooks (`psutil`, active window monitors).

---

## 🗺️ Project Phases

- [ ] **Phase 1:** Core Infrastructure & Local LLM/Voice Setup
- [ ] **Phase 2:** Database Design, Task Management, & FastAPI Backend
- [ ] **Phase 3:** OS-Level System Tracking & Permissions Daemons
- [ ] **Phase 4:** RAG Implementation & Long-term Memory
- [ ] **Phase 5:** Celery Background Jobs & Proactive Routines (Morning/Evening)
- [ ] **Phase 6:** Lightweight Frontend Admin Dashboard & Integration

---

## ⚙️ Getting Started (Setup Instructions coming soon)

1. Clone the repository.
2. Set up your local Python environment and configure Docker for Redis/PostgreSQL.
3. Install local models via Ollama and configure your speech pipeline.
