# ExamGuard AI Proctoring System

## Development of Smart Examination Monitoring Platform with Integrity Analysis & Reporting System

## 1. Project Overview

ExamGuard is an AI-assisted online examination monitoring and proctoring system developed to improve the integrity and reliability of online examinations.

The system provides a controlled examination environment by verifying the identity of candidates, monitoring examination activities, detecting suspicious behaviour, recording proctoring events, calculating examination integrity scores, classifying candidate risk levels, and providing administrators with analytics and reports.

The project combines web application development, database management, computer vision, machine learning, dashboard development, and AI-assisted reporting into a single examination monitoring platform.

---

## 2. Problem Statement

Online examinations provide flexibility and accessibility, but they also create challenges related to candidate identity verification, examination monitoring, suspicious activity detection, and maintaining examination integrity.

Traditional online examination systems may depend mainly on login credentials and do not provide sufficient monitoring of candidate behaviour during an examination.

ExamGuard addresses these challenges by introducing automated identity verification, activity monitoring, suspicious-event detection, event logging, integrity analysis, and administrator reporting.

---

## 3. Project Objectives

The main objectives of ExamGuard are:

- To provide secure candidate registration and authentication.
- To verify the identity of candidates before examination.
- To monitor candidate activity during an examination.
- To detect suspicious examination events.
- To record detected events for later analysis.
- To provide warnings when suspicious activity is identified.
- To calculate an examination integrity score.
- To classify candidates according to their examination risk level.
- To provide administrators with examination analytics.
- To support examination and proctoring data export.
- To generate AI-assisted examination integrity reports.
- To validate the complete examination workflow through testing.

---

## 4. Major Features

### 4.1 Candidate Registration

Candidates can register by providing the required information. The system validates the submitted details before creating the candidate account.

The registration process helps ensure that only valid candidate information is stored in the system.

### 4.2 Secure Candidate Login

Candidates can log in using their registered credentials.

The authentication system validates the submitted credentials before allowing access to the examination environment.

### 4.3 Password Security

Candidate passwords are handled using password hashing rather than storing passwords directly in plain text.

This provides an additional layer of security for candidate authentication information.

### 4.4 Face Verification

ExamGuard includes identity verification using computer vision techniques.

The system uses the candidate's facial information to verify that the person attempting to take the examination matches the expected candidate identity.

### 4.5 Face Detection

The system uses computer vision technologies such as OpenCV and MediaPipe for detecting faces during examination monitoring.

Face detection provides information that can be used as part of the examination monitoring process.

### 4.6 Examination Activity Monitoring

During an examination, candidate activity is monitored to identify events that may indicate suspicious behaviour.

The detected events are recorded so that they can be analyzed after or during the examination.

### 4.7 Suspicious Event Detection

ExamGuard identifies predefined suspicious examination events and records them in the system.

Examples of monitored events can include unexpected candidate activity or conditions that require further examination.

### 4.8 Warning System

When suspicious activity is detected, the system can generate warnings for the candidate.

The warning mechanism helps notify the candidate while also maintaining a record of the event.

### 4.9 Event Logging

Detected examination events are stored as records.

Event logging provides administrators with a history of examination-related activities and supports later integrity analysis.

### 4.10 Integrity Score Calculation

ExamGuard uses recorded examination events to calculate an examination integrity score.

The score provides a summarized representation of the candidate's examination monitoring results.

### 4.11 Risk Classification

Based on examination monitoring and integrity information, the system classifies candidates into appropriate risk levels.

This helps administrators identify examinations that may require additional review.

### 4.12 Administrator Dashboard

The administrator dashboard provides a centralized interface for reviewing examination and proctoring information.

Administrators can use the dashboard to inspect candidate information, examination events, analytics, integrity information, and reports.

### 4.13 Analytics

The system provides analytical information based on examination and proctoring data.

The analytics functionality helps administrators understand examination activity and integrity-related information.

### 4.14 Data Export

Relevant examination and proctoring information can be exported for further analysis, record keeping, or reporting purposes.

### 4.15 AI-Assisted Report Generation

ExamGuard includes an AI-assisted reporting component for generating examination integrity reports from available examination and monitoring information.

The project uses LangChain and OpenAI-related components for the AI reporting functionality.

---

## 5. Technology Stack

### 5.1 Backend Technologies

- Python
- Flask
- SQLite

Python is used as the primary programming language.

Flask is used for developing the web application and handling application routes and backend functionality.

SQLite is used for storing application and examination-related data.

### 5.2 Computer Vision and Machine Learning

- OpenCV
- MediaPipe
- YOLO
- Scikit-learn

OpenCV and MediaPipe support computer vision and face-related processing.

YOLO is used for object-detection-related processing.

Scikit-learn supports machine learning functionality used within the project.

### 5.3 Dashboard and Data Analysis

- Streamlit
- Pandas
- NumPy
- Matplotlib

Streamlit is used for dashboard and monitoring-related interfaces.

Pandas and NumPy support data processing and analysis.

Matplotlib is used for data visualization.

### 5.4 AI Reporting

- LangChain
- OpenAI

These technologies support the AI-assisted examination report generation functionality.

### 5.5 Development Tools

- Visual Studio Code
- Git
- GitHub
- Python virtual environment

Git and GitHub are used for source-code management, version control, and project documentation.

---

## 6. System Architecture

ExamGuard is organized into multiple components that work together to provide the complete examination monitoring workflow.

The major components are:

### Candidate Interface

The candidate interface provides functionality for:

- Registration
- Login
- Identity verification
- Examination access
- Examination activity monitoring
- Warnings
- Examination submission

### Backend Application

The Flask backend manages:

- Application routes
- Authentication
- Candidate information
- Examination operations
- Event processing
- Database communication
- Application logic

### Database Layer

The database stores information required by the application, including candidate and examination-related records and monitoring events.

### AI and Computer Vision Layer

The AI and computer vision components support:

- Face detection
- Face verification
- Object detection
- Suspicious-event monitoring
- Integrity analysis

### Analytics and Dashboard Layer

The dashboard and analytics components provide administrators with:

- Examination information
- Candidate monitoring information
- Event analysis
- Integrity scores
- Risk classification
- Reports
- Data export

---

## 7. Project Workflow

The overall ExamGuard workflow is as follows:

### Step 1: Candidate Registration

The candidate provides the required registration information.

The system validates the submitted information and creates the candidate account when the information is valid.

### Step 2: Candidate Authentication

The candidate enters the registered credentials.

The system validates the credentials and provides access when authentication is successful.

### Step 3: Identity Verification

Before the examination begins, the candidate's identity is verified using the available face verification functionality.

### Step 4: Examination Begins

After successful verification, the candidate can begin the examination.

The examination environment maintains the required examination session information.

### Step 5: Examination Monitoring

Candidate activity is monitored during the examination using the available monitoring and computer vision components.

### Step 6: Suspicious Event Detection

When a suspicious condition is identified, the system records the corresponding event.

### Step 7: Warning Generation

Depending on the detected event, the system can generate a warning for the candidate.

### Step 8: Event Logging

Monitoring events and relevant examination information are stored for further analysis.

### Step 9: Integrity Analysis

The recorded examination information is processed to calculate the examination integrity score.

### Step 10: Risk Classification

The system uses the integrity-related information to classify the examination according to its risk level.

### Step 11: Administrator Analysis

The administrator can review examination information, monitoring events, analytics, integrity scores, and risk classifications through the dashboard.

### Step 12: Reporting and Export

Examination information can be exported and AI-assisted examination integrity reports can be generated for further review.

---

## 8. Project Structure

The major project components include:

```text
ExamGuard/
│
├── models/
├── routes/
├── static/
├── templates/
├── utils/
│
├── app.py
├── config.py
├── database.py
├── analytics.py
│
├── streamlit_dashboard.py
├── requirements.txt
├── requirements-streamlit.txt
│
├── test_analytics_part13.py
├── test_camera.py
├── test_face_mesh.py
├── test_haar.py
├── test_mediapipe.py
├── test_proctoring_fix.py
├── test_session_dashboard.py
├── test_yolo.py
│
├── update_database.py
├── update_database_part11.py
├── update_database_part12.py
├── update_database_part13.py
│
├── yolov8n.pt
├── yolov8m.pt
│
├── README.md
├── Documentation.md
└── LICENSE


The repository also contains Agile documentation under:
docs/
└── Agile_Documentation/
    ├── ExamGuard_Agile_Template.xlsx
    ├── ExamGuard_Defect_Tracker.xlsx
    └── ExamGuard_Unit_Test_Plan.xlsx
These documents contain the project planning, defect tracking, and unit-testing information prepared for the project.

9. Database Management

The project uses SQLite for application data storage.

The database layer is responsible for managing application data and providing the required information to the backend components.

The database-related functionality supports the storage and retrieval of information required for:

Candidate accounts
Examination information
Monitoring events
Examination results
Integrity analysis
Risk classification
Reporting

Database update scripts are also maintained in the repository for project development and database modification activities.

10. Examination Integrity Analysis

One of the main purposes of ExamGuard is to convert examination monitoring information into useful integrity information.

The analysis process can be summarized as:

Candidate Activity
        ↓
Event Detection
        ↓
Event Logging
        ↓
Event Analysis
        ↓
Integrity Score
        ↓
Risk Classification
        ↓
Administrator Review
        ↓
Integrity Report

The integrity score provides a summarized view of the examination monitoring results.

Risk classification helps administrators identify examinations that may require additional attention.

11. AI-Assisted Reporting

The project includes an AI-assisted reporting component.

The reporting process uses available examination and monitoring information to generate a structured examination integrity report.

The AI reporting functionality is designed to help administrators understand the examination results without manually reviewing every individual event.

The project uses LangChain and OpenAI-related components as part of this reporting functionality.

The generated report is intended to support administrative review and should be considered together with the underlying examination records and detected events.

12. Testing Strategy

Testing was performed across different parts of the system to verify functionality and identify defects.

The testing areas include:

Candidate registration
Invalid registration
Candidate login
Invalid login
Password security
Face verification
Face detection
Suspicious-event detection
Warning system
Event logging
Integrity-score calculation
Risk classification
Examination timer
Examination submission
Administrator dashboard
Examination analytics
Data export
AI report generation
End-to-end examination workflow
Invalid and edge-case inputs

The project also contains individual testing scripts for camera processing, face detection, MediaPipe processing, YOLO processing, analytics, dashboard functionality, and proctoring-related functionality.

The completed Unit Test Plan documents the test cases, test procedures, expected results, actual results, and test status.

13. End-to-End Validation

The complete examination workflow was validated through end-to-end testing.

The end-to-end validation covers the major application flow from candidate access through examination monitoring and related analysis.

The completed testing record includes successful execution of the available end-to-end test cases.

14. Defect Management

Defects identified during development and testing were recorded in the Defect Tracker.

The Defect Tracker contains information such as:

Defect identification number
Submitted by
Submission date
Defect description
Detected sprint
Assigned team member
Defect type
Action taken
Action date
Defect status
Remarks

Identified issues were reviewed and corrective actions were recorded.

Open issues are retained in the tracker when further investigation or resolution is required.

15. Agile Development

The project development process was documented using Agile documentation.

The Agile documentation contains:

Product Backlog
Sprint Backlog
Stand-up Meeting records
Sprint Retrospection

The Product Backlog contains user stories and their priority, dependencies, assignee, and status.

The Sprint Backlog contains tasks, dates, team member information, activities, estimates, and daily progress.

Stand-up Meeting documentation records development impediments and the actions taken to address them.

Retrospection documentation records observations from the sprint and identifies activities that should be started, stopped, or continued.

16. Documentation Files

The repository contains project documentation and supporting development documents.

The documentation includes:

README.md — Provides a high-level overview of the project.
Documentation.md — Provides detailed project documentation.
LICENSE — Contains the MIT License.
docs/Agile_Documentation/ExamGuard_Agile_Template.xlsx — Contains Agile planning and sprint documentation.
docs/Agile_Documentation/ExamGuard_Defect_Tracker.xlsx — Contains defect tracking information.
docs/Agile_Documentation/ExamGuard_Unit_Test_Plan.xlsx — Contains the unit test plan and test cases.

The Agile reference files supplied by the mentor are not included in the repository. The files in the repository are the completed project-specific documentation files.

17. Security Considerations

The project includes several security-related practices:

Candidate authentication
Password hashing
Input validation
Controlled access to examination functionality
Database-based information management
Environment-variable support for sensitive configuration

Sensitive configuration values should be maintained outside the source code.

The repository .gitignore is configured to prevent common environment files, Python cache files, virtual environments, and local database files from being committed accidentally.

18. Project Limitations

The project has some practical limitations that should be considered when deploying and using the system.

The performance of computer vision and AI-based monitoring depends on available hardware, camera quality, lighting conditions, and software dependencies.

AI-based detection results may require administrator review because automated detection can produce incorrect or incomplete results in certain conditions.

The deployment environment must also provide compatible Python packages and sufficient resources for the computer vision and machine learning components.

19. Future Enhancements

Possible future improvements include:

Improved real-time browser-based camera monitoring
More advanced suspicious-behaviour detection
Improved face verification accuracy
Additional examination analytics
More detailed administrator controls
Improved AI-generated reports
Cloud-based database integration
Scalable deployment architecture
Enhanced examination security controls
Automated notification and alert mechanisms
Improved user interface and accessibility
More comprehensive automated testing
20. Project Status

The core ExamGuard components have been implemented and tested.

The project currently includes:

Candidate registration
Authentication
Password security
Face verification
Face detection
Examination monitoring
Suspicious-event detection
Warning functionality
Event logging
Integrity-score calculation
Risk classification
Administrator dashboard
Analytics
Data export
AI-assisted reporting
Unit testing
End-to-end validation
Agile documentation
Defect tracking

The project is maintained as an ongoing development project, with further improvements possible in deployment, scalability, monitoring accuracy, and user experience.

21. Conclusion

ExamGuard provides an integrated approach to online examination monitoring by combining authentication, identity verification, computer vision, suspicious-event detection, event logging, integrity analysis, risk classification, analytics, and AI-assisted reporting.

The system is designed to support administrators in reviewing examination activity and identifying examinations that may require additional attention.

The combination of automated monitoring and structured reporting provides a foundation for developing a more reliable and transparent online examination monitoring platform.

22. Author

Revu Siri Harshini
