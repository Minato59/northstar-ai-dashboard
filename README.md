# Northstar AI Operations Dashboard

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
