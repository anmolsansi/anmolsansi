<h1 align="center">Hi, I'm Anmol Sansi 👋</h1>

<h3 align="center">
ML/AI Full Stack Software Engineer | Python, Java, React, AWS | LLMs + RAG | High-Throughput APIs, Cloud Systems, SQL/NoSQL
</h3>

<p align="center">
  <a href="mailto:asansi0896@gmail.com">
    <img src="https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white" alt="Email" />
  </a>
  <a href="https://www.linkedin.com/in/anmol-sansi/">
    <img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn" />
  </a>
  <a href="https://anmolsansi.github.io/Anmol-Sansi-Resume/">
    <img src="https://img.shields.io/badge/Portfolio-000000?style=for-the-badge&logo=githubpages&logoColor=white" alt="Portfolio" />
  </a>
  <a href="https://github.com/anmolsansi">
    <img src="https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white" alt="GitHub" />
  </a>
</p>


---

## 👨‍💻 About Me

- ML/AI **Full Stack Software Engineer** with 4+ years of experience building production systems in Python, Java, and JavaScript/ TypeScript.  
- Comfortable owning services end‑to‑end: API design, data modeling (PostgreSQL, MongoDB), containerization, observability, and on‑call incident response in cloud environments (AWS, Docker, Kubernetes).
- Recently focused on AI‑powered products: LLM + RAG workflows, multi‑agent systems, and automation tools that compress manual work from hours to minutes. 

---

## 🧠 Tech Stack

**Languages**

<p>
  <img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white" />
  <img src="https://img.shields.io/badge/Java-007396?style=for-the-badge&logo=openjdk&logoColor=white" />
  <img src="https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white" />
  <img src="https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=000" />
</p>

**Backend & APIs**

<p>
  <img src="https://img.shields.io/badge/FastAPI-009688?style=for-the-badge&logo=fastapi&logoColor=white" />
  <img src="https://img.shields.io/badge/Flask-000000?style=for-the-badge&logo=flask&logoColor=white" />
  <img src="https://img.shields.io/badge/Django-092E20?style=for-the-badge&logo=django&logoColor=white" />
  <img src="https://img.shields.io/badge/Spring%20Boot-6DB33F?style=for-the-badge&logo=springboot&logoColor=white" />
  <img src="https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=nodedotjs&logoColor=white" />
  <img src="https://img.shields.io/badge/REST%20APIs-005571?style=for-the-badge&logo=swagger&logoColor=white" />
</p>

**Frontend**

<p>
  <img src="https://img.shields.io/badge/React-61DAFB?style=for-the-badge&logo=react&logoColor=000" />
  <img src="https://img.shields.io/badge/Redux-764ABC?style=for-the-badge&logo=redux&logoColor=white" />
  <img src="https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white" />
  <img src="https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white" />
</p>

**Databases & Data**

<p>
  <img src="https://img.shields.io/badge/PostgreSQL-4169E1?style=for-the-badge&logo=postgresql&logoColor=white" />
  <img src="https://img.shields.io/badge/MongoDB-47A248?style=for-the-badge&logo=mongodb&logoColor=white" />
  <img src="https://img.shields.io/badge/DynamoDB-4053D6?style=for-the-badge&logo=amazondynamodb&logoColor=white" />
  <img src="https://img.shields.io/badge/SQLite-003B57?style=for-the-badge&logo=sqlite&logoColor=white" />
</p>

**Cloud, DevOps & Infra**

<p>
  <img src="https://img.shields.io/badge/AWS-FF9900?style=for-the-badge&logo=amazonaws&logoColor=white" />
  <img src="https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white" />
  <img src="https://img.shields.io/badge/Kubernetes-326CE5?style=for-the-badge&logo=kubernetes&logoColor=white" />
  <img src="https://img.shields.io/badge/Microservices-000000?style=for-the-badge&logo=microgenetics&logoColor=white" />
</p>

**LLMs & AI**

<p>
  <img src="https://img.shields.io/badge/OpenAI-412991?style=for-the-badge&logo=openai&logoColor=white" />
  <img src="https://img.shields.io/badge/RAG-0A0A0A?style=for-the-badge&logo=vector&logoColor=white" />
  <img src="https://img.shields.io/badge/ChatGPT-00A67E?style=for-the-badge&logo=openai&logoColor=white" />
  <img src="https://img.shields.io/badge/Ollama-000000?style=for-the-badge&logo=ollama&logoColor=white" />
</p>

---

## 🚀 Featured Projects

### 🔹 AI Resume Agent

> Built a FastAPI web app that tailors a resume to a job description, selects the most relevant projects, rewrites content without inventing experience, and exports a downloadable .docx with a side‑by‑side diff.

- Designed `/generate` and `/regenerate` flows that accept pasted resumes or uploaded `.docx`, fall back to a master resume, and return a rich payload (score, summary, selected projects, HTML diff, download link).  
- Implemented a multi‑step LLM pipeline to analyze the JD, select projects, rewrite the resume, and run a recruiter‑style judge loop until the score clears a threshold and project selection is valid.  
- Added resilient iteration by accumulating judge feedback, re‑running project selection on `project_selection_issue`, and always restarting rewrites from a clean base resume.  
- Built strict JD parsing via a local Ollama client with enforced JSON schema, normalization/deduplication, retries with stricter prompts, and fallback to OpenRouter when local models fail.  
- Implemented OpenRouter API key rotation with daily limits, persistent usage tracking, and automatic failover on error codes.  
- Shipped a review‑first UX with versioned `.docx` outputs (v1, v2, …) and side‑by‑side diff tables for easy auditing.  

**Tech:** `Python` · `FastAPI` · `Ollama` · `OpenRouter` · `Docker` · `Uvicorn` · `python-docx`  

---

### 🔹 Resume Tracker — Serverless Web Application

> A serverless app to track job applications and automate follow‑ups.

- Built a serverless backend with Python/Flask on AWS Lambda and API Gateway.  
- Stored application data in DynamoDB and assets in S3 for reliable CRUD workflows.  
- Automated weekly follow‑up reminders using SES and CloudWatch scheduling.  

**Tech:** `Python` · `Flask` · `AWS Lambda` · `DynamoDB` · `API Gateway` · `S3` · `SES` · `CloudWatch` · `React`  

---

### 🔹 AI Job Application Tracker

> A job tracker that parses email confirmations and generates follow‑ups using LLMs.

- Integrated Gmail API to automatically detect job applications and responses.  
- Used OpenAI/LLM prompts to draft personalized follow‑up emails for better reply rates.  
- Stored structured application history in PostgreSQL for querying and reporting.  

**Tech:** `Python` · `Flask` · `PostgreSQL` · `Gmail API` · `LLM`  

---

### 🔹 FHIR-Based Patient Data Ingestion Platform

> A pipeline to ingest and normalize healthcare data following FHIR standards.

- Built ingestion endpoints and validation for structured patient data flows.  
- Normalized data into a consistent schema to enable downstream analytics.  
- Focused on reliability and observability to reduce ingestion failures.  

**Tech:** `Python` · `FastAPI` · `FHIR` · `Docker`  

---

### 🔹 Pharmacy Management System — Desktop and Web

> A role‑based pharmacy system with REST APIs and a React UI.

- Designed role‑based authentication and authorization with REST APIs.  
- Built a React UI with real‑time filtering and form validation for better UX.  
- Improved backend performance with Java and PostgreSQL query tuning.  

**Tech:** `Java` · `PostgreSQL` · `React` · `JSP` · `Maven` · `JavaScript`  

---

### 🔹 The Movie Review — Android Application

> An Android app for browsing movies, trailers, and favorites with offline support.

- Integrated TMDB and OMDB APIs to support large‑scale movie browsing.  
- Added favorites and improved retention with a cleaner UI flow.  
- Implemented offline access with SQLite and auth with Firebase.  

**Tech:** `Java` · `Kotlin` · `TMDB API` · `OMDB API` · `Firebase` · `SQLite` · `YouTube API`  

---

## 💼 Experience Snapshot

- **Full Stack Engineer – Alphadroid (USA)**  
  Built multilingual, voice‑assisted platforms and AI hotel agents using React + Python/Node.js + OpenAI, cutting intake time by 30%, boosting form completion by 40%, and improving page load by 25%.

- **AI Full Stack Software Engineer II – AI.Rawat (USA)**  
  Delivered a real‑time sales analytics platform and AI‑driven workflows for Moodle LMS with RAG chatbots and automated reporting, improving academic outcomes by 20% and feedback quality by 30%.

- **Software Engineer – S&P Global (India)**  
  Migrated financial data platforms to the cloud, maintained 99.9% uptime, built 100+ REST APIs, and engineered ETL pipelines processing 1M+ records/day with AWS Lambda, Kinesis, and SQS.

---

