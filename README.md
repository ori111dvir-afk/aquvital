# Aquavital Demo System

This repository contains a static browser demo for dehydration risk monitoring using Firebase Realtime Database.

## Project Requirements

The source of truth for the project requirements is `aquavital_requirements.txt`.
It describes the intended demo behavior, Firebase data structure, UI expectations, and technical constraints.

## Files

- `index.html` — landing page with navigation buttons for the patient simulator and caregiver dashboard.
- `patient.html` — patient simulator that generates readings every 3 seconds, computes a risk score, updates Firebase, and pushes alerts when risk becomes red.
- `caregiver.html` — caregiver dashboard that listens to `/readings/latest` and `/alerts`, displays live readings, risk status, and top-center alert popups.
- `aquavital_requirements.txt` — project requirements and acceptance criteria.

## Notes

- Uses Firebase via CDN scripts only.
- No frameworks, no npm, no build tools.
- Designed to run as static HTML files, suitable for GitHub Pages.
- Firebase config is embedded directly in both HTML files.

