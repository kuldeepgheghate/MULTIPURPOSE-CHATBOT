# MULTIPURPOSE-CHATBOT

## Overview
The Multi-Purpose ChatBot is a Python-based application that integrates various functionalities such as web scraping, LinkedIn profile fetching, and conversational AI capabilities using FastAPI and LangChain. This project is designed to facilitate natural conversations and perform specific tasks based on user input.

## Features
- **Web Scraping:** Scrapes a specified website and finds occurrences of a given text.
- **LinkedIn Profile Fetching:** Retrieves LinkedIn profile details based on a username.
- **LinkedIn Posting:** Allows users to post updates on LinkedIn.
- **Conversational AI:** Engages users in natural conversations using LangChain and OpenAI.

## Command Tasks:  
    This ChatBot should be equipped to execute specific tasks that extend beyond general conversation. Examples of these command tasks include:
        i. Fetch LinkedIn Profile Details: The bot should be able to retrieve public information from LinkedIn profiles based on user input.

        ii. Update a Post about Trumio on LinkedIn: The ChatBot should be capable of interfacing with LinkedIn to post updates or articles about specified topics, like Trumio, using provided credentials or API access.

        iii. Web Scrape a Website and Search for Occurrences of a Text: The bot should perform web scraping activities to search websites for specific text or patterns, providing the results back to the user in a concise format.

## Prerequisites
Before you begin, ensure you have met the following requirements:
- **Python 3.8 or higher**
- **Node.js and npm** (for the React frontend)
- **Access tokens for LinkedIn API and OpenAI API**

## Installation for BACKEND (in Command Prompt or Windows Powershell)
1. **Clone the repository**
   git clone https://github.com/yourusername/multi-purpose-chatbot.git
   cd multi-purpose-chatbot

2. **Set up a virtual environment**
    python -m venv venv
    venv\Scripts\activate

3. **Install required Python packages**
    pip install -r requirements.txt

4. **Create a .env file in the project root directory and add your API keys:**
    LINKEDIN_ACCESS_TOKEN=your_linkedin_access_token
    OPENAI_API_KEY=your_openai_api_key

5. **Instructions for Use**
    1. **Setup Environment**: Follow the installation instructions in `README.md`.
    2. **Run the Server**: Start the FastAPI server :uvicorn backend.main:app --reload
                            and Open your browser and navigate to http://127.0.0.1:8000/docs to access the API documentation.
    3. **Test Endpoints**: Use tools like cURL to test the different endpoints.

    ### Final Notes
    - Make sure to replace placeholder values (like `YOUR_PERSON_URN` and `YOUR_LINKEDIN_ACCESS_TOKEN`) with actual values where required.
    - Add proper error handling and testing to ensure reliability.


## Installation for FRONTEND
**Frontend Installation Guide**
    Prerequisites:
        Before you begin, ensure you have the following installed on your system:
            Node.js: Install Node.js, which includes npm (Node Package Manager). You can download it from Node.js official website.
            Create React App: You can create your React application using Create React App.

1. Set Up Your React App
Create a New React Application: Open your terminal and run the following command to create a new React application:
        npx create-react-app frontend
        This command creates a new directory named frontend with the initial project structure.

2. Navigate to the Project Directory: Change your directory to the newly created React app:
        cd chatbot-frontend

3. Install Required Packages: Install any required packages such as axios for making HTTP requests and react-markdown for rendering markdown:
        npm install axios react-markdown

## Your project structure should look like this:

    frontend/
    ├── node_modules/
    ├── public/
    ├── src/
    │   ├── App.js
    │   ├── index.js
    │   ├── index.css
    │   └── ...
    ├── package.json
    └── README.md

    -> src/App.js: Main component file.
    -> src/index.js: Entry point for the React application.
    -> src/index.css: add some basic styles

4. Run the React Application
    # Start the React Development Server: In the terminal, run the following command to start the React app:
        npm start

        -> This command will open your application in the default web browser, typically at http://localhost:3000.

# Simultaneous Running
    You should now have:

    Your FastAPI backend running on http://127.0.0.1:8000
    Your React frontend running on http://localhost:3000
    Both applications can communicate with each other. In your React app, make sure that you point to the FastAPI backend API endpoints correctly.


**Your React frontend is now set up and connected to your FastAPI backend via WebSockets for real-time communication. You can extend the functionality by adding features such as LinkedIn profile fetching, posting updates, and improving the chat interface.**

# This Chatbot has integrated the following technologies to ensure a seamless and robust implementation:
    a. FastAPI for building and managing API endpoints.
    b. Python as the primary programming language due to its extensive libraries and ease of integration with AI models.
    c. ReactJS for building the user interface, offering a dynamic and responsive user experience.
    d. WebSockets to enable real-time communication between the ChatBot and users, ensuring prompt task execution and feedback.
    e. LangChain to manage and chain together various NLP tasks, enhancing the bot’s ability to handle complex requests.
    f. OpenAI for leveraging advanced conversational AI models that drive the bot's general discussion capabilities.


# This README provides a comprehensive guide to setting up your Multi-Purpose ChatBot and will be very helpful for anyone looking to use or contribute to your project!
