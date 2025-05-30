# Express Sentry Integration Demo

## Overview
Node.js Express app with basic Sentry setup and error trigger route.

## Setup

```bash
git clone https://github.com/yourname/sentry-integration-demos.git
cd sentry-integration-demos/express-sentry-demo
npm install

Update index.js:
Sentry.init({ dsn: 'YOUR_DSN_HERE' });

Run the app:
node index.js

Visit to trigger error:
http://localhost:3000/debug-sentry
