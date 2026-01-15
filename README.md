📖 Real-Time Chat Application
A real-time chat application built with Flask and Flask-SocketIO, designed to support multiple chat rooms, private messaging, and dynamic user management.
----------

✨ Features
Guest authentication: users are automatically assigned a unique guest username (GuestXXXX).

Chat rooms: multiple predefined rooms (General, Zero to Knowing, Code you Code, The Nerd Nook).

Public messages: broadcasted to all users in the current room.

Private messages: sent directly to a specific user using the @username syntax.

Active users list: dynamically updated in real time.

System notifications: automatic messages when users join or leave rooms.

Modern frontend: responsive interface built with HTML, CSS, and JavaScript.

-----------
🛠️ Tech Stack
Backend: Python 3, Flask, Flask-SocketIO, Werkzeug ProxyFix

Frontend: HTML5, CSS3, Vanilla JavaScript

Real-time communication: WebSockets via Socket.IO

Logging: Python logging for event monitoring
--------------
📂 Project Structure
REAL_TIME_CHAT/

├── chat_app/

│   ├── static/

│   │   ├── chat.js  # Client-side Socket.IO logic

│   │   └── styles.css      # UI styling

│   ├── templates/

│   │   └── index.html      # Main template

│   └── main.py             # Flask + SocketIO server

└── README.md

-----------

⚙️ Installation & Setup
1. Clone the repository:
   git clone https://github.com/yourusername/real-time-chat.git
  cd real-time-chat/chat_app

2. Create and activate a virtual environment:2.
  python -m venv .venv
  source .venv/bin/activate   # Linux/Mac
  .venv\Scripts\activate      # Windows

3. Install dependencies:
   pip install flask flask-socketio eventlet

4. Run the application:
  python main.py

5. Open in your browser:
   http://127.0.0.1:5000
   
----------------
💻 Usage
   On entry, you are assigned a guest username automatically.

   Select a room from the sidebar.

   Type messages in the input field.

   To send a private message:
     @Username Hello, this is a private message
     
-----------------
🔒 Security Notes

   Active users are stored in memory (active_users dict).
   
   For production, use Redis or another distributed storage solution.
   
   Configure SECRET_KEY and CORS_ORIGINS via environment variables.

---------------
🚀 Future Improvements

   - User authentication and registration.
   
   - Persistent message storage in a database.
   
   - File and media sharing support.
   
   - Push notifications.
   
   - Deployment with Docker/Kubernetes.

----------------
## 📜 License
This project is licensed under the MIT License.  
You are free to use, modify, and distribute this software with proper attribution.




