Chatbot Project README
LEARNFLU FINAL PROJECT CHATBOT (AI ML )
NAME : PRAKASH RAJ A


Overview
This project implements a simple chatbot using Flask and the DialoGPT model from the Hugging Face Transformers library. The chatbot is capable of engaging in conversations with users and generates responses based on user inputs.

Table of Contents
Requirements
Setup
Running the Application
Usage
Code Explanation

Requirements
To run this project, you need the following:

Python 3.6 or higher
Flask
Transformers
Torch
(Optionally) A virtual environment manager (like venv or conda)
You can install the required packages using:
    pip install flask transformers torch

Installation & Setup

[Install Python] https://www.python.org/downloads/

[Install pip]  curl https://bootstrap.pypa.io/get-pip.py -o get-pip.py

python3 get-pip.py

Ensure pip is installed by running the following command

pip --version

If you have Python & pip installed then check their version in the terminal or command line tools

python3 --version
pip --version

Installing Flask
In your terminal run the requirements.txt file using this pip
                   pip install -r requirements.txt

SET UP:

Clone the Repository:
  
          git clone https://github.com/your-username/chatbot-project.git
          
          cd chatbot-project

Create a Virtual Environment (optional but recommended):


          python -m venv venv

          source venv/bin/activate  # On Windows use `venv\Scripts\activate

Install Dependencies:

             pip install -r requirements.txt

ChatBot Link

          The Chatbot is constructed using the Microsoft/DialoGPT-medium model.

          https://huggingface.co/microsoft/DialoGPT-medium


Running the Application

Start the Flask server: 
           python app.py

Access the Chatbot: Open your web browser and navigate to http://127.0.0.1:5000/.

Usage
Type your message in the chat input field and press Enter or click the send button.
The chatbot will respond based on the input you provided.
You can continue the conversation by typing more messages.

Code Explanation
app.py: This is the main application file. It sets up the Flask app, loads the DialoGPT model, and defines routes for rendering the chat interface and handling messages.

Routes:

"/": Renders the main chat interface.
"/get": Handles POST requests to process user messages and return chatbot responses.

get_Chat_response function: This function processes the user's input and generates a response using the DialoGPT model. It maintains the conversation history for context.

