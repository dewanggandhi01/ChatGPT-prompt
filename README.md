# Resume Parser using ChatGPT Prompt Engineering

## Assignment

**Task:** Write a ChatGPT prompt that takes a resume as input and parses the content into a structured JSON format.

This project demonstrates how Prompt Engineering can be used with ChatGPT to convert unstructured resume data into machine-readable JSON. The resulting output can be used in Applicant Tracking Systems (ATS), recruitment platforms, candidate databases, and HR analytics workflows.

---

## Problem Statement

Resumes are typically available in unstructured formats such as PDF, DOCX, or plain text. Extracting relevant information manually is time-consuming and difficult to scale.

The objective of this assignment is to design a prompt that enables ChatGPT to:

* Read resume content
* Identify important sections
* Extract relevant information
* Generate structured JSON output
* Handle missing information consistently

---

## Prompt

The following prompt was used to perform resume parsing:

```text
You are a Resume Parsing Assistant.

Task: Parse the provided resume and return the extracted information in valid JSON format.

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
```

---

## Approach

The solution follows a simple workflow:

1. Provide resume content to ChatGPT.
2. Apply the parsing prompt.
3. Extract relevant information from the resume.
4. Organize the extracted information into a structured JSON schema.
5. Return machine-readable output.

This approach eliminates the need for complex rule-based parsers and allows flexible extraction from different resume formats.

---

## Sample Output

The following JSON was generated from the resume used for testing.

```json
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
```

---

## Information Extracted

The parser is capable of extracting:

* Personal Information
* Contact Details
* Educational Qualifications
* Technical Skills
* Projects
* Work Experience
* Internships
* Certifications
* Achievements

---

## Applications

This approach can be applied in:

### Recruitment Systems

* Applicant Tracking Systems (ATS)
* Resume Screening
* Candidate Databases

### Human Resource Analytics

* Candidate Profiling
* Skill Analysis
* Talent Classification

### Automation Workflows

* Resume Processing Pipelines
* Candidate Search Systems
* Data Extraction Solutions

---

## Challenges

Some common challenges in resume parsing include:

* Different resume layouts
* Missing information
* Inconsistent section naming
* Variations in formatting
* Maintaining a consistent JSON structure

These challenges can be reduced through carefully designed prompts and explicit extraction rules.

---

## Future Improvements

Possible enhancements include:

* Direct PDF and DOCX support
* Resume scoring and ranking
* ATS compatibility checking
* Automatic skill categorization
* Candidate-job matching
* Bulk resume processing

---

## Technologies Used

* ChatGPT
* Prompt Engineering
* JSON
* Natural Language Processing Concepts

---

## Learning Outcomes

Through this assignment, the following concepts were explored:

* Prompt Engineering
* Information Extraction
* JSON Schema Design
* Large Language Models
* Structured Data Generation
* AI-Assisted Automation

---

## Author

**Dewang Gandhi**

B.Tech in Computer Science and Engineering
ABES Engineering College

BS in Data Science
Indian Institute of Technology Madras
