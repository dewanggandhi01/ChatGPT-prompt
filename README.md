Resume Parser Prompt using ChatGPT

Overview

This project demonstrates how ChatGPT can be used as a Resume Parsing Assistant. The prompt takes a resume as input and extracts relevant information in a structured JSON format. This makes resume data easier to process, store, analyze, and integrate with recruitment or applicant tracking systems (ATS).

---

Objective

The objective of this project is to design an effective prompt that enables ChatGPT to:

- Read resume content.
- Extract important information.
- Convert unstructured resume data into structured JSON.
- Handle missing information gracefully.
- Produce machine-readable output.

---

Prompt

You are a Resume Parsing Assistant.

Task:
Parse the provided resume and return the extracted information in valid JSON format.

Extract the following fields:
- name
- email
- phone
- education
- skills
- projects
- internships
- work_experience
- certifications
- achievements

Rules:
1. Return only valid JSON.
2. Do not include explanations.
3. Use empty arrays for missing fields.
4. Preserve original information whenever possible.
5. Ensure the JSON structure is properly formatted.

Resume:
<PASTE_RESUME_HERE>

---

Sample Resume Input

Example Resume:

Name: Dewang Gandhi

Education:

- B.Tech CSE, ABES Engineering College
- BS Data Science, IIT Madras

Skills:

- Python
- Machine Learning
- FastAPI
- SQL

Projects:

- Data Analyst Agent
- e-Raksha-Setu
- Gandhi Traders Business Analytics

---

Sample JSON Output

{
  "name": "Dewang Gandhi",
  "contact": {
    "phone": "+91-9411654775",
    "email": "dewanggandhi2@gmail.com",
    "linkedin": "dewang-gandhi-21323b331",
    "github": "dewanggandhi01",
    "leetcode": "dewang_gandhi01",
    "portfolio": "Available"
  },
  "education": [
    {
      "degree": "BS in Data Science",
      "institution": "Indian Institute of Technology Madras",
      "mode": "Online",
      "duration": "2023-2027",
      "cgpa": "7.0"
    },
    {
      "degree": "B.Tech in Computer Science and Engineering",
      "institution": "ABES Engineering College",
      "location": "Ghaziabad, Uttar Pradesh",
      "affiliation": "AKTU",
      "duration": "2023-2027",
      "cgpa": "8.5"
    },
    {
      "qualification": "Senior Secondary (Class XII)",
      "board": "CBSE",
      "institution": "Krishna International School",
      "location": "Aligarh, Uttar Pradesh",
      "year": "2022-2023",
      "percentage": "93.8%"
    }
  ],
  "projects": [
    {
      "name": "Data Analyst Agent",
      "year": "2025",
      "technologies": [
        "Python",
        "FastAPI",
        "Seaborn",
        "Matplotlib",
        "Generative AI"
      ],
      "description": [
        "Developed an AI-driven data analysis agent that processes datasets through natural language queries.",
        "Integrated visualization, web scraping, and support for CSV, Excel, JSON, Parquet, and TXT files.",
        "Implemented an end-to-end ML pipeline with API-based workflows."
      ]
    },
    {
      "name": "e-Raksha-Setu",
      "year": "2025",
      "technologies": [
        "AI",
        "Blockchain",
        "Geo-Fencing"
      ],
      "description": [
        "Developed an AI-powered tourist safety system using multiple risk factors.",
        "Implemented geo-fencing and tracking with less than 2-second alert latency.",
        "Built a blockchain-based Digital Identity system with SOS and E-FIR integration."
      ]
    },
    {
      "name": "Gandhi Traders Business Analytics & Inventory Optimization",
      "year": "2024",
      "technologies": [
        "Excel",
        "Data Analysis",
        "Business Intelligence"
      ],
      "description": [
        "Digitized handwritten sales and inventory records into structured datasets.",
        "Analyzed revenue, profit, inventory, and customer insights.",
        "Developed forecasting and inventory optimization models."
      ]
    },
    {
      "name": "DEBO (Real-Time Chat & Utility Platform)",
      "year": "2025",
      "technologies": [
        "Node.js",
        "Express.js",
        "Socket.io",
        "JavaScript",
        "HTML",
        "CSS"
      ],
      "description": [
        "Developed a real-time chat and file-sharing platform.",
        "Implemented QR and link-based file transfer.",
        "Built utilities including PDF creation tools and multiplayer games."
      ]
    }
  ],
  "skills": {
    "core_subjects": [
      "Data Structures and Algorithms",
      "Operating Systems",
      "Object Oriented Programming",
      "DBMS",
      "Computer Networks"
    ],
    "programming_languages": [
      "Python",
      "C++",
      "Java"
    ],
    "machine_learning_ai": [
      "Scikit-learn",
      "XGBoost",
      "Pandas",
      "NumPy",
      "Matplotlib",
      "Seaborn",
      "Model Evaluation"
    ],
    "data_engineering_analytics": [
      "ETL Pipelines",
      "Data Cleaning",
      "Business Analysis",
      "Power BI",
      "Excel"
    ],
    "web_development": [
      "HTML5",
      "CSS3",
      "Bootstrap"
    ],
    "backend_databases": [
      "FastAPI",
      "SQL"
    ],
    "cloud_deployment": [
      "Vercel",
      "Netlify",
      "Render",
      "Railway",
      "GitHub Actions"
    ],
    "tools": [
      "Git",
      "GitHub",
      "Postman",
      "VS Code",
      "Jupyter Notebook",
      "Google Colab",
      "Replit",
      "GitHub Copilot"
    ]
  },
  "achievements_and_certifications": [
    "Finalist, HackHeaven 2.0 - Top 12 out of 200+ teams",
    "NCC C Certificate holder",
    "IIT Madras Foundational Level and Diploma in Data Science",
    "4 Star Problem Solving on HackerRank",
    "C++ Programming (Beginner to Advanced) Certification",
    "Solved 400+ coding problems across multiple platforms",
    "Finalist at Paranox 2.0 Hackathon among 1500+ teams"
  ],
  "work_experience": [],
  "internships": []
}
---

Applications

- Applicant Tracking Systems (ATS)
- Resume Screening
- Recruitment Automation
- HR Analytics
- Candidate Database Management

---

Technologies Used

- ChatGPT
- Prompt Engineering
- JSON
- Natural Language Processing (NLP)

---

Future Improvements

- Support for multiple resume formats (PDF, DOCX, TXT).
- Automatic skill categorization.
- Resume ranking and scoring.
- ATS compatibility checking.
- Integration with recruitment platforms.

---

Author

Dewang Gandhi

B.Tech (Computer Science & Engineering) – ABES Engineering College

BS (Data Science) – IIT Madras
