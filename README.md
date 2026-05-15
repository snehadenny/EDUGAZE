# EDUGAZE
EduGaze is an AI-powered web application that monitors student attention during online classes using webcam-based gaze tracking and machine learning. It detects engagement, distractions, attendance, and generates real-time reports while ensuring privacy through local browser-side processing.

## Features
- Real-Time Engagement Monitoring
- Gaze Tracking System
- Tab Switching Detection
- Attendance Tracking
- AI-Based Transcript
- Teacher Dashboard
- Note Uploading Feature
- AI Suggestion System
- Low-Latency Communication
- Privacy-Focused Design

## Directory Breakdown

```bash
webgazer/
├── apps/
│   ├── server/              ➜ Express API & Socket.io backend
│   ├── dashboard2/          ➜ React-based Admin Dashboard
│   ├── extension/           ➜ Student Tracking Extension
│   ├── extension-teacher/   ➜ Teacher Extension Module
│   └── uploads/             ➜ Uploaded notes and session resources
│
├── dev/                     ➜ Development scripts and utilities
├── html/                    ➜ Documentation and static files
└── package.json             ➜ Monorepo configuration
```

# Technologies Used
### Frontend
- React 19 & Vite -for a blazing-fast dashboard.
- Mantine UI -for a premium, accessible component library.
### Backend
- Node.js & Express with Socket.IO  -for real-time duplex communication between extension and dashboard.
### AI & Machine Learning
- WebGazer.js – Gaze tracking
- OpenCV – Face and eye detection
- Google Gemini – AI-based summaries and suggestions
- NLP (Natural Language Processing) – Automated notes generation
- Speech-to-Text – Real-time transcript generation
### Artificial Intelligence
Ollama (Llama 3.2) -powers our local LLM infrastructure for report generation and real-time content recovery.
### Data Persistence
SQLite with optimized indexing -for low-latency event logging and session management.

# Running Process
 ### 1. Clone the Repository
 ```bash
git clone <repository-link>
cd EduGaze
```
### 2. Install Frontend Dependencies
```bash 
cd frontend
npm install
```
### 3. Install Backend Dependencies
```
cd ../backend
npm install
```
### 4. Configure Environment Variables

Create a .env file in the backend folder and add:
```
PORT=5000
MONGO_URI=your_database_url
GEMINI_API_KEY=your_api_key
JWT_SECRET=your_secret_key
```
### 5. Start the Backend Server
```
npm start
```
### 6. Start the Frontend Application

Open another terminal and run:
```
cd frontend
npm run dev
```
### 7. Open the Application

Visit:
```
http://localhost:5173
```
### 8. Grant Permissions

Allow webcam and microphone access for real-time monitoring.

### 9. Start a Session
- Sign in as Teacher
- Enter session details
- Click Initialize Tracking
### 10. Features During Session
- Real-time gaze tracking
- Attention monitoring
- Attendance tracking
- Tab switching detection
- AI transcript generation
- Dashboard analytics
### 11. End Session

After ending the session, the system generates:

- Engagement reports
- Student analytics
- AI insights
- Session summaries

# System Design
### System Architecture
The figure shows EduGaze's modular, real-time architecture, centered on a backend server connecting the User Interface with AI modules. It has three layers: an Input Layer (for webcam and mic), an AI Processing Layer (gaze tracking, attention detection, speech-to-text), and an Application & Storage Layer (managing operations and data). This hub-and-spoke design allows independent module updates, providing a scalable and efficient solution for online learning.

![img](https://github.com/snehadenny/EDUGAZE/blob/b8ad2ad9b2ac7172fd3a134a56fee7ee54b80014/System%20Arch.jpeg)
![img](https://github.com/snehadenny/EDUGAZE/blob/654c9121863d6bb464a00c20c99ba0e51e020dda/system%20workflow.jpeg)


### Use case diagram
The Use Case diagram shows key interactions between the Student, Teacher, and EduGaze modules. It outlines actions like capturing video, calibrating gaze, and monitoring attention. It also maps how the system creates student summaries, pedagogical reports, and AI feedback. This blueprint ensures all user actions align with system features, supporting an intelligent learning environment.

![img](https://github.com/snehadenny/EDUGAZE/blob/654c9121863d6bb464a00c20c99ba0e51e020dda/usecase%20diagramm.jpeg)

# Results
### Sign-in Page
The Sign-in page is the starting interface for instructors to begin real-time student attention monitoring. It includes navigation options such as History, Go Live, Notes, and Settings. Instructors can enter session details and start monitoring using the “Initialize Tracking” option, which activates gaze tracking and attention analysis.

![img](https://github.com/snehadenny/EDUGAZE/blob/654c9121863d6bb464a00c20c99ba0e51e020dda/sign%20in%20page.jpeg)

### Knowledge Base
The Knowledge Base interface allows instructors to upload and manage study materials like PDFs, DOCX, PPTX, and images. Uploaded resources are displayed in the resource library for easy student access, supporting organized and efficient learning material distribution.

![img](https://github.com/snehadenny/EDUGAZE/blob/5799d8dd91d07eedbf5688a32208db3a3f2df2e4/knowledge%20base.jpeg)

### Past And Live session View
past: 

![img](https://github.com/snehadenny/EDUGAZE/blob/6960b112ea2b1de0b0653e3b74e2561353b4b695/past.jpeg)

live:

![img](https://github.com/snehadenny/EDUGAZE/blob/d589730dcc488a93a95516abac2827c94c154ebb/live.jpeg)

### Session Report
The Sessional Report interface provides a summary of completed sessions, including average engagement, attendance, and peak distraction moments. It also supports report sharing and data export for further analysis.

The student page displays individual performance details such as engagement levels, activity status, timelines, and AI insights, helping instructors track and improve student learning outcomes.

![img](https://github.com/snehadenny/EDUGAZE/blob/654c9121863d6bb464a00c20c99ba0e51e020dda/session%20report.jpeg)

### Real-time student engagement and attention overview
The figure shows a classroom analytics dashboard with real-time student engagement metrics such as attendance, distraction level, average attention, session duration, and shared materials. It also includes an Engagement Flow graph that visualizes attention levels throughout the session, helping track student focus and identify distraction patterns.

![img](https://github.com/snehadenny/EDUGAZE/blob/654c9121863d6bb464a00c20c99ba0e51e020dda/real%20time%20engagement%20and%20attension%20overview.jpeg)



