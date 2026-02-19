# 🎓 Smart Exam Script Verification & College Management System - TEAM 164 🚀

![React](https://img.shields.io/badge/React-Frontend-blue.svg)
![Node.js](https://img.shields.io/badge/Node.js-Backend-green.svg)
![MongoDB](https://img.shields.io/badge/MongoDB-Database-green.svg)
![Python](https://img.shields.io/badge/Python-3.9-blue.svg)
![PyTorch](https://img.shields.io/badge/PyTorch-Deep%20Learning-ee4c2c.svg)
![Transformers](https://img.shields.io/badge/Hugging%20Face-TrOCR-yellow.svg)

## 📌 Overview

**Smart Exam Script Verification & College Management System** is a unified digital platform designed to modernize educational institutions. It solves two critical problems: **Administrative Inefficiency** and **Academic Integrity** in handwritten exams.

Unlike traditional ERPs, this system integrates a robust **MERN Stack Web Portal** for daily operations (Attendance, Slot Booking, Parent Updates) with an advanced **AI Evaluation Engine** that automatically detects plagiarism in handwritten assignments using **Transformer-based OCR (TrOCR)**.

---

## 🚀 Key Features

### 🧠 AI Evaluation Engine (Python Microservice)
* **📄 Batch Processing:** Automatically converts and processes folders full of handwritten PDF submissions.
* **🖼️ Advanced Preprocessing:** Uses **OpenCV** (Bilateral Filtering, Adaptive Thresholding) to clean noisy scanned scripts.
* **🤖 AI-Powered OCR:** Utilizes the state-of-the-art `microsoft/trocr-large-handwritten` model to digitize handwriting with high accuracy.
* **🔍 Plagiarism Detection:** Performs $N^2$ pairwise comparison using sequence-matching algorithms to detect verbatim copying.
* **📊 Automated Reporting:** Generates PDF Integrity Reports flagging suspicious pairs (Similarity > 75%).

### 🌐 College Management Web Portal (MERN Stack)
* **🔐 Role-Based Access Control:** Secure login for **Admins, Teachers, Students, and Parents**.
* **📅 Smart Slot Booking:** Real-time checking and booking of Seminar Halls/Labs with conflict prevention logic.
* **👨‍👩‍👧 Parent Portal:** A dedicated dashboard for parents to view their ward's real-time attendance and academic alerts.
* **📂 Digital Submissions:** Students can upload assignments directly, which are stored securely in the cloud.

---

## 🛠️ Tech Stack

| Component | Technology |
| :--- | :--- |
| **Frontend** | React.js, Tailwind CSS, Redux |
| **Backend** | Node.js, Express.js, JWT Authentication |
| **Database** | MongoDB (NoSQL) |
| **AI Engine** | Python 3.9, PyTorch, Hugging Face Transformers |
| **Image Processing** | OpenCV, PIL |
| **Cloud Storage** | AWS S3 / Cloudinary (for PDF storage) |

---

## 📂 Project Structure

```bash
├── client/                # React.js Frontend
│   ├── src/
│   │   ├── components/    # Reusable UI components
│   │   ├── pages/         # Dashboard, Login, Booking pages
│   │   └── redux/         # State management
├── server/                # Node.js Backend
│   ├── models/            # Mongoose Schemas (User, Booking, Submission)
│   ├── routes/            # API Endpoints
│   └── controllers/       # Business Logic
└── ai_engine/             # Python Microservice
    ├── main.py            # Entry point for plagiarism check
    ├── preprocessing.py   # OpenCV image enhancement
    └── ocr_model.py       # TrOCR inference logic

```
## ⚡ Installation & Setup        
Prerequisites      
```python
Node.js & npm installed
Python 3.9+installed
MongoDB running locally or via Atlas
```
## 1. Setup Backend (Server)Bash

```python
cd server
npm install
# Create a .env file and add your MONGO_URI and JWT_SECRET
npm start
```
## 2. Setup Frontend (Client)Bash      

```python
cd client
npm install
npm start
```
The web portal will open at
```http://localhost:3000```
## 3. Setup AI EngineBashcd ai_engine           
```python
pip install torch transformers opencv-python pdf2image scikit-learn
python main.py
```


## How to Run
## Backend (Terminal 1):

bash
```python
cd "c:/Users/SEC/Downloads/main project/project 2/code/codes/backend"
python run.py
```

The server runs on 
```python
http://localhost:5000.
```
## Frontend (Terminal 2):

bash
```python
cd "c:/Users/SEC/Downloads/main project/project 2/code/codes/frontend"
npm run dev
```
Access the app at           
```python
http://localhost:5173.
``` 


## 📸 Screenshots

Admin Dashboard:
<img width="1919" height="951" alt="Screenshot 2026-01-29 103525" src="https://github.com/user-attachments/assets/0a83b75c-a602-4e03-9278-db81cbf68307" />

Parent Portal: 
<img width="1919" height="957" alt="Screenshot 2026-01-29 103738" src="https://github.com/user-attachments/assets/b0a699f7-cc5a-4202-98e2-93f010d91050" />

Student Portal:
<img width="1919" height="946" alt="Screenshot 2026-01-29 103937" src="https://github.com/user-attachments/assets/8f59af67-a8c7-4fb1-aec1-70a631d720cd" />

Plagiarism Report:

![1](https://github.com/user-attachments/assets/fbe922f4-0bf8-4c12-b0ce-429a10987b71)

![2](https://github.com/user-attachments/assets/e6367d41-019d-451e-9530-ff859d21f987)


## 🧪 Algorithms Used    

### TrOCR (Transformer OCR):
Uses a Vision Transformer (ViT) encoder and RoBERTa decoder to transcribe handwritten text.
### SequenceMatcher: 
Recursive longest common subsequence algorithm to calculate similarity ratios (0.0 - 1.0).
### Bilateral Filtering:
Non-linear, edge-preserving, and noise-reducing smoothing filter for images. 
### Bcrypt & JWT:  
For secure password hashing and stateless session management.

### 🤝 Contributors - TEAM 164: 
THANJIYAPPAN K - Full Stack Dev & AI Integration                 
PRAKASH M - Frontend & UI/UX                   
SANJAY K - Backend & Database

### 📝 License   
This project is licensed under the MIT License - see the LICENSE file for details.

### credentials
#### Admin:  
prakash1@gmail.com             
123             
### Parent:
thanji1@gmail.com              
123   
### Teacher
ranga@gmail.com       
123   
### Student
thanji@gmail.com         
123         
