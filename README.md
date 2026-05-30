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
  "email": "dewanggandhi2@gmail.com",
  "phone": "+91-9411654775",
  "education": [
    {
      "degree": "BS Data Science",
      "institution": "IIT Madras"
    },
    {
      "degree": "B.Tech Computer Science and Engineering",
      "institution": "ABES Engineering College"
    }
  ],
  "skills": [
    "Python",
    "Machine Learning",
    "FastAPI",
    "SQL"
  ],
  "projects": [
    "Data Analyst Agent",
    "e-Raksha-Setu",
    "Gandhi Traders Business Analytics"
  ],
  "internships": [],
  "work_experience": [],
  "certifications": [],
  "achievements": []
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
