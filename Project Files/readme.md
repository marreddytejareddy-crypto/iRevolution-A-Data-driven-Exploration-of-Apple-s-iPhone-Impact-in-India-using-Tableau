# Project Files: iRevolution Flask App

<div align="center">
  <a href="../Document/readme.md">
    <img src="https://img.shields.io/badge/Read_Documentation-Project_Insights-000000?style=for-the-badge&logo=readdotcv&logoColor=white" alt="Read Documentation" />
  </a>
</div>

This folder contains the core source code for the "iRevolution" Flask web application, an interactive platform built to seamlessly embed and showcase Tableau dashboards detailing Apple's impact in India.

## Folder Structure

The application is structured into clearly separated layers to ensure maintainability and separation of concerns:

- `app.py`: The main entry point and routing file for the Flask Python backend. It defines standard `home`, `dashboard`, and `story` endpoints.
- `requirements.txt`: Contains all vital Python dependencies needed to construct and run the environment, specifically `Flask`.
- `templates/`: Contains all Jinja HTML templates structurally serving the content.
  - `base.html`: The root layout shared across all specific views containing standard `head` metadata and standard application navigation.
  - `index.html`: The sleek, Apple-inspired landing page offering paths into specific analytical branches of the project.
  - `dashboard.html`: Securely embeds the analytical dashboard components directly from Tableau Public through the V3 Embedded JavaScript API.
  - `story.html`: Securely embeds the chronological data story components from Tableau Public.
- `static/css/style.css`: Features all customized utility styling utilizing CSS variables and an inherently responsive layout. It features deep layout optimization to accurately portray embedded iframes at 100% dimensions across various viewports.

## Running Locally

To start the Flask development server on a local machine, simply run:

```bash
pip install -r requirements.txt
python app.py
```

Then visit `http://localhost:5000` or `http://127.0.0.1:5000` via a web browser.
