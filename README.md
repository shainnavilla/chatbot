# ARIA - FSUUComBot Frontend

A responsive static frontend for an AI-powered student support chatbot experience built for the FSUU (or related academic/community) context. The project includes a marketing landing page, a chatbot interface, and an admin dashboard UI.

## Project Overview

This repository contains the frontend interface for an AI assistant that can answer student and support queries using Anthropic Claude via direct API calls from the browser. It is designed as a lightweight static web app with no build setup required.

## Features

- Marketing landing page for the AI assistant
- Chatbot interface for student support questions
- Admin dashboard panel
- Mobile-responsive layout
- Tabler Icons and modern styling
- Direct Claude API integration in the browser

## Project Structure

- `index.html` — marketing landing page
- `fsuu_sco_chatbot.html` — chatbot interface
- `admin.html` — admin dashboard UI
- `css/` — frontend stylesheets
- `html/` — additional HTML resources and embedded pages
- `js/` — JavaScript assets
- `TECHSTACK.md` — technology summary

## Tech Stack

- HTML5
- CSS3
- Vanilla JavaScript
- Tabler Icons
- Google Fonts
- Anthropic Claude API (`claude-sonnet-4-6`)

## Running the Project Locally

Because this is a static frontend project, you can run it by opening the HTML files directly in a browser.

### Option 1: Open directly

- Open `index.html` in your browser for the landing page
- Open `fsuu_sco_chatbot.html` for the chatbot experience
- Open `admin.html` for the admin panel

### Option 2: Serve locally with a simple web server

From the project folder, run:

```bash
python -m http.server 8000
```

Then open:

- `http://localhost:8000/`
- `http://localhost:8000/fsuu_sco_chatbot.html`
- `http://localhost:8000/admin.html`

## Anthropic API Configuration

The chatbot currently sends requests to:

```text
https://api.anthropic.com/v1/messages
```

using the model:

```text
claude-sonnet-4-6
```

Important:

- This project is a frontend-only implementation.
- API keys and secrets should not be placed directly in client-side code for production use.
- For production deployment, it is strongly recommended to move the API call behind a secure backend server or serverless function.

## Notes

- This repository is intentionally lightweight and does not use a framework or package manager.
- The app is designed for quick deployment as a static site.
- Some generated or embedded HTML files in the `html/` folder may be legacy or reference materials and are not necessarily core app files.

## License

This project does not currently include a license file. If you plan to publish it publicly, add a license such as MIT before release.

## Recommended Next Step

Before publishing to GitHub or deploying publicly, consider:

1. Moving the Anthropic call to a secure backend
2. Adding environment configuration for API keys
3. Removing unused generated HTML files if they are not needed
4. Adding a proper `.gitignore` file
5. Creating a production deployment setup

## GitHub Setup

To push this project to GitHub:

```bash
git init
git add .
git commit -m "Initial frontend commit"
git branch -M main
git remote add origin <your-repository-url>
git push -u origin main
```

---

Built as a static AI support frontend for FSUUComBot.
