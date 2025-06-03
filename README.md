# LangGraph Time Bot

A stateless chatbot using LangGraph and OpenAI GPT-4o that can respond to user messages and return the current UTC time when asked.

## Features

- Stateless LangGraph chat flow
- One tool: `get_current_time` — returns UTC time in ISO‑8601 format
- Uses OpenAI GPT-4o or any model that supports tool use

## Installation

Clone the repository and install dependencies:

```bash
git clone <your_repo>
cd langgraph-time-bot
python -m venv .venv && source .venv/bin/activate
pip install -r requirements.txt
```

## Setup

Before running, set your OpenAI API key:

```bash
export OPENAI_API_KEY="your-openai-key"
```

This is required for accessing OpenAI's API.

## Run

Start the chatbot with:

```bash
langgraph dev
```

## Example

```
You: What time is it?
Bot: {"utc": "2025-06-03T18:04:22Z"}
```

## Notes

- No memory or database used
- Only one tool is implemented: `get_current_time`
