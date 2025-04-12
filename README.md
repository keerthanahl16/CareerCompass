Career Development Assistant📃

A comprehensive Flask-based web application that leverages Google's Gemini AI to provide career development tools and guidance.

This website is launched at: https://careercompass.pythonanywhere.com/
Tech Stack Used
1.Python
2.Flask
3.Html
4.Css
5.Javascript
6.Gemini API

Description:

CareerCompass is an AI-powered platform that generates personalized career roadmaps with interactive timelines, offers peer resume comparison, creates tailored resumes, analyzes resume effectiveness, and provides progress tracking and AI mentorship to guide users toward their dream careers.

Homepage:
![WhatsApp Image 2025-04-12 at 08 19 18_af8d3e03](https://github.com/user-attachments/assets/98827e47-0398-4348-b594-0c6d5954693c)


Features:

Career Roadmap Generator: Creates personalized career development paths based on user goals and current skills

![screencapture-careercompass-pythonanywhere-roadmap-2025-04-12-08_21_51 1](https://github.com/user-attachments/assets/103a69f3-0347-4e45-b08c-fb1ca5f6c208)


Resume Analyzer: Evaluates resumes and provides detailed feedback and suggestions

![screencapture-careercompass-pythonanywhere-resume-analyzer-2025-04-12-09_07_44 1](https://github.com/user-attachments/assets/50641342-9759-47d5-9df9-0949ec9c3bde)


Progress Tracker: Monitors and scores weekly career development achievements

![Screenshot (11)](https://github.com/user-attachments/assets/1b972e95-f0d9-4414-a984-c9a575183283)


Resume Comparison: Compares two resumes and provides detailed insights

![zbroalwr](https://github.com/user-attachments/assets/a45fcfee-8c1c-4637-ae9f-a6462fd34af7)


Career Chatbot: Offers personalized career guidance and advice

![l7rf81zm](https://github.com/user-attachments/assets/9ee50b99-34bb-4f5f-9320-3014766ace15)


Resume Builder: Users can select a template and create resume easily by filling simple forms Repository Link for Resume Builder: https://github.com/keerthanahl16/CareerCompassResume.git

![screencapture-careercompassresume-pythonanywhere-2025-04-12-09_24_19 1](https://github.com/user-attachments/assets/072125a0-5f36-44c4-b6c6-2e3551515b50)


![dcjeoj9f](https://github.com/user-attachments/assets/eab5cc9f-7cc6-47ec-a0dc-ec1c926a6bf7)


Interactive Web Interface: Clean and user-friendly frontend for all features

Prerequisites

1.Python 3.7+
2.Flask
3.Google Generative AI library
4.Flask-CORS

Installation

1.Clone the repository:
git clone https://github.com/keerthanahl16/CareerCompass.git
cd CareerCompass
2.Install required dependencies:
pip install flask flask-cors google-generativeai
3.Set up your Google Gemini API key:
Replace GEMINI_API_KEY in app.py with your actual API key
For production, use environment variables instead of hardcoding

Usage

1.Start the Flask server:
python app.py
2.Access the application at http://localhost:5000

API Endpoints

Career Roadmap Generator
1.Endpoint: /generate-roadmap
2.Method: POST
3.Payload:
{
    "name": "string",
    "careerGoal": "string",
    "currentSkills": "string",
    "experience": "string",
    "interests": "string"
}

Resume Analyzer
1.Endpoint: /analyze-resume
2.Method: POST
3.Payload:
{
    "resume": "string"
}

Progress Tracker
1.Endpoint: /track-progress
2.Method: POST
3.Payload:
{
    "achievements": "string"
}

Resume Comparison
1.Endpoint: /compare-resumes
2.Method: POST
3.Payload:
{
    "user_resume": "string",
    "peer_resume": "string"
}

Career Chatbot
1.Endpoint: /chat
2.Method: POST
3.Payload:
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

1.Validates input data
2.Provides fallback responses if AI service fails
3.Returns appropriate HTTP status codes
4.Includes detailed error messages for debugging

Security Considerations
1.Implements CORS for cross-origin requests
2.API key should be stored securely in production
3.Input validation on all endpoints
4.Error messages are sanitized in production

Development
The application runs in debug mode by default on port 5000. For production:

1.Disable debug mode
2.Use environment variables for sensitive data
3.Implement proper logging
4.Add rate limiting
5.Set up proper CORS policies

Contributing
1.Fork the repository
2.Create a feature branch
3.Commit your changes
4.Push to the branch
5.Create a Pull Request

License
[Add your license here]
