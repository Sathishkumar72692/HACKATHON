# JH-RESOLVE — Jharkhand Resilience Network

Hackathon-ready prototype for a Statewide Collaborative Disaster Resilience Network.

## Core journey
Citizen report → smart priority/tagging → n8n workflow → university routing → industry support → government oversight.

## Run
Open `index.html` in a browser. For best results, serve the folder with any static server (VS Code Live Server is enough).

This prototype uses browser `localStorage` as a shared demo datastore. It also includes a configurable n8n webhook field and a simulated IoT telemetry panel.

## Pages
- `index.html` — role selection / landing page
- `citizen.html` — report a disaster challenge
- `student.html` — claim and manage capstone projects
- `industry.html` — pledge funding, mentorship or hardware
- `government.html` — state command center

## n8n
Set the webhook URL in Government → Automation Settings. The frontend sends a JSON payload when a new challenge is created. A real deployment should place authentication and a backend API in front of n8n.

## IoT
The IoT simulator generates ESP32-style telemetry. A water-level threshold can automatically create a challenge in the demo datastore.
