# 5-Day AI Agents Intensive Course with Google (Kaggle) — 2025

A comprehensive repository containing notebooks, assignments, and a capstone project from the **5-Day AI Agents Intensive Course with Google** hosted on Kaggle. This course explores AI agent design, reasoning, automation, and real-world applications using Google's cutting-edge AI tools.

---

## 📚 Course Overview

This repository documents a complete learning journey through AI agents:

- **Day 1**: Foundations & Agent Architectures
- **Day 2**: Tools & Best Practices
- **Day 3**: Sessions & Memory Management
- **Day 4**: Observability & Evaluation
- **Day 5**: Multi-Agent Communication Systems
- **Capstone**: AI-Powered Task Manager Agent

---

## 🎯 Key Features

✅ **Hands-on Experience** — Practical exercises for designing and building AI agents  
✅ **Google AI Tools** — Learn Gemini, Google ADK, and integrated APIs  
✅ **Structured Curriculum** — 5-day progression with daily notebooks and assignments  
✅ **Real-World Application** — Capstone project applying all learned concepts  
✅ **Production-Ready Code** — Sessions, runners, evaluation frameworks, and persistent storage  

---

## 📋 Prerequisites

- **Python** 3.8+
- **Jupyter Notebook** or JupyterLab
- **Kaggle Account** (for course affiliation)
- **API Keys** (Google AI, OpenAI if applicable)

---

## 🔧 Installation & Setup

### 1. Clone the Repository

```bash
git clone https://github.com/SheemaMasood381/5-Day-AI-Agents-Intensive-Course-with-Google2025.git
cd 5-Day-AI-Agents-Intensive-Course-with-Google2025
```
### 2. Install Dependencies

```bash
pip install -r requirements.txt
```

Or install core packages manually:
```bash
pip install google-generativeai openai tiktoken python-dotenv
```

### 3. Configure API Keys
Create a .env file in the project root:

```
GOOGLE_API_KEY=YOUR_GOOGLE_API_KEY
OPENAI_API_KEY=YOUR_OPENAI_API_KEY
```
Linux/macOS alternative:
```bash
export GOOGLE_API_KEY="YOUR_GOOGLE_API_KEY"
export OPENAI_API_KEY="YOUR_OPENAI_API_KEY"
```
⚠️ Make sure to never commit secret keys to version control.

### 4. Launch Jupyter
```bash
jupyter notebook
# or
jupyter lab

```
---
## 📂 Repository Structure
5-Day-AI-Agents-Intensive-Course-with-Google2025/
│
├── README.md                                          # This file
├── requirements.txt                                   # Python dependencies
│
├── Day-1-Foundations/
│   ├── ai-agents-day-1a-from-prompt-to-action.ipynb
│   └── ai-agents-day-1b-agent-architectures.ipynb
│
├── Day-2-Tools-and-Best-Practices/
│   ├── ai-agents-day-2a-agent-tools.ipynb
│   └── ai-agents-day-2b-agent-tools-best-practices.ipynb
│
├── Day-3-Sessions-and-Memory/
│   ├── ai-agents-day-3a-agent-sessions.ipynb
│   └── ai-agents-day-3b-agent-memory.ipynb
│
├── Day-4-Observability-and-Evaluation/
│   ├── ai-agents-day-4a-agent-observability.ipynb
│   └── ai-agents-day-4b-agent-evaluation.ipynb
│
├── Day-5-Multi-Agent-Systems/
│   └── ai-agents-day-5a-agent2agent-communication.ipynb
│
├── Capstone-Project/
│   ├── ai-powered-task-manager-capstone-project.ipynb
│   ├── task_database.json                             # Persistent task storage
│   ├── integration.evalset.json                       # Evaluation test cases
│   └── CAPSTONE_WRITEUP.md                            # Project documentation
│
├── .env.example                                       # Template for API keys
└── LICENSE                                            # Apache 2.0 License


## Course Curriculum

# Course Curriculum

## Day 1 — Foundations

**ai-agents-day-1a-from-prompt-to-action.ipynb**  
Understanding agent loops and prompt-to-action pipelines

**ai-agents-day-1b-agent-architectures.ipynb**  
Exploring different agent design patterns


## Day 2 — Tools & Best Practices

**ai-agents-day-2a-agent-tools.ipynb**  
Creating and integrating custom tools

**ai-agents-day-2b-agent-tools-best-practices.ipynb**  
Tool design patterns and error handling


## Day 3 — Sessions & Memory

**ai-agents-day-3a-agent-sessions.ipynb**  
Managing agent sessions and state

**ai-agents-day-3b-agent-memory.ipynb**  
Memory architectures: in-memory, vector-based, persistent


## Day 4 — Observability & Evaluation

**ai-agents-day-4a-agent-observability.ipynb**  
Logging, tracing, and monitoring agents

**ai-agents-day-4b-agent-evaluation.ipynb**  
Building evaluation frameworks and test suites


## Day 5 — Multi-Agent Systems

**ai-agents-day-5a-agent2agent-communication.ipynb**  
Agent-to-agent communication and coordination

## Capstone: AI-Powered Task Manager
**ai-powered-task-manager-capstone-project.ipynb — Full-stack multi-agent task management system**

---

##  Capstone Project

# Production-Ready Multi-Agent System for Intelligent Task Management

## Architecture

- **Root Task Manager Agent**
  - **Task Understand Agent**
  - **Task Generation Agent**
    - **Tool Functions**
      - `add_task()`
      - `complete_task()`
      - `list_tasks()`
    - **Task Database** (JSON / Persistent)
-----


## Features

- **Natural Language Understanding** — Parse free-form user inputs  
- **Multi-Agent Coordination** — Specialized agents for understanding, generation, and management  
- **Persistent Storage** — JSON-based task database  
- **Session Management** — Maintains conversation context across interactions  
- **Tool Integration** — Custom functions for task CRUD operations  
- **Evaluation Framework** — Complete test suite with evalset validation  

## Quick Demo

# User: "Add buy groceries to my tasks"
# Agent → calls add_task("buy groceries", "medium")
# Response: "Added task: buy groceries with priority: medium"

# User: "Complete buy groceries"
# Agent → calls complete_task("buy groceries")
# Response: "Completed task: buy groceries"

# User: "Show my tasks"
# Agent → calls list_tasks()
# Response: [lists all active tasks]


## Technologies Used

- **Gemini 2.5 Flash Lite** — LLM backbone  
- **Google ADK** — Agent framework  
- **InMemorySessionService** — Session management  
- **InMemoryRunner** — Event-based execution  
- **Function Tools** — Custom tool definitions  
- **JSON Database** — Persistent storage  


## Usage Examples

### Running a Notebook
```bash
jupyter notebook ai-agents-day-1a-from-prompt-to-action.ipynb

```

### Running the Capstone Project
```bash
jupyter notebook Capstone-Project/ai-powered-task-manager-capstone-project.ipynb
```

## Configuration

Notebooks allow customization of:

- **Model Selection** — Choose Gemini model variants  
- **Temperature** — Controls creativity (0.0 to 1.0)  
- **Top-P** — Nucleus sampling for diversity  
- **Max Tokens** — Response length limits  
- **Tool Behavior** — Error handling and retries  

---
## Evaluation & Testing

The capstone includes a comprehensive **integration.evalset.json** with:

- **Tool call validation**
- **Response correctness checks**
- **Multi-turn conversation tests**
- **Edge case handling**
- **Agent robustness validation**

Run evaluation within the capstone notebook to validate agent behavior across scenarios.

---

## Key Technologies

| Technology                    | Purpose                         |
|------------------------------|---------------------------------|
| Google Generative AI SDK     | Gemini model access             |
| Google ADK                   | Agent framework                 |
| Python 3.8+                  | Programming language            |
| Jupyter                      | Interactive notebooks           |
| JSON                         | Data persistence                |
| asyncio                      | Async execution                 |

---

## Learning Outcomes

After completing this course, you will understand:

- **Agent design patterns and architectures**
- **Tool creation and integration**
- **Session and memory management**
- **Agent evaluation and testing frameworks**
- **Multi-agent communication and coordination**
- **Building production-ready agent systems**

---

## Contributing

Contributions are welcome! To contribute:

1. **Fork the repository**
2. Create a feature branch:
   ```bash
   git checkout -b feature/your-feature-name
   ```
3. Commit your changes with clear messages
4. Push to your fork
5. Submit a pull request

Please follow existing code style and document new features.
-----

## License

This repository is licensed under the **Apache License 2.0**.  
See the LICENSE file for full details.

© 2025 Google LLC

---

## Acknowledgments

- **Google & Kaggle** — for the 5-Day AI Agents Intensive Course  
- **Course Instructors** — for guidance and curriculum design  
- **Community** — for feedback and contributions  

---

## Author

**Sheema Masood**

- **GitHub:** @SheemaMasood381  
- **Kaggle:** Smart Personal Task Manager Agent Writeup  

---

## Contact & Support

- **Email:** SheemaMasood381  
- **GitHub Issues:** Create an issue on the repository
