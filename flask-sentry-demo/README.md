## flask-sentry-demo/README.md

```markdown
# Flask Sentry Integration Demo

## Overview
Python Flask app with Sentry integration and route to trigger errors.

## Setup

```bash
git clone https://github.com/yourname/sentry-integration-demos.git
cd sentry-integration-demos/flask-sentry-demo
python -m venv venv
venv\Scripts\activate  # Windows
pip install flask sentry-sdk

Update app.py:
sentry_sdk.init(
    dsn="YOUR_DSN_HERE",
    integrations=[FlaskIntegration()],
    traces_sample_rate=1.0
)

Run:
flask run

Vist:
http://localhost:5000/debug-sentry
