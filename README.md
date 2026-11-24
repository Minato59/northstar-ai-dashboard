# Northstar AI Operations Dashboard
AI-Powered Project Operations & Workflow Automation | Northstar Commerce
Python, Gemini API, Pandas, Streamlit, GitHub, Google Colab
- Engineered and deployed an AI-assisted operations platform for project monitoring, risk detection, dependency analysis, and intelligent task escalation.
- Automated risk assessment across 5 projects and 18 tasks, identifying overdue activities, critical blockers, and forecast delays.
- Integrated LLM-powered management Q&A, automated request classification, and owner-specific actionable recommendations.
- Implemented human-in-the-loop validation, structured AI outputs, exception handling, and API failure recovery mechanisms.
- Developed an interactive, seven-page dashboard supporting data-driven decision-making and operational visibility.

Interactive Streamlit assessment prototype.

## Features

- Project health monitoring
- Task and dependency monitoring
- Owner escalation previews
- AI inbox triage results
- Live Gemini management Q&A
- Saved management Q&A fallback
- Audit and safety reporting

## Data

Uses fictional assessment data with a fixed reference
date of November 13, 2026.

The dashboard is read-only. It does not send emails,
approve requests, or update project records.

## Run locally

Install dependencies:

```bash
pip install -r requirements.txt
```

Start the application:

```bash
streamlit run app.py
```

## Gemini configuration

Create a local `.streamlit/secrets.toml` file:

```toml
GEMINI_API_KEY = "your_api_key_here"
```

Never commit this file.

For Streamlit Community Cloud, configure GEMINI_API_KEY
in the application's Secrets settings.

## Limitations

This is an assessment prototype, not a production
operations system. It does not include authentication,
role-based access, persistent review decisions, or
live company-system integrations.

Gemini responses require human verification.
API quotas may temporarily prevent live Q&A.
