# 🍅 AI-Assisted Pomodoro Timer

A minimalist, responsive Pomodoro timer built with **React** and **Tailwind CSS**. 

> **🎯 Project Goal:** This project serves as a case study in **AI-Native Development**, demonstrating how the **Cursor** IDE can be leveraged to accelerate prototyping, refactoring, and logic implementation while maintaining clean code standards.

App Screenshot<img width="1744" height="870" alt="スクリーンショット 2026-01-16 154352" src="https://github.com/user-attachments/assets/496ecdab-1ebd-45c7-b7d6-9d8ac628ae88" />

*(Live Demo: [https://paulafranquesa.github.io/pomodoro-timer/])*

## 🛠️ Tech Stack & Tools

- **Framework:** React (Vite)
- **Styling:** Tailwind CSS
- **State Management:** React Hooks (useState, useEffect)
- **AI Tooling:** **Cursor (Claude 3.5 Sonnet / GPT-4o)**

## 🤖 The "Cursor" Workflow

This application was built to test the limits of **AI-Pair Programming**. Instead of writing every line manually, I acted as the **Software Architect**, guiding Cursor through specific prompts and context management.

### Key AI Implementations:

#### 1. Context-Aware Scaffolding (`Cmd + K`)
I used Cursor's inline generation to rapidly build the UI components.
* **Prompt used:** *"Create a responsive card component for the timer display using Tailwind CSS. It should have a neumorphic design style and centered text."*

#### 2. Complex Logic Generation (`Composer`)
Handling React's `setInterval` creates common bugs (drifting time, memory leaks). I leveraged Cursor's **Composer** feature to generate a robust custom hook.
* **Challenge:** The timer needed to switch automatically between "Focus" and "Break" modes.
* **Solution:** Used Cursor to write a `useTimer` hook that handles state transitions and audio alerts cleanly.

#### 3. Intelligent Debugging (`@Codebase`)
When encountering a state update issue, I used the `@Codebase` symbol to let the AI analyze the entire file structure.
* **Outcome:** Cursor identified a missing dependency in the `useEffect` array in seconds, explaining *why* it was causing the bug.

## 🧠 Human vs. AI Role

While AI generated ~70% of the syntax, my role focused on:
* **Architecture:** Deciding to separate the timer logic into a custom hook for reusability.
* **Code Review:** Verifying that the AI-generated code followed accessibility standards (ARIA labels).
* **Refinement:** Tweaking the Tailwind configuration to match the specific aesthetic vision that the AI couldn't purely guess.

## 🚀 Features

- [x] Customizable timer durations (Focus, Short Break, Long Break).
- [x] Audio notifications.
- [x] Visual progress bar.
- [x] Fully responsive mobile design.

## 📦 Installation

```bash
# Clone the repository
git clone [URL_DEL_TEU_REPO]

# Install dependencies
npm install

# Run the development server
npm run dev
```
Built with ❤️ and 🤖 by Paula
