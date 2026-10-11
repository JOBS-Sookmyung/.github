
<!-- Header -->
<img src="https://capsule-render.vercel.app/api?type=blur&color=gradient&height=300&section=header&text=Jobis&fontSize=80" />

# 👀 Jobis
An AI-powered **personalized interview preparation platform**.

Jobis generates tailored interview questions based on users' resumes and job posting URLs. It helps users prepare effectively for job interviews by providing real-time feedback and recommending relevant learning videos.

---

## 🍎 Introduction
![1](https://github.com/user-attachments/assets/67379bb3-8184-472c-9a80-1787732c4445)

Jobis aims to go beyond traditional recruitment and resume management services by offering a **personalized AI-powered interview preparation experience**.

Based on each user's resume and target job position, Jobis generates customized interview questions and provides actionable feedback. It also recommends relevant video resources to help users improve areas where they need additional preparation.

**Key Features**
- 📝 **Personalized Interview Question Generation** (LLM + RAG)
- 💬 **Real-time Feedback and Improvement Suggestions**
- 🎥 **Resume-based Video Recommendations**
- 📊 **Interview Feedback History Management**

---

## 🍎 Team
![9](https://github.com/user-attachments/assets/ada8b4f0-507d-410d-9b0f-41d3db558373)

---

## 🍎 Background
![4](https://github.com/user-attachments/assets/f3b25bd3-3504-46da-9ffd-f5a27ad24dae)

### Limitations of Existing Services
1. Primarily focused on **recruitment rather than interview preparation**
2. Reliance on **standardized interview questions**, resulting in limited diversity and relevance
3. **Limited personalization** based on individual qualifications and job requirements
4. **Lack of real-time feedback** to support continuous improvement

➡️ Jobis addresses these limitations by providing a differentiated interview preparation solution focused on **personalization and actionable feedback**.

---

## 🍎 Tech Stack

<h4>Frontend</h4>
<div>
  <img src="https://img.shields.io/badge/react-20232a.svg?style=for-the-badge&logo=react&logoColor=61DAFB" />&nbsp
  <img src="https://img.shields.io/badge/javascript-F7DF1E.svg?style=for-the-badge&logo=javascript&logoColor=20232a" />&nbsp
  <img src="https://img.shields.io/badge/html5-E34F26.svg?style=for-the-badge&logo=html5&logoColor=white" />&nbsp
  <img src="https://img.shields.io/badge/styled--components-DB7093?style=for-the-badge&logo=styled-components&logoColor=ffd35b" />&nbsp
  <img src="https://img.shields.io/badge/tailwindcss-1daabb.svg?style=for-the-badge&logo=tailwind-css&logoColor=white" />&nbsp
  <img src="https://img.shields.io/badge/css3-1572B6.svg?style=for-the-badge&logo=css3&logoColor=white" />&nbsp
</div>

<h4>Backend</h4>
<div>
  <img src="https://img.shields.io/badge/Fastapi-009688.svg?style=for-the-badge&logo=Fastapi&logoColor=white" />&nbsp
  <img src="https://img.shields.io/badge/mysql-4479A1.svg?style=for-the-badge&logo=mysql&logoColor=white" />&nbsp
  <img src="https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=Docker&logoColor=white"/>&nbsp
</div>

<h4>AI</h4>
<div>
  <img src="https://img.shields.io/badge/openai-412991?style=for-the-badge&logo=openai&logoColor=white"/>
  <img src="https://img.shields.io/badge/faiss-E34F26?style=for-the-badge&logo=openai&logoColor=white"/>
  <img src="https://img.shields.io/badge/yt_dlp-009688?style=for-the-badge&logo=openai&logoColor=white"/>
  <img src="https://img.shields.io/badge/selenium-1572B6?style=for-the-badge&logo=openai&logoColor=white"/>
</div>

---

## 🍎 System Architecture

```mermaid
flowchart TD
    A[User Resume + Job Posting URL] -->|Input| B[LLM + RAG Processing]
    B --> C[Personalized Interview Question Generation]
    C --> D[Real-time Feedback]
    D --> E[Relevant Video Recommendation System]
    E --> F[UI/UX Frontend]
```

---

## 🍎 UI/UX

![38](https://github.com/user-attachments/assets/bdd8b5f2-f375-417b-83f5-4cf1e4e7a61f)
![39](https://github.com/user-attachments/assets/40c2564b-0a0b-4647-9934-371f94dc76c2)
![40](https://github.com/user-attachments/assets/786c8f87-9fb7-4000-9bc5-20800cdea3de)
![42](https://github.com/user-attachments/assets/15cc7623-9451-4042-ab81-a6f25777c8ad)

---

## 🍎 Core Features

### Video Recommendation System

* Automatically recommends relevant learning videos based on the user's resume and target job position
* Enhances personalization through **FAISS-based vector similarity search**
* Retrieves up-to-date learning resources through YouTube crawling using `yt_dlp` and `selenium`

### AI Interview Chatbot

* Simulates an interviewer by generating personalized interview questions
* Provides **real-time feedback** on user responses and suggests areas for improvement
* Stores interview responses and maintains feedback history to help users track their progress over time

---

## 🍎 Installation & Setup

```bash
# Clone repository
git clone https://github.com/your-repo/jobis.git
cd jobis

# Run Backend
cd backend
docker-compose up --build

# Run Frontend
cd frontend
npm install
npm run dev
```

---

## 🍎 Future Improvements

* Voice-based real-time feedback using **Speech-to-Text and Sentiment Analysis**
* Expansion of company-specific and job-specific interview datasets
* Enhanced **personalization based on user data and interview history**
* Interactive interview mode with realistic video interview simulations

