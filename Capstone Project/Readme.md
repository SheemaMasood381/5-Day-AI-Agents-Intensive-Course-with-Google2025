# AI-Powered Personal Task Manager Agent

## Problem Statement
Managing personal tasks across different platforms often becomes messy, repetitive, and time-consuming. People take notes in mobile apps, set reminders elsewhere, and manually track progress — leading to forgotten tasks, duplicated lists, and poor productivity.  

To solve this, I built an intelligent **Personal Task Manager Agent** that can understand natural language, manage tasks dynamically, and maintain persistent task storage — all powered through an agentic architecture.

---

## Why Agents?
Traditional scripts can add or list tasks, but they can't interpret user intent, decide which tool to call, or hold context across conversations.  

Agents solve this by:

- Understanding free-form user instructions
- Choosing the right action (add / complete / list tasks)
- Using tools autonomously
- Maintaining session context so the agent “remembers” ongoing tasks
- Integrating multiple sub-agents to handle different parts of the workflow  

This makes task management conversational, intelligent, and automated.

---

## What I Created
A **multi-agent architecture** using:

- Google ADK + Gemini  
- Function Tools  
- In-memory runner  
- Persistent JSON task database  

---

## Architecture Components

### Root Agent (TaskManagerAgent)
- Main controller
- Receives user messages
- Decides which tool to call
- Generates natural responses

### Task Understanding Agent
- Interprets user's task description and priority
- Ensures accurate extraction of intent

### Task Generation Agent
- Generates helpful tasks using Google Search
- Provides context-based recommendations

### Tool Functions
- `add_task(task_description, priority)`  
- `complete_task(task_description)`  
- `list_tasks()`  

Tools read/write from a persistent JSON task database.

### Sessions + In-Memory Runner
- Allows continuous conversations
- Preserves task list per user
- Mimics production-style session-based memory

### Evaluation Suite
- Implemented proper `integration.evalset.json`
- Includes test cases to validate tool usage
- Ensures the agent calls correct tools and returns expected responses

---

## Demo (How It Works)

**Example 1: Add Task**  
User: "Please add buy groceries to my tasks"  
Agent: "Added task: buy groceries with priority: medium"  
Tool called → `add_task("buy groceries", "medium")`

**Example 2: Complete Task**  
User: "Please complete buy groceries from my tasks"  
Agent: "Completed task: buy groceries"  
Tool called → `complete_task("buy groceries")`

**Example 3: List Tasks**  
User: "What tasks do I have?"  
Agent reads JSON DB and lists tasks.

---

## Implementation Details

### Task Database Layer
- JSON-based persistent database
- Helper functions to load/save user tasks
- Each task stored as:  
```json
{
  "description": "…",
  "priority": "medium",
  "completed": false
}
```

# Smart Personal Task Manager Agent

## Tool Functions
- **Add task**, **mark task complete**, **list tasks**  
- Interacts with task database and returns clean output

## Multi-Agent Structure
- **Understanding Agent**  
- **Generation Agent**  
- **Root Task Manager Agent**  

> All models powered by Gemini with retry logic.

## Sessions + Runner
- **InMemorySessionService** ensures task memory  
- **InMemoryRunner** executes agent decisions event-by-event  
- Handles asynchronous messaging

## Test Framework
- Complete evaluation dataset: `integration.evalset.json`  
- Validates tool calls, final responses, and agent correctness

## Main Execution
- Safe asynchronous execution with automatic session creation  
- **Test sequence:**  
  1. Add groceries  
  2. Complete groceries  
  3. List remaining tasks

## Future Enhancements
- Priority inference (auto-detect critical tasks)  
- Deadline understanding and reminders  
- Calendar integration (Google Calendar, Notion)  
- Better natural language extraction using chain-of-thought reasoning  
- Smart recommendations for procrastinated tasks  
- Voice-based task entry  
- Mobile-friendly UI (Streamlit / Gradio)  
- Vector-based memory instead of JSON file  
- Multi-user authentication for fully deployed app

## Author
**Sheema Masood**  
- GitHub: [@SheemaMasood381](https://github.com/SheemaMasood381)  
- Kaggle: Smart Personal Task Manager Agent Writeup

## License
This writeup has been released under the **Attribution 4.0 International (CC BY 4.0)** license.

**Citation:**  
Sheema Masood. *Smart Personal Task Manager Agent*.  
Capstone Project Writeup on Kaggle. 2025.

