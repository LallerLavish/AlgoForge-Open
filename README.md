# AlgoForge

<p align="center">

[![Python](https://img.shields.io/badge/Python-3.9%2B-blue?logo=python&logoColor=white)](https://www.python.org/)
[![Docker](https://img.shields.io/badge/Docker-Ready-blue?logo=docker&logoColor=white)](https://www.docker.com/)
[![React](https://img.shields.io/badge/React-20232A?logo=react&logoColor=61DAFB)](https://react.dev/)
[![TailwindCSS](https://img.shields.io/badge/TailwindCSS-38B2AC?logo=tailwindcss&logoColor=white)](https://tailwindcss.com/)
[![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?logo=typescript&logoColor=white)](https://www.typescriptlang.org/)
[![FastAPI](https://img.shields.io/badge/FastAPI-009688?logo=fastapi&logoColor=white)](https://fastapi.tiangolo.com/)
[![C++](https://img.shields.io/badge/C++-00599C?logo=cplusplus&logoColor=white)](https://isocpp.org/)
[![Java](https://img.shields.io/badge/Java-007396?logo=java&logoColor=white)](https://www.java.com/)
[![Firebase](https://img.shields.io/badge/Firebase-FFCA28?logo=firebase&logoColor=black)](https://firebase.google.com/)
[![OpenAI GPT-4](https://img.shields.io/badge/OpenAI-GPT--4-412991?logo=openai&logoColor=white)](https://openai.com/)
[![Google Gemini](https://img.shields.io/badge/Google-Gemini-4285F4?logo=google&logoColor=white)](https://deepmind.google/technologies/gemini/)
[![AutoGen](https://img.shields.io/badge/AutoGen-Microsoft-0078D4?logo=microsoft&logoColor=white)](https://microsoft.github.io/autogen/)

</p>

</p>

  <!-- AI Tools -->
  <br/><br/>
  <img src="https://img.shields.io/badge/OpenAI-412991?style=flat-square&logo=openai&logoColor=white" />
  <img src="https://img.shields.io/badge/Gemini-4285F4?style=flat-square&logo=google&logoColor=white" />
  <img src="https://img.shields.io/badge/AutoGen-0078D4?style=flat-square&logo=microsoft&logoColor=white" />
</p>  

---

AlgoForge is an end-to-end platform for *algorithm problem solving, AI-powered code generation, and solution analysis*.  
It combines a modern *React frontend* with a *FastAPI backend*, orchestrated by agentic AI for multi-language code generation, complexity analysis, and Firebase-based user management.  

 *[Watch Demo Video](https://shorturl.at/y2PGS)*  

---

##  Features  

-  *AI-powered code generation* (Python, Java, C++).  
-  *Multi-agent pipeline* for problem extraction, solution generation, and code fitting.  
-  *Automatic time/space complexity analysis* and solution explanation.  
-  *User authentication* via Firebase.  
-  *Problem history tracking* and solution review.  
-  *Modern, responsive UI* with dark mode support.  

---

##  Architecture  

- *Frontend:* React + TypeScript + Tailwind CSS (frontend/)  
- *Backend:* FastAPI + SQLAlchemy + Firebase Admin + Agentic AI (backend/)  
- *AI Pipeline:* Multi-agent orchestration for extraction, solution, and fitting (backend/app/agentic_ai/)  

---

##  Tech Stack  

<p align="center">
  <img src="https://skillicons.dev/icons?i=react,typescript,tailwind,fastapi,python,cpp,java,firebase,sqlite,docker,git" />
</p>  

---

##  Frontend  

- Built with [Create React App](https://github.com/facebook/create-react-app)  
- Styled using [Tailwind CSS](https://tailwindcss.com/) with custom scrollbars  
- Firebase authentication + storage  
- Key files:  
  - src/App.tsx → Main app and routing  
  - src/pages/ProblemResult.tsx → Solution display  
  - src/services/api.ts → API integration  

### Start Frontend  

```sh
cd frontend
npm install
npm start


Runs at [http://localhost:3000](http://localhost:3000).

---

## Backend

- Built with [FastAPI](https://fastapi.tiangolo.com/)
- Uses [SQLAlchemy](https://www.sqlalchemy.org/) for database ORM
- Firebase Admin SDK for user authentication
- Agentic AI pipeline for code extraction, solution, and fitting
- Key files:
  - `app/__init__.py`: FastAPI app, models, routes
  - `app/agentic_ai/final.py`: Pipeline orchestrator
  - `app/agentic_ai/ThreeAgentTeam.py`: Multi-agent solution generator

### Start Backend

```sh
cd backend
python -m uvicorn app.main:app --reload
```

Runs at [http://localhost:8000](http://localhost:8000).

---

## Environment Variables

### Frontend (`frontend/.env`)

```
REACT_APP_FIREBASE_API_KEY=...
REACT_APP_FIREBASE_AUTH_DOMAIN=...
REACT_APP_FIREBASE_PROJECT_ID=...
REACT_APP_FIREBASE_STORAGE_BUCKET=...
REACT_APP_FIREBASE_SENDER_ID=...
REACT_APP_FIREBASE_APP_ID=...
REACT_APP_API_BASE=http://localhost:8000
```

### Backend (`backend/.env`)

```
ALGOFORGE_DB=sqlite:///./algoforge.db
key4=...         # AI model API key
model4=...       # AI model name
# Add other agent keys/models as needed
```

---

## Project Structure

```
AlgoForge/
  frontend/
    src/
      App.tsx
      pages/
        ProblemResult.tsx
      services/
        api.ts
    public/
    tailwind.config.js
    ...
  backend/
    app/
      __init__.py
      main.py
      agentic_ai/
        final.py
        ThreeAgentTeam.py
        ...
    requirements.txt
    Dockerfile
    ...
```

---

## Running the Project

1. **Clone the repository**

   ```sh
   git clone https://github.com/LallerLavish/AlgoForge.git
   cd AlgoForge
   ```

2. **Setup environment variables**  
   Copy `.env.example` to `.env` in both `frontend/` and `backend/` and fill in your credentials.

3. **Install dependencies and start backend**

   ```sh
   cd backend
   pip install -r requirements.txt
   python -m uvicorn app.main:app --reload
   ```

4. **Install dependencies and start frontend**

   ```sh
   cd frontend
   npm install
   npm start
   ```

5. **Access the app**  
   - Frontend: [http://localhost:3000](http://localhost:3000)  
   - Backend API: [http://localhost:8000/docs](http://localhost:8000/docs) (Swagger UI)

---

## Contributing

Pull requests are welcome! For major changes, please open an issue first to discuss what you would like to change.

---


*Crafted with ❤️ by Lavish and Deepak.