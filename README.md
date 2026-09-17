# ExamGuard AI Proctoring System

## Development of Smart Examination Monitoring Platform with Integrity Analysis & Reporting System

ExamGuard is an AI-assisted online examination monitoring platform designed to improve examination integrity through identity verification, activity monitoring, suspicious-event detection, integrity scoring, risk classification, analytics, and reporting.

## Features

- Candidate registration and secure login
- Application ID and password authentication
- Password hashing
- AI-based face verification
- Face detection using OpenCV and MediaPipe
- Examination activity monitoring
- Suspicious event detection and logging
- Candidate warning system
- Examination integrity score calculation
- Risk-level classification
- Candidate examination analytics
- Administrator monitoring dashboard
- Examination and proctoring data export
- AI-assisted integrity report generation
- End-to-end testing

## Technology Stack

### Backend
- Python
- Flask
- SQLite

### AI/ML and Computer Vision
- OpenCV
- MediaPipe
- YOLO
- Scikit-learn

### Dashboard and Data Analysis
- Streamlit
- Pandas
- NumPy
- Matplotlib

### AI Reporting
- LangChain
- OpenAI

## Project Structure

```text
ExamGuard/
├── app.py
├── config.py
├── requirements.txt
├── streamlit_dashboard.py
├── database/
├── models/
├── routes/
├── utils/
├── templates/
├── static/
├── tests/
└── README.md
