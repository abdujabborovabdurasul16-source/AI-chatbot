Flask Chatbot with BlenderBot
This project is a simple Flask web application that integrates the BlenderBot 400M Distill (huggingface.co in Bing) model from Hugging Face Transformers. It provides a web interface for conversational AI, with CORS enabled for cross-origin requests.

Features
Flask backend serving a chatbot interface
Integration with Hugging Face’s transformers library
Conversation history tracking
Web UI via index.html
CORS support for API calls from external clients

Requirements
Python 3.8+
pip / virtualenv
Dependencies listed in requirements.txt:
text
flask
flask-cors
transformers
torch
Installation
Clone the repository
powershell
# On Windows PowerShell
python -m venv my_env
.\my_env\Scripts\Activate
bash
# On Linux/macOS
python3 -m venv my_env
source my_env/bin/activate
Install dependencies:

bash
pip install -r requirements.txt
Running the App
Start the Flask server:

bash
python app.py
By default, the app runs on:
Code.
http://127.0.0.1:5000/
Open this URL in your browser to access the chatbot interface.
How It Works
Loads the BlenderBot model and tokenizer from Hugging Face.
Maintains a conversation_history list.
Provides a home route (/) that serves index.html.
Future expansion: add a /chat route to handle user input and return model responses.

Deployment
You can deploy this app using:

Heroku
IBM Code Engine 
Docker containerization

 Next Steps
Implement chat endpoint for AJAX requests

Enhance conversation memory

Add frontend styling and interactivity
