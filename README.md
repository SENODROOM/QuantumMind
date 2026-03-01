# AnonymousThinker 🧠

AnonymousThinker is a premium AI reasoning platform designed to provide structured, logical responses with a specialized focus on defending and explaining Islamic principles through reason and scholarly knowledge.

## ✨ Key Features

- **Dual-Model Comparative Analysis**: Compare responses from a personal logic model (Llama 3.1 8B) and a powerful reasoning model (DeepSeek-R1-70B) side-by-side.
- **Sovereign AI Hub**: A centralized command center for administrators to define the AI's persona, logical framework, and core strategy.
- **Knowledge Base (RAG)**: Ground AI responses in scholarly Islamic knowledge by uploading PDFs and text files globally.
- **Admin-Restricted Training**: Only authorized developers can train the AI or modify its core directives.
- **Glassmorphic UI**: A premium, modern interface with dark mode, fluid animations, and a focus on readability.

---

## 🛠️ Tech Stack

- **Frontend**: React.js, React Router, Axios, Vanilla CSS (Standardized Design System).
- **Backend**: Node.js, Express, MongoDB (Mongoose), JWT Auth.
- **AI Infrastructure**:
  - **Inference**: Groq API & Hugging Face Serverless Inference.
  - **Reasoning Models**: Llama-3.1-8B-Instruct & Llama-3.3-70B-Versatile.
  - **Logic Engine**: Custom NLP pipeline for PDF parsing and RAG (Retrieval Augmented Generation).

---

## 🚀 Local Setup Guide

Follow these steps to get the project running on your local machine.

### 1. Prerequisites
- **Node.js** (v18+)
- **npm** or **yarn**
- **MongoDB** (Local instance or Atlas URI)

### 2. Clone the Repository
```bash
git clone <repository-url>
cd AnonymousThinker
```

### 3. Backend Setup
1. Navigate to the backend directory:
   ```bash
   cd backend
   ```
2. Install dependencies:
   ```bash
   npm install
   ```
3. Configure Environment Variables:
   - Copy `.env.example` to `.env`:
     ```bash
     cp .env.example .env
     ```
   - Open `.env` and add your `MONGODB_URI`, `JWT_SECRET`, `GROQ_API_KEY`, and `HUGGINGFACE_API_KEY`.

4. Start the server (Development mode):
   ```bash
   npm run dev
   ```

### 4. Frontend Setup
1. Navigate to the frontend directory:
   ```bash
   cd ../frontend
   ```
2. Install dependencies:
   ```bash
   npm install
   ```
3. Start the application:
   ```bash
   npm start
   ```

---

## 🛡️ Administrative Configuration

### Promoting Your Account to Admin
To access the "Train AI" command center, you must promote your account.

1. Register an account through the UI.
2. In the `backend/scripts` folder, run:
   ```bash
   node makeAdmin.js your-email@example.com
   ```
   *Note: Ensure your backend server is stopped or you have configured `.env` correctly for the script.*

### Default Admin Login
If you configured `ADMIN_EMAIL` and `ADMIN_PASSWORD` in your `.env`, you can login directly with those credentials to auto-promote your session.

---

## 📚 Global Knowledge Training

To ensure the AI prioritizes Islamic logical proofs:
1. Login as an Admin.
2. Click **"Train AI"** in the sidebar.
3. Use the **Upload Zone** to ingest PDFs of scholarly Islamic works.
4. Update the **"Core Logic & Strategy"** textarea to define how the AI should refute specific claims.
5. Click **"Commit Changes to Core"** to synchronize the AI's logic globally.

---

## 📜 License
MIT License - Developed for Sovereign Thought Analysis.
