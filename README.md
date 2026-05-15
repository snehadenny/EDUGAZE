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

# Technologies Used
### Frontend
- React – Teacher dashboard and user interface
- TypeScript – Frontend development
- HTML, CSS – UI design and styling
- Recharts – Analytics and graphs
- Socket.IO – Live data updates
- Lucide – Dashboard icons
### Backend
- Node.js – Backend server
- Express.js – API handling and server management
- Socket.IO – Real-time synchronization
- Multer – File uploading support
- JWT / Authentication APIs – User authentication and session handling
### AI & Machine Learning
- WebGazer.js – Gaze tracking
- OpenCV – Face and eye detection
- Google Gemini – AI-based summaries and suggestions
- NLP (Natural Language Processing) – Automated notes generation
- Speech-to-Text – Real-time transcript generation
### Database & Storage
- Database (DB) – Session data, notes, and analytics storage
- Cloud-based storage – Learning material and transcript storage
- Browser & Extension Technologies
- Google Chrome Extension – Real-time monitoring and tab tracking
- Browser APIs – Webcam, microphone, and activity detection
### Communication & Deployment
- REST APIs – System integration and communication
- Low-latency real-time processing architecture
- Secure web-based deployment

# System Design
### System Architecture
The figure shows EduGaze's modular, real-time architecture, centered on a backend server connecting the User Interface with AI modules. It has three layers: an Input Layer (for webcam and mic), an AI Processing Layer (gaze tracking, attention detection, speech-to-text), and an Application & Storage Layer (managing operations and data). This hub-and-spoke design allows independent module updates, providing a scalable and efficient solution for online learning.
![img](https://github.com/snehadenny/EDUGAZE/blob/b8ad2ad9b2ac7172fd3a134a56fee7ee54b80014/System%20Arch.jpeg)
![img]()

### Use case diagram
The Use Case diagram shows key interactions between the Student, Teacher, and EduGaze modules. It outlines actions like capturing video, calibrating gaze, and monitoring attention. It also maps how the system creates student summaries, pedagogical reports, and AI feedback. This blueprint ensures all user actions align with system features, supporting an intelligent learning environment.
![img]()

# Results
### Sign-in Page
The Sign-in page is the starting interface for instructors to begin real-time student attention monitoring. It includes navigation options such as History, Go Live, Notes, and Settings. Instructors can enter session details and start monitoring using the “Initialize Tracking” option, which activates gaze tracking and attention analysis.
![img]()

### Knowledge Base
The Knowledge Base interface allows instructors to upload and manage study materials like PDFs, DOCX, PPTX, and images. Uploaded resources are displayed in the resource library for easy student access, supporting organized and efficient learning material distribution.
![img](https://github.com/snehadenny/EDUGAZE/blob/5799d8dd91d07eedbf5688a32208db3a3f2df2e4/knowledge%20base.jpeg)

### Past And Live session View
![img]()
![img]()

### Session Report
The Sessional Report interface provides a summary of completed sessions, including average engagement, attendance, and peak distraction moments. It also supports report sharing and data export for further analysis.

The student page displays individual performance details such as engagement levels, activity status, timelines, and AI insights, helping instructors track and improve student learning outcomes.
![img]()

### Real-time student engagement and attention overview
The figure shows a classroom analytics dashboard with real-time student engagement metrics such as attendance, distraction level, average attention, session duration, and shared materials. It also includes an Engagement Flow graph that visualizes attention levels throughout the session, helping track student focus and identify distraction patterns.
![img]()



