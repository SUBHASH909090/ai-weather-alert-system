# AI Weather Alert System

An AI-powered weather monitoring and alert generation workflow built using **n8n and Google Gemini**.

The system processes weather information, evaluates weather conditions using AI, assigns an alert severity level, and generates recommended actions.

## Workflow Architecture

`Weather Data → AI Agent (Google Gemini) → Structured Weather Analysis → Severity-Based Alert`

## Features

* Processes weather information automatically.
* Analyses temperature, rainfall, and wind speed.
* Classifies weather severity into four levels:

  * Normal
  * Advisory
  * Warning
  * Critical
* Generates explanations for weather conditions.
* Recommends appropriate actions based on severity.
* Produces structured JSON output.

## Technologies Used

* n8n — Workflow automation
* Google Gemini — AI-powered weather analysis
* Structured JSON — Weather assessment output

## Output Fields

| Field              | Description                            |
| ------------------ | -------------------------------------- |
| severity           | Normal, Advisory, Warning, or Critical |
| temperature        | Temperature value                      |
| rainfall_mm        | Rainfall measurement                   |
| wind_speed_kmh     | Wind speed                             |
| weather_condition  | Weather description                    |
| reason             | Explanation for the alert              |
| recommended_action | Suggested action                       |

## Project Screenshots

### Workflow

![Workflow](screenshots/workflow.png)

### Weather Analysis

![Weather Analysis](screenshots/weather-analysis.png)

### Alert Output

![Alert Output](screenshots/alert-output.png)

## Setup Instructions

1. Download the workflow JSON from the `workflow` folder.
2. Import it into your n8n instance.
3. Configure the required API credentials.
4. Configure the weather data source used by the workflow.
5. Execute the workflow and inspect the generated alert.

## What I Learned

* Building automated workflows using n8n.
* Integrating AI models into automation systems.
* Designing structured JSON outputs.
* Implementing severity-based decision logic.
* Generating actionable AI-powered alerts.

## Disclaimer

This project is a portfolio demonstration, not an official weather-warning service. AI-generated assessments should not replace alerts from authorised meteorological agencies.
