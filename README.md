# CyberShield AI Web Server

This project is a simple, multi-page business website for a fictional AI security consultancy, "CyberShield AI," built using the Flask web framework. It is designed to run on a Raspberry Pi 5.

## Getting Started

To run this project locally, follow these steps:

1.  **Clone the repository:**
    ```bash
    git clone [https://github.com/bwhi491/barrywhitehead-site.git](https://github.com/bwhi491/barrywhitehead-site.git)
    ```
2.  **Navigate to the project directory:**
    ```bash
    cd barrywhitehead-site
    ```
3.  **Create and activate a virtual environment:**
    ```bash
    python3 -m venv .venv
    source .venv/bin/activate
    ```
4.  **Install dependencies:**
    ```bash
    pip install Flask gunicorn
    ```

## Running the Server

* **Development Mode (for testing):**
    ```bash
    python3 app.py
    ```
* **Production Mode (for deployment):**
    ```bash
    gunicorn --bind 0.0.0.0:5000 app:app
    ```

## Project Structure

- `app.py`: The main Flask application, containing all routes and server logic.
- `templates/`: Contains all the HTML files for the website pages.
  - `base.html`: The main layout file.
  - `home.html`, `about.html`, etc.: Specific page content.
- `.venv/`: The virtual environment for Python dependencies.
- `.gitignore`: Specifies files and folders to be ignored by Git.

## Key Learnings

- Setting up a web server on a Raspberry Pi.
- Using Git and GitHub for version control.
- Managing Python dependencies with a virtual environment.
- Debugging common Flask errors like `500 Internal Server Error`.