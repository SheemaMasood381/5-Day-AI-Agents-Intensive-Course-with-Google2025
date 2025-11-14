# 5-Day AI Agents Intensive Course with Google (Kaggle) — 2025

Notebooks, assignments, and a capstone project from the 5-Day AI Agents Intensive Course with Google (hosted on Kaggle). This repository explores AI agent design, reasoning, and automation using Google AI tools.

---

## Key Features & Benefits

- **Hands-on Experience:** Practical exercises for designing and building AI agents.  
- **Google AI Tools:** Learn to leverage Google's cutting-edge AI technologies (e.g., Gemini).  
- **Comprehensive Curriculum:** Covers agent design, reasoning, and automation across 5 days.  
- **Real-World Applications:** Apply knowledge to solve practical problems in a capstone project.  
- **Structured Learning:** A well-organized curriculum with day-by-day notebooks and assignments.

---

## Prerequisites & Dependencies

To run the notebooks and complete the assignments:

- Python 3.6+  
- Jupyter Notebook or JupyterLab (recommended)  
- Kaggle account (course affiliation)  
- Required Python packages (install via pip):

```bash
pip install openai google-generativeai tiktoken
```

Packages used in the notebooks may include:
- `openai` — OpenAI API client (if applicable)
- `google-generativeai` — Google AI SDK for Gemini models
- `tiktoken` — Tokenization utilities

---

## API Keys

Obtain API keys for any external services used by the agents (e.g., Google AI Studio, OpenAI). Store them securely using environment variables.

Example (Linux/macOS):

```bash
export GOOGLE_API_KEY="YOUR_GOOGLE_API_KEY"
export OPENAI_API_KEY="YOUR_OPENAI_API_KEY"
```

Or add a `.env` file to the project root:

```
GOOGLE_API_KEY=YOUR_GOOGLE_API_KEY
OPENAI_API_KEY=YOUR_OPENAI_API_KEY
```

Make sure to never commit secret keys to version control.

---

## Installation & Setup

1. Clone the repository:

```bash
git clone https://github.com/SheemaMasood381/5-Day-AI-Agents-Intensive-Course-with-Google2025.git
cd 5-Day-AI-Agents-Intensive-Course-with-Google2025
```

2. Install dependencies:

If a `requirements.txt` file is provided:

```bash
pip install -r requirements.txt
```

Or install the core packages manually:

```bash
pip install openai google-generativeai tiktoken
```

3. Set up API keys (see "API Keys" above).

4. Launch Jupyter Notebook or JupyterLab and open notebooks:

```bash
jupyter notebook
# or
jupyter lab
```

Navigate to the repository folder and open the desired `.ipynb` files.

---

## Course Curriculum

Day-by-day notebooks:

- **Day 1 — Foundations**
  - `ai-agents-day-1a-from-prompt-to-action.ipynb`
  - `ai-agents-day-1b-agent-architectures.ipynb`

- **Day 2 — Tools & Best Practices**
  - `ai-agents-day-2a-agent-tools.ipynb`
  - `ai-agents-day-2b-agent-tools-best-practices.ipynb`

- **Day 3 — Sessions & Memory**
  - `ai-agents-day-3a-agent-sessions.ipynb`
  - `ai-agents-day-3b-agent-memory.ipynb`

- **Day 4 — Observability & Evaluation**
  - `ai-agents-day-4a-agent-observability.ipynb`
  - `ai-agents-day-4b-agent-evaluation.ipynb`

- **Day 5 — Multi-Agent Systems**
  - `ai-agents-day-5a-agent2agent-communication.ipynb`

Each notebook contains code examples, explanations, and hands-on exercises.

---

## Usage Examples & API Documentation

Refer to individual notebooks for:
- Code examples and explanations
- Hands-on exercises
- Best practices and tips
- Integration guidance for Google AI and OpenAI APIs

Notebooks typically include code cells showing how to configure models, call APIs, and run agent pipelines.

---

## Configuration Options

Common configurations (set within notebooks or as environment variables):

- API Keys: Use environment variables (see above).  
- Model Selection: Choose between models (e.g., Gemini family, GPT-3.5, GPT-4) as supported by the SDKs.  
- Hyperparameters: Tune agent behavior with options such as:
  - `temperature` — controls randomness/creativity
  - `top_p` — nucleus sampling for diversity
  - Other model-specific parameters

---

## Capstone Project

The capstone ties together the concepts from the 5 days into a practical project. See the capstone notebook and assignment(s) for requirements, dataset(s), and evaluation criteria.

---

## Contributing

We welcome contributions!

1. Fork the repository  
2. Create a feature branch:

```bash
git checkout -b feature/your-feature-name
```

3. Make your changes and document them.  
4. Submit a pull request with a clear description.

Please follow the existing coding style and include documentation for any new features.

---

## License

This repository is licensed under the Apache License, Version 2.0.

For the full license text, see the `LICENSE` file or visit: https://www.apache.org/licenses/LICENSE-2.0

Copyright © 2025 Google LLC

---

## Acknowledgments

This repository is based on the 5-Day AI Agents Intensive Course with Google (Kaggle). We gratefully acknowledge Google and Kaggle for providing the course materials, curriculum, and resources.

---

## Contact & Licensing Inquiries

For questions regarding licensing or usage rights, contact: SheemaMasood381

Happy Learning! 🚀
