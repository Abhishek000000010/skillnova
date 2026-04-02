# 🚀 SkillNova - Intern Management Platform

Welcome to **SkillNova**! This project is a full-stack platform designed to help manage interns, track their courses, and manage user profiles. 

This guide is written in **simple words** so that you (or any new intern) can understand what's going on and how to keep building.

---

## 📂 Project Structure

The project is divided into two main parts:

1.  **`backend/`**: The "brain" of the app. It handles the database, security, and logic. (Built with **Python & FastAPI**)
2.  **`skillnova/`**: The "face" of the app. This is what the user sees and interacts with. (Built with **React & Vite**)

---

## 🧠 Backend (The Brain)

Located in the `backend/` folder.

- **What it does**: Stores user data, authenticates logins, and manages course lists.
- **Key Files**:
  - `app/main.py`: The starting point of the backend.
  - `app/routes/`: Contains different files for different actions (login, courses, user profiles).
  - `app/models/`: Defines how the data should look in the database.
  - `requirements.txt`: List of all Python tools needed.

### How to start the backend:
1.  Open your terminal in the `backend/` folder.
2.  Install tools: `pip install -r requirements.txt`
3.  Fill in your `.env` file (copy `.env.example` if it exists, or check the file for database settings).
4.  Run the server: `uvicorn app.main:app --reload`
5.  **Bonus**: You can see the interactive API docs at `http://127.0.0.1:8000/docs` once it's running!

---

## 🎨 Frontend (The Face)

Located in the `skillnova/` folder.

- **What it does**: Shows beautiful dashboards, login pages, and course lists. It talks to the backend to get data.
- **Key Tools**:
  - **React 19**: The foundation.
  - **Vite**: Makes the development super fast.
  - **Framer Motion**: Makes the animations smooth and "cool."
  - **Lucide React**: For the icons you see on buttons.

### How to start the frontend:
1.  Open your terminal in the `skillnova/` folder.
2.  Install tools: `npm install`
3.  Run the app: `npm run dev`
4.  Open `http://localhost:5173` in your browser.

---

## 🔥 Features We Have So Far

- ✅ **Login/Signup**: Secure authentication.
- ✅ **Course Listing**: A way to see all available courses.
- ✅ **Profile Management**: Users can see and edit their info.
- ✅ **Database Auto-Sync**: The backend automatically sets up database tables when it starts.

---

## 🛠️ Tips for New Interns

- **Adding a new API**: Look at `backend/app/routes/courses.py` for an example of how to make a new endpoint.
- **Adding a new Page**: Look at the `skillnova/src/` folder. Most pages are components.
- **Need help?**: Always check the "Network" tab in your browser's inspect tool (F12) to see if the frontend is talking to the backend correctly.

**Let's keep building something awesome! 🚀**
