Career Development Assistant📃
A comprehensive Flask-based web application that leverages Google's Gemini AI to provide career development tools and guidance.

This website is launched at: https://careercompass.pythonanywhere.com/
Tech Stack Used
Python
Flask
Html
Css
Javascript
Gemini API
Description
CareerCompass is an AI-powered platform that generates personalized career roadmaps with interactive timelines, offers peer resume comparison, creates tailored resumes, analyzes resume effectiveness, and provides progress tracking and AI mentorship to guide users toward their dream careers.

Homepage:
screencapture-careercompass-pythonanywhere-2025-04-12-08_17_53

Features
Career Roadmap Generator: Creates personalized career development paths based on user goals and current skills

screencapture-careercompass-pythonanywhere-roadmap-2025-04-12-08_21_51

Resume Analyzer: Evaluates resumes and provides detailed feedback and suggestions

screencapture-careercompass-pythonanywhere-resume-analyzer-2025-04-12-09_07_44

Progress Tracker: Monitors and scores weekly career development achievements

screencapture-careercompass-pythonanywhere-progress-tracker-2025-04-12-09_15_28

Resume Comparison: Compares two resumes and provides detailed insights

screencapture-careercompass-pythonanywhere-resume-comparison-2025-04-12-09_17_09

Career Chatbot: Offers personalized career guidance and advice

screencapture-careercompass-pythonanywhere-chatbot-2025-04-12-09_20_33

Resume Builder: Users can select a template and create resume easily by filling simple forms Repository Link for Resume Builder: https://github.com/Aryan-Prasad-666/CareerCompassResume.git

screencapture-careercompassresume-pythonanywhere-2025-04-12-09_24_19

sample

Interactive Web Interface: Clean and user-friendly frontend for all features

Prerequisites
Python 3.7+
Flask
Google Generative AI library
Flask-CORS
Installation
Clone the repository:
git clone https://github.com/Aryan-Prasad-666/CareerCompass.git
cd CareerCompass
Install required dependencies:
pip install flask flask-cors google-generativeai
Set up your Google Gemini API key:
Replace GEMINI_API_KEY in app.py with your actual API key
For production, use environment variables instead of hardcoding
Usage
Start the Flask server:
python app.py
Access the application at http://localhost:5000
API Endpoints
Career Roadmap Generator
Endpoint: /generate-roadmap
Method: POST
Payload:
{
    "name": "string",
    "careerGoal": "string",
    "currentSkills": "string",
    "experience": "string",
    "interests": "string"
}
Resume Analyzer
Endpoint: /analyze-resume
Method: POST
Payload:
{
    "resume": "string"
}
Progress Tracker
Endpoint: /track-progress
Method: POST
Payload:
{
    "achievements": "string"
}
Resume Comparison
Endpoint: /compare-resumes
Method: POST
Payload:
{
    "user_resume": "string",
    "peer_resume": "string"
}
Career Chatbot
Endpoint: /chat
Method: POST
Payload:
{
    "query": "string"
}
Frontend Routes
/: Homepage
/roadmap: Career roadmap generator interface
/resume-analyzer: Resume analysis tool
/progress-tracker: Progress tracking dashboard
/resume-comparison: Resume comparison tool
/chatbot: Career guidance chatbot interface
Error Handling
The application includes comprehensive error handling:

Validates input data
Provides fallback responses if AI service fails
Returns appropriate HTTP status codes
Includes detailed error messages for debugging
Security Considerations
Implements CORS for cross-origin requests
API key should be stored securely in production
Input validation on all endpoints
Error messages are sanitized in production
Development
The application runs in debug mode by default on port 5000. For production:

Disable debug mode
Use environment variables for sensitive data
Implement proper logging
Add rate limiting
Set up proper CORS policies
Contributing
Fork the repository
Create a feature branch
Commit your changes
Push to the branch
Create a Pull Request
License
[Add your license here]
