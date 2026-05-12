# Getting Started with GitHub Copilot

<img src="https://octodex.github.com/images/Professortocat_v2.png" align="right" height="200px" />

This sample project is a simple FastAPI application that serves a static frontend and provides an API for viewing and signing up for extracurricular activities.

## Prerequisites

- Python 3.9+ installed
- `pip` available

## Quick Start

1. Open a terminal in the project root.
2. Create and activate a virtual environment:

   ```bash
   python -m venv .venv
   source .venv/bin/activate
   ```

3. Install the dependencies:

   ```bash
   pip install -r requirements.txt
   ```

4. Start the app:

   ```bash
   python -m uvicorn src.app:app --reload --host 0.0.0.0 --port 8000
   ```

5. Open the app in your browser:

   - Frontend: `http://127.0.0.1:8000`
   - API docs: `http://127.0.0.1:8000/docs`

## Project Structure

- `src/app.py` — FastAPI application and route definitions
- `src/static/` — static frontend assets served by FastAPI
- `requirements.txt` — Python dependencies

## Usage

- `GET /activities` — list all activities
- `POST /activities/{activity_name}/signup?email=you@example.com` — sign up for an activity

---

&copy; 2025 GitHub &bull; [Code of Conduct](https://www.contributor-covenant.org/version/2/1/code_of_conduct/code_of_conduct.md) &bull; [MIT License](https://gh.io/mit)

