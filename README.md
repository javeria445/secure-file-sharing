# Secure File Sharing System

A secure web-based file sharing system that provides encrypted file storage, controlled file access, user authentication, and QR-code-based file sharing.

## Overview

The Secure File Sharing System is designed to provide a safer way of storing and sharing files through a web application.

The system uses encryption to protect uploaded files and provides controlled access through generated sharing tokens and QR codes. Users can register and log in, upload files, generate secure sharing links/QR codes, and manage access to their shared files.

## Features

- User registration and authentication
- Secure password hashing
- Encrypted file storage
- File upload and download
- QR-code-based file sharing
- Token-based file access
- Password-protected file access
- File ownership and access control
- Ability to revoke file access
- Tracking of file access activity
- Web-based user dashboard
- Account management

## Technologies Used

- **Python**
- **Flask**
- **HTML/CSS**
- **PyCryptodome**
- **QRCode**
- **Pillow**
- **Werkzeug**

## Project Structure

```text
secure-file-sharing/
│
├── app.py
├── qr_generator.py
├── requirements.txt
├── README.md
├── .gitignore
│
├── templates/
│   ├── access_password.html
│   ├── access_verify.html
│   ├── account.html
│   ├── dashboard.html
│   ├── index.html
│   ├── login.html
│   └── register.html
│
├── uploads/
│   └── .gitkeep
│
└── qr_codes/
    └── .gitkeep
```

## Installation

### 1. Clone the Repository

```bash
git clone https://github.com/YOUR-USERNAME/secure-file-sharing.git
cd secure-file-sharing
```

### 2. Create a Virtual Environment

```bash
python -m venv venv
```

Activate it on Windows:

```bash
venv\Scripts\activate
```

Activate it on Linux/macOS:

```bash
source venv/bin/activate
```

### 3. Install Dependencies

```bash
pip install -r requirements.txt
```

## Running the Application

Start the Flask application with:

```bash
python app.py
```

The application will start locally and can be accessed through the URL displayed in the terminal.

## Security Considerations

This project demonstrates several security concepts, including:

- Password hashing
- Symmetric encryption
- Authentication and authorization
- Token-based access control
- Controlled file sharing
- Access revocation
- Secure handling of application secrets

Runtime data such as user records, generated tokens, encryption keys, uploaded files, and generated QR codes should not be committed to the repository.

## Files Excluded from Git

The following runtime and sensitive files/directories are intentionally excluded from the repository:

```text
users.json
qr_tokens.json
uploads/
qr_codes/
__pycache__/
.env
```

These files may contain user information, access tokens, encryption keys, uploaded files, or generated QR codes and should remain local.

## Disclaimer

This project was developed for educational and academic purposes to demonstrate secure file-sharing concepts and practical cybersecurity techniques.

## Author

**Javeria Anis**

BS Cyber Security  
COMSATS University Islamabad
