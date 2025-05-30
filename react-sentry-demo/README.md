## react-sentry-demo/README.md

```markdown
# React Sentry Integration Demo

## Overview
React app that integrates Sentry and allows triggering a sample error via button click.

## Setup

```bash
git clone https://github.com/yourname/sentry-integration-demos.git
cd sentry-integration-demos/react-sentry-demo
npm install

In src/index.js:
Sentry.init({ dsn: 'YOUR_DSN_HERE' });

Run:
npm start

Use the UI to trigger an error.

Make sure Android Studio, Java SDK, and platform tools are installed. Set up AVD and JAVA_HOME.

Run app:
npx react-native run-android

