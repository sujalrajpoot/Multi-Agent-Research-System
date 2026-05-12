# 🤖 Multi-Agent Research System

A modular Python research framework for experimenting with multi-agent workflows, task orchestration, and intelligent pipelines.

## 🚀 What is this project?

`Multi-Agent-Research-System` is a lightweight research system designed to help developers, researchers, and AI practitioners prototype multi-agent interactions quickly. It brings together agents, pipelines, and utility tools in a flexible structure so you can explore collaboration strategies between autonomous processes.

## 🧠 How it works

The repository is organized into key components:

- `agents.py` — defines agent logic and communication patterns.
- `app.py` — provides the main application entry point for running the system.
- `pipeline.py` — composes workflows, routes tasks, and manages agent execution.
- `tools.py` — houses reusable helper functions and utilities.
- `requirements.txt` — lists Python dependencies for setting up the environment.

The system is built to:

1. Initialize agents with distinct roles and responsibilities
2. Pass tasks through a configurable pipeline
3. Use tools to simplify data handling and agent coordination
4. Produce research-ready results while remaining easy to extend

## 💡 Why this is useful

This project can help you:

- Prototype multi-agent collaboration models
- Explore workflow orchestration for research experiments
- Validate strategies for agent communication and decision making
- Build a foundation for larger agent-based systems

## 🛠️ Getting started

### Prerequisites

- Python 3.10+ (or compatible)
- `pip` installed

### Install dependencies

```bash
pip install -r requirements.txt
```

### Setup environment variables

The system requires API keys for LLM and search functionality. Create a `.env` file in the project root with the following variables:

```bash
OPENAI_API_KEY=sk-your-openai-api-key-here
TAVILY_API_KEY=your-tavily-api-key-here
```

#### Environment Variables Reference

| Variable | Required | Purpose | Source |
|----------|----------|---------|--------|
| `OPENAI_API_KEY` | ✅ Yes | API key for OpenAI GPT models (gpt-4o-mini, gpt-4, etc.) | [OpenAI API Keys](https://platform.openai.com/api-keys) |
| `TAVILY_API_KEY` | ✅ Yes | API key for Tavily web search service | [Tavily API](https://tavily.com) |

**How to get API keys:**

1. **OpenAI API Key:**
   - Go to https://platform.openai.com/api-keys
   - Create a new API key
   - Copy and paste it into your `.env` file as `OPENAI_API_KEY`

2. **Tavily API Key:**
   - Visit https://tavily.com
   - Sign up for an account
   - Find your API key in the dashboard
   - Copy and paste it into your `.env` file as `TAVILY_API_KEY`

> ⚠️ **Security tip:** Never commit your `.env` file to version control. Add it to `.gitignore`.

### Run the app

```bash
python app.py
```

## 🌐 Use from GitHub

If this repository is hosted on GitHub, clone it and run the system locally:

```bash
git clone https://github.com/sujalrajpoot/Multi-Agent-Research-System.git
cd Multi-Agent-Research-System
pip install -r requirements.txt
python app.py
```

> If you want to customize the behavior, inspect `agents.py`, `pipeline.py`, and `tools.py`.

## 🧪 Tech stack & packages

This project is built in Python and uses the following technologies and packages:

- Python 3.10+ for the runtime environment
- `langchain` / `langchain-core` / `langchain-community` / `langchain-openai` for agent orchestration and LLM integration
- `openai` to connect with OpenAI models
- `tavily-python` for search tool integration
- `requests`, `beautifulsoup4`, `lxml`, `html5lib` for web scraping and HTML parsing
- `python-dotenv` for environment variable management
- `aiohttp` for asynchronous agent and tool execution
- `pandas` for data handling and pipeline analytics
- `tiktoken` for token counting and text utilities
- `rich` for better logging and debugging output
- `tenacity` for retry logic and robustness
- `orjson` for fast JSON serialization/deserialization
- `pydantic` for model validation and structured data support

## 📌 Suggested usage

- Add new agents with specific goals in `agents.py`
- Extend `pipeline.py` to support new task routing or scheduling logic
- Create helper functions in `tools.py` for reuse across experiments
- Use `app.py` as the launching point for your research runs

## 🧩 Recommended enhancements

Here are a few ideas for extending the system:

- Add a configuration file for agent settings
- Implement logging and result tracking
- Enable distributed or asynchronous agent execution
- Add a web dashboard or CLI for experiment control

## 🤝 Contributing

Contributions are welcome!

If you'd like to help:

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/my-agent`)  
3. Commit your changes (`git commit -m "Add new agent behavior"`)  
4. Push to your branch (`git push origin feature/my-agent`)  
5. Open a pull request

Please also consider:

- Keeping code modular and readable
- Adding comments for new agent behaviors
- Documenting pipeline changes in the README

## 📄 License

This project is licensed under the MIT License.

## ✨ Note

This project is intended as a flexible experimental foundation. Feel free to adapt the architecture to your own research goals and use it as a starting point for advanced multi-agent systems.
