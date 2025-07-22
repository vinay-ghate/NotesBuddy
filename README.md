# NotesBuddy

A simple, secure web-based note-taking application built with Flask. Create, manage, and organize your personal notes with user authentication and a clean, responsive interface.

## Demo Link : [NotesBuddy](https://notesbuddy-1-v6ew.onrender.com)

## Features

- **User Authentication**: Secure signup and login system [1](#0-0) 
- **Personal Notes**: Create and manage private notes tied to your account [2](#0-1) 
- **Real-time Deletion**: Delete notes instantly with AJAX functionality [3](#0-2) 
- **Responsive Design**: Bootstrap-powered UI that works on all devices [4](#0-3) 

## Quick Start

### Prerequisites
- Python 3.6+
- pip package manager

### Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/vinay-ghate/NotesBuddy.git
   cd NotesBuddy
   ```

2. **Install dependencies**
   ```bash
   pip install flask flask-sqlalchemy flask-login
   ```

3. **Run the application**
   ```bash
   python main.py
   ```

4. **Access the app**
   Open your browser and navigate to `http://localhost:5000`

The application will automatically create a SQLite database (`database.db`) on first run. [5](#0-4) 

## Project Structure

```
NotesBuddy/
├── main.py                    # Application entry point
├── website/                   # Main application package
│   ├── __init__.py           # Flask app factory
│   ├── models.py             # User and Note database models
│   ├── views.py              # Note management routes
│   ├── auth.py               # Authentication routes
│   ├── static/               # Static assets
│   │   └── index.js          # Client-side JavaScript
│   └── templates/            # HTML templates
│       ├── base.html         # Base template
│       ├── home.html         # Notes dashboard
│       ├── login.html        # Login form
│       └── sign_up.html      # Registration form
└── instance/
    └── database.db           # SQLite database (auto-created)
```

## Technology Stack

- **Backend**: Flask (Python web framework) [6](#0-5) 
- **Database**: SQLite with SQLAlchemy ORM [7](#0-6) 
- **Authentication**: Flask-Login for session management [8](#0-7) 
- **Frontend**: Bootstrap 4 + jQuery for responsive UI [9](#0-8) 

## Usage

1. **Sign Up**: Create a new account with email and password
2. **Login**: Access your personal note dashboard
3. **Add Notes**: Use the textarea to create new notes [10](#0-9) 
4. **Delete Notes**: Click the delete button to remove notes instantly [11](#0-10) 

## Development

The application runs in debug mode by default for development: [12](#0-11) 

- **Auto-reload**: Code changes trigger automatic server restart
- **Network Access**: Accessible from other devices on your network (`0.0.0.0`)
- **Error Pages**: Detailed error information for debugging

## Database Schema

The application uses two main models:

- **User**: Stores user credentials and profile information [13](#0-12) 
- **Note**: Stores note content with timestamps and user relationships [14](#0-13) 

## Security Features

- User session management with Flask-Login [15](#0-14) 
- Route protection with `@login_required` decorator [16](#0-15) 
- User authorization checks for note operations [17](#0-16) 

## Contributing

1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Test thoroughly
5. Submit a pull request

## License

This project is open source and available under the MIT License.
