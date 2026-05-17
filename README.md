# ai-bootcamp

# FlowPilot AI — Workflow Automation Intake Assistant

FlowPilot AI is an AI-powered workflow automation intake assistant built as part of my 30-Day AI Systems Engineering Bootcamp.

The goal of this project is to help users describe a manual workflow and receive a structured analysis of how that process can be improved, digitized, or automated. The system is designed to identify current-state steps, bottlenecks, automation opportunities, recommended tools, risk checks, and estimated time savings.

## Why I Am Building This

I am building this project to strengthen my skills in AI systems engineering, workflow automation, prompt engineering, API integration, and solution architecture.

This project is also aligned with the type of work done by an AI Solutions Architect: working with subject matter experts, understanding manual processes, identifying bottlenecks, designing practical automation solutions, and communicating technical recommendations to both technical and non-technical stakeholders.

## Project Vision

By the end of the bootcamp, FlowPilot AI will allow a user to enter a workflow such as:

> A scientist receives assay result files by email, copies values into Excel, manually checks formatting, sends the file to QA for approval, and uploads the final document to a shared folder.

The system will return a structured response such as:

- Current workflow summary
- Key bottlenecks
- Automation opportunities
- Recommended tools
- AI vs rule-based automation recommendation
- Risk and quality checks
- Estimated time saved
- Future-state workflow suggestion

## Example Use Case

A product development or lab operations team may have a manual workflow like:

1. Receive experiment or assay result files by email
2. Copy values into an Excel tracker
3. Manually validate formatting
4. Send the file to QA for review
5. Wait for approval
6. Upload the final document to a shared location

FlowPilot AI would analyze the workflow and suggest improvements such as:

- Use Python scripts to extract data from files
- Add rule-based validation for formatting checks
- Use a FastAPI endpoint to submit and track workflow requests
- Use an LLM to summarize issues and generate review notes
- Track time saved before and after automation

## Core Features

### Module 1 — Environment Setup

- Create GitHub repository
- Set up Python environment
- Create `.env` and `.gitignore`
- Install FastAPI
- Run a basic FastAPI Hello World application

### Planned Features

- FastAPI backend
- Workflow analysis endpoint
- LLM-powered workflow evaluation
- Prompt templates for structured recommendations
- Basic ROI and time-saved calculator
- Risk and quality review section
- Simple frontend or API documentation page
- Public deployment URL

## Tech Stack

- Python 3.11+
- FastAPI
- Uvicorn
- Anthropic Claude API
- dotenv
- GitHub
- Future deployment: Render, Railway, or similar platform

## API Plan

### `GET /`

Returns a basic health check.

```json
{
  "message": "FlowPilot AI is running"
}
