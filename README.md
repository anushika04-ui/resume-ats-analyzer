# Resume ATS Analyzer

A beginner-friendly full-stack project that analyzes resume text (or a PDF resume) and optionally compares it with a Job Description to show:
- ATS-style score
- Resume level (Fresher / Entry-Level)
- Matched & missing keywords (based on JD)

## Features
- Paste resume text and get an ATS score
- Paste job description for keyword matching
- Upload a resume PDF (extracts text and fills the resume textbox)
- Clean UI with one-click Analyze & Clear
- Works without MongoDB (no database required)

## Tech Stack
- Frontend: React, Axios
- Backend: Node.js, Express
- PDF Text Extraction: Multer + pdf-parse

## Project Structure
resume-ats-analyzer/
│
├── ats-frontend/                 # React Frontend
│   ├── public/
│   ├── src/
│   │   ├── App.js                # Main UI & API integration
│   │   ├── App.css               # Styling
│   │   └── index.js
│   ├── package.json
│   └── package-lock.json
│
├── server/                       # Node.js Backend
│   ├── server.js                 # Express server setup
│   ├── analyze.js                # ATS scoring logic
│   ├── upload.js                 # PDF upload & extraction
│   ├── uploads/                  # Temporary PDF storage
│   ├── package.json
│   └── package-lock.json
│
├── .gitignore
└── README.md

## Live Demo
Frontend: https://resume-ats-analyzer-anushika.vercel.app
Backend: https://ai-resume-ats-analyzer-2yrs.onrender.com

