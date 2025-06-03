# LangGraph Time Bot

A stateless chatbot using LangGraph and OpenAI GPT-4o that can respond to user messages and return the current UTC time when asked.

## Features

- Stateless LangGraph chat flow
- One tool: `get_current_time` — returns UTC time in ISO‑8601 format
- Uses OpenAI GPT-4o or any model that supports tool use

## Installation

Clone the repository and install dependencies:

```bash
git clone https://github.com/M4dCup/Test_Task_Korolev.git
cd Test_Task_Korolev
python -m venv .venv and source .venv/bin/activate
pip install -r requirements.txt
```

## Setup

Before running, set your OpenAI API key:

```bash
export OPENAI_API_KEY="your-api-key-here"     # Mac/Linux
set OPENAI_API_KEY="your-api-key-here"        # Windows CMD
$env:OPENAI_API_KEY="your-api-key-here"       # Windows PowerShell
```

This is required for accessing OpenAI's API.

## Run

Start the chatbot with:

```bash
langgraph dev
```
or:
```bash
python main.py
```

## Example

```
You: What time is it?
Bot: {"utc": "2025-06-03T18:04:22Z"}
```

## Notes

- No memory or database used
- Only one tool is implemented: `get_current_time`
