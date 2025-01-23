# Python Test Assignment

## Overview
This project demonstrates a FastAPI-based application for managing candidate interviews, generating interview questions, and assessing candidate responses. The application provides a seamless workflow for evaluating candidates and storing interview data.

## Features
- RESTful APIs for managing candidates and interviews.
- Automated generation of interview questions based on candidate job titles.
- Assessment of candidate responses with detailed evaluation summaries.
- Persistent storage of interview data.

---

## Getting Started

### Prerequisites
Ensure you have Python 3.10+, Node.js installed on your system.

### Installation

Follow these steps to install and run the application on Windows and macOS.

1. **Clone the Repository**
   ```bash
   git clone https://github.com/Nazar04u/Websocket_JWT_auth
   ```
   Open two terminals
   In the first one
   ```bash
   cd Websocket_JWT_auth/backend/
   ```
   In the second one
   ```bash
   cd Websocket_JWT_auth/frontend/web_socket_chat
   ```

2. **Create a Virtual Environment**
    In the first terminal enter
   ```bash
   #Windows
   python -m venv venv
   venv\Scripts\activate
   
   #MacOS
   python3 -m venv venv
   source venv/bin/activate
   ```


3. **Install Dependencies**
    In the first terminal:
   ```bash
   pip install -r requirements.txt
   ```
   In the second terminal:
   ```bash
   npm install
   ```

4. **Create a `.env` File**
   Create a `.env` file in backend folder in the project root and add your `SECRET_KEY`:
   ```plaintext
   SECRET_KEY=<your_secret_key>
   ```
   or just use for testing reason:
   ```plaintext
   SECRET_KEY=qwerty
   ```

5. **Apply Migrations**
   Apply the generated migration to create the database schema in first terminal:
   ```bash
   alembic upgrade head
   ```

6. **Run the Application**
    In the first terminal run:
   ```bash
   uvicorn app.main:app --port=8000 --reload
   ```
   In the second run:
   ```bash
   npm start
   ```

7. **Access API Documentation**
   Open your browser and navigate to [http://127.0.0.1:8000/docs](http://127.0.0.1:8000/docs) to explore the API endpoints.
   In register endpooint register user and then login.
   To use full app go to  [http://localhost:3000/](http://localhost:3000/)
---

### Notes

- Ensure you have `Python 3.10` or newer installed on your system.
- Install Node.js if you haven’t already, as it’s required to run the frontend.
- If you encounter any issues with permissions, try running commands with `sudo` (macOS) or as Administrator (Windows).
- To stop the application, press `Ctrl+C` in the terminal where the server is running.
