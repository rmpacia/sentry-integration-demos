## sentry-troubleshooting.md


# Sentry Integration — Troubleshooting Reference

## React (Web)
- Blank screen: Missing render code or incorrect component structure.
- No events in Sentry: Ensure DSN is correct; try private browser window.
- Missing dependencies: Install with npm as needed (`npm install ajv`).

## Flask (Python)
- Activation issues: Use `venv\Scripts\activate` on Windows.
- pip not recognized: Ensure Python added to system PATH.

## Express (Node.js)
- requestHandler undefined: Downgraded to @sentry/node@7.92.0.
- Middleware order matters: Sentry middleware should wrap around all logic.

## React Native (Android)
- adb not found: Install Android SDK, add to PATH.
- JAVA_HOME not set: Define environment variable to JDK install.
- SDK issues: Create `local.properties` with `sdk.dir` entry.
- App deploy failures: Use `adb uninstall` or reset emulator.

## Validation Checklist
- [x] Correct DSN
- [x] Error-triggering tested
- [x] Event appears in dashboard
- [x] App runs and builds successfully
- [x] Network or log output confirms delivery
