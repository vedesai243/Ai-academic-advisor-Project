

# AI Academic Advisor

A simple, interactive AI-powered academic advisor built using **Python**.  
The application uses **Anthropic’s Claude** via **LangChain** to answer academic planning questions, with support for web search and Wikipedia lookups.

---

## Features

- Answers academic planning questions using AI
- Focused on UW Computer Science and WLU BBA (Double Degree)
- Uses external tools for real-time information:
  - DuckDuckGo web search
  - Wikipedia summaries
- Returns structured responses using Pydantic
- Saves responses to a text file with timestamps

---

## Technologies Used

- **Python** – core application logic
- **LangChain** – agent framework
- **Anthropic Claude 3.5 Sonnet** – large language model
- **Pydantic** – structured output validation
- **DuckDuckGo Search** – web search
- **Wikipedia API** – factual lookups
- **python-dotenv** – environment variable management

---

## How It Works

- On startup, the program loads the Anthropic API key from `apikey.env`.
- A LangChain agent is initialized with access to search, Wikipedia, and file-saving tools.
- The user enters an academic question through the command line.
- The agent selects the appropriate tools to gather relevant information.
- The final response is generated in a structured format and saved for reference.

---

## Setup

Install dependencies:
```bash
pip install -r requirements

Create an apikey.env file and add your Anthropic API key:
ANTHROPIC_API_KEY=your_api_key_here


