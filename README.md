# CodeArena 2.0

A gamified, enterprise-grade coding and web development platform built with **React, Vite, and Monaco Editor**, featuring over 100+ progressive challenges, real-time code optimization grading, AI-assisted theory explanations, UI visual template similarity evaluation, GitHub profile exploration, ATS resume checking, and official Bonafide certificates of completion.

## 🚀 Quick Start

```bash
# 1. Install dependencies
npm install

# 2. Start the Vite development server
npm run dev        # http://localhost:5173

# Optional: Run the Express API Backend
npm run server     # http://localhost:5000
```

Other available scripts:
- `npm run build`: Production bundle build.
- `npm run verify`: Automated verification of all 102 problems across all tiers.
- `npm run preview`: Preview the production build locally.

---

## ✨ Features Overview

### 1. 🔑 REST API Authentication Format
- Speaks standard REST API format (`/api/auth/register`, `/api/auth/login`, `/api/auth/me`, `/api/auth/logout`, `/api/auth/profile`).
- Dual Engine:
  - **In-Browser High-Fidelity Mock REST API**: Complete with realistic network latency, password hashing (PBKDF2-SHA256), and JWT Bearer token generation.
  - **Live Custom Backend Mode**: Set custom API URL (e.g., `http://localhost:5000/api`) directly from the navbar settings modal to connect to a live backend.
  - Standalone **Node.js / Express backend server** provided in `server/server.js`.

### 2. 🏆 100+ Progressive Challenges & 10 Mastery Levels
Organized into 10 distinct levels across 3 mastery tiers:
- **Tier 1: Beginner (Levels 1 - 3)**:
  - Level 1: Web & Programming Fundamentals (Strings, Math, Logic)
  - Level 2: Array Operations & Logic (Transformations, Two Pointers)
  - Level 3: Modern JS, DOM & ES6+ (Debounce, Throttle, Closures, Async, Currying)
  - *Unlocks: Beginner Bonafide Certificate*
- **Tier 2: Intermediate (Levels 4 - 6)**:
  - Level 4: CSS Layouts, Flexbox & Grid (Centering, Responsive Grids, Glassmorphism)
  - Level 5: React Components & State (Reducers, Form controls, Widgets)
  - Level 6: React Hooks & Architecture (Custom Hooks, Virtualization, Theme Sync)
  - *Unlocks: Intermediate Bonafide Certificate & Career Tools*
- **Tier 3: Advanced & Grandmaster (Levels 7 - 10)**:
  - Level 7: Core Algorithmic Optimization (Kadane, Binary Search, Sliding Window)
  - Level 8: Dynamic Programming & Data Structures (Coin Change, Trees, Graphs, LRU)
  - Level 9: Real-World UI Template Similarity Challenges
  - Level 10: Grandmaster Systems (Kanban drag-and-drop, State machines, Token buckets)
  - *Unlocks: Advanced & Grandmaster Bonafide Certificates*

### 3. 🤖 AI Chatbot Tutor (API + Offline Mode)
- Built directly into the problem-solving workspace.
- Capable of:
  - **Theory & Mathematical Explanation**: Deep dive into time/space complexity, intuition, and edge cases.
  - **Socratic Hint System**: Progressive hints without giving away the full answer immediately.
  - **Code Review & Optimization**: Analyzes current editor code for bottlenecks (e.g., nested loops, linear search in loops).
- Works **100% offline** with built-in problem knowledge, or connect your **Google Gemini API Key** or **OpenAI API Key** in settings for live generative responses.

### 4. ⚡ Dynamic Code Optimization & Marks Engine
- Automatically grades submissions on a **0 - 100 marks scale**:
  - **Correctness & Accuracy (40 marks)**
  - **Runtime Execution Speed (25 marks)**
  - **Space & Memory Optimization (20 marks)**
  - **Code Quality & Cleanliness (15 marks)**
- Assigns grades: **S Tier** (95-100), **A+ Tier** (90-94), **A Tier** (80-89), **B Tier** (65-79), **C Tier** (50-64).
- Automatic Big-O time and space complexity estimation (e.g. $O(N)$ vs $O(N^2)$).

### 5. 🎆 Tiered Celebration with Confetti & Fanfare
- Dynamic celebration screen triggered on level completion according to earned marks:
  - **S/A+ Tier (90-100 marks)**: Triple multi-cannon confetti explosion, golden trophy, 3 stars, and majestic ascending fanfare.
  - **A Tier (75-89 marks)**: Sparkle confetti shower and upbeat cheerful chime.
  - **B Tier (50-74 marks)**: Friendly completion chime and particle burst.
- Synthesized audio fanfare using the **Web Audio API** (zero external MP3 dependencies).

### 6. 🎨 Web Development UI Similarity Challenge Arena
- Supports **HTML**, **CSS**, **JavaScript**, and **React (JSX)**.
- Each challenge displays a target visual template mockup (e.g., Modern SaaS Pricing Table, Glassmorphism Profile Card, Responsive Navbar).
- Real-time sandboxed live preview iframe.
- Automated Visual & Structural Similarity Evaluator calculating a **0 - 100% match score** (DOM structure, CSS styling, responsive layout, interactivity).

### 7. 🐙 GitHub Developer Explorer with Likes
- Search any developer on GitHub (e.g., `torvalds`, `gaearon`, `yyx990803`).
- Fetches real live public data: avatar, bio, follower metrics, location, and top starred repositories.
- **Like Profile Button** with heart animation and persistent "Liked Developers" gallery.

### 8. 📄 Career Tools: ATS Resume & Portfolio Checker
- Unlocked after reaching milestone levels.
- **ATS Resume Checker**: Analyzes resume text against technical recruiter ATS algorithms, evaluates keyword density (React, TypeScript, Redux, Git), action verbs, and quantifiable metrics.
- **Portfolio Health Checker**: Evaluates live demos, repository cleanliness, mobile responsiveness, and custom domain presence.

### 9. 📜 Official Bonafide Certificates of Completion
- Verifiable, high-prestige Bonafide Certificates for:
  - *Beginner Web & Code Developer*
  - *Intermediate Frontend & React Specialist*
  - *Advanced Full-Stack & Systems Engineer*
  - *Grandmaster CodeArena Champion*
- Includes Credential ID, student name, conferment date, average optimization grade, verified skills, security guilloche watermark, and official seal.
- Built-in `@media print` formatting for 1-click **Print to PDF** export!
