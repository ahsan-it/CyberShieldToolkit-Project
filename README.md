# CyberShield Toolkit

CyberShield is a Django-based web application that brings together a set of practical cybersecurity tools in one place. It was developed as a semester project for the CY-104 Programming Fundamentals course, with each team member contributing a dedicated module to the platform.

The toolkit currently provides password validation, strong password generation, text encryption and decryption using the Caesar Cipher, and hash generation. The project is built with a focus on clean structure, simple usage, and clear separation between individual tool modules.

## Features

- **Password Validator** – Checks password strength based on length, uppercase and lowercase letters, numbers, and special characters.
- **Random Password Generator** – Generates strong, random passwords using a configurable mix of characters.
- **Caesar Cipher** – Encrypts and decrypts text using a classic shift-based cipher.
- **Hash Generator** – Converts input text into a fixed-length hash for integrity checking and security purposes.

Each tool is built as an independent module, making the project easy to extend with new tools in the future.

## Tech Stack

- **Backend:** Python, Django
- **Frontend:** HTML, CSS
- **Database:** SQLite

## Project Structure

```
cybershield/
├── config/          # Django project configuration
├── main/            # Core app (authentication, dashboard, routing)
├── tools/           # Individual security tool modules and services
├── templates/        # HTML templates for all pages
├── static/css/       # Stylesheets
├── manage.py
├── requirements.txt
└── SETUP.md
```

## Getting Started

### 1. Clone the repository

```bash
git clone https://github.com/ahsan-it/CyberShieldToolkit-Project.git
cd CyberShieldToolkit-Project
```

### 2. Install dependencies

```bash
pip install -r requirements.txt
```

### 3. Apply database migrations

```bash
python manage.py migrate
```

### 4. Run the development server

```bash
python manage.py runserver
```

The application will be available at `http://127.0.0.1:8000/`.

For additional setup details, including URL routes and instructions for adding new tools, see [SETUP.md](SETUP.md).

## Application Routes

| URL | Description |
|-----|-------------|
| `/` | Landing page |
| `/home/` | Home page (requires login) |
| `/dashboard/` | User dashboard |
| `/login/` | Login page |
| `/register/` | Registration page |
| `/logout/` | Logout |

## Team

This project was developed collaboratively by a four-member team as part of the CY-104 Programming Fundamentals semester project, under the supervision of Miss Hira Abbasi and Miss Areesha.

- Ahsan – Password and Encryption Tools
- Zunaira
- Unaiza
- Hussain

## License

This project was created for academic purposes as part of a university course assignment.
