# Latest AI Development Crew

A sophisticated AI crew built with CrewAI that conducts comprehensive research and generates detailed reports on cutting-edge AI developments.

## 🎯 Project Overview

As a manager overseeing AI research initiatives, I've created this automated crew to streamline our research and reporting processes. This crew consists of specialized AI agents that work together to deliver thorough, up-to-date intelligence on AI developments.

## 🤖 Meet the Team

### Senior Data Researcher
- **Role**: Topic-specific Senior Data Researcher
- **Mission**: Uncover cutting-edge developments in specified AI topics
- **Expertise**: Finding the most relevant and current information with exceptional clarity and conciseness

### Reporting Analyst
- **Role**: Topic-specific Reporting Analyst  
- **Mission**: Transform research findings into detailed, actionable reports
- **Expertise**: Converting complex data into clear, comprehensive reports that drive decision-making

## 🚀 Capabilities

### Research Task
- Conducts thorough research on specified AI topics
- Focuses on current year developments and trends
- Delivers 10 key bullet points of the most relevant findings

### Reporting Task
- Reviews and expands research findings into comprehensive reports
- Creates detailed sections for each major topic
- Outputs professional markdown-formatted reports

## 📋 Requirements

- Python 3.10-3.13
- CrewAI framework (>=0.150.0)
- Dependencies managed via uv

## 🛠 Installation

# Install dependencies
uv sync
```

## 💻 Usage

### Quick Start
```bash
# Run the crew with default settings (AI LLMs research)
uv run latest_ai_development

# Alternative command
uv run run_crew
```

### Training the Crew
```bash
uv run train
```

### Testing
```bash
uv run test
```

### Replay Previous Runs
```bash
uv run replay
```

## 🎯 Current Focus

The crew is currently configured to research **AI Large Language Models (LLMs)**, but can be easily adapted for any AI-related topic by modifying the input parameters.

## 📁 Project Structure

```
latest_ai_development/
├── src/latest_ai_development/
│   ├── crew.py              # Main crew orchestration
│   ├── main.py              # Entry point and execution logic
│   ├── config/
│   │   ├── agents.yaml      # Agent configurations
│   │   └── tasks.yaml       # Task definitions
│   └── tools/
│       └── custom_tool.py   # Custom tools and utilities
├── knowledge/               # Knowledge base and preferences
├── tests/                   # Test suite
└── pyproject.toml          # Project configuration
```

## 🔧 Customization

To research different topics, modify the `inputs` dictionary in `main.py`:

```python
inputs = {
    'topic': 'Your AI Topic Here',
    'current_year': str(datetime.now().year)
}
```

## 📊 Output

The crew generates detailed markdown reports containing:
- Executive summary of key findings
- Comprehensive analysis of current developments
- Structured sections for easy navigation
- Actionable insights for strategic planning

