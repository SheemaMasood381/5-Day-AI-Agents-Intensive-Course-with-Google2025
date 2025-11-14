# 5-Day-AI-Agents-Intensive-Course-with-Google2025

Notebooks, assignments, and capstone project from the 5-Day AI Agents Intensive Course with Google (Kaggle) — exploring AI agent design, reasoning, and automation using Google AI tools.

## Key Features & Benefits

*   **Hands-on Experience:** Gain practical experience in designing and building AI agents.
*   **Google AI Tools:** Learn to leverage Google's cutting-edge AI technologies.
*   **Comprehensive Curriculum:** Covers agent design, reasoning, and automation.
*   **Real-World Applications:** Apply your knowledge to solve practical problems with a capstone project.
*   **Structured Learning:** Follow a well-organized curriculum spread over 5 days.

## Prerequisites & Dependencies

To successfully run the notebooks and complete the assignments in this repository, you'll need the following:

*   **Python 3.6+:**  Ensure you have Python installed on your system.
*   **Jupyter Notebook/Lab:** Recommended for running and interacting with the notebooks.
*   **Kaggle Account:**  A Kaggle account is required, as the course is affiliated with Kaggle.
*   **Required Python Packages:** Install the following packages using pip:

    ```bash
    pip install openai google-generativeai  tiktoken
    ```

    *   `openai`: OpenAI API for interacting with GPT models (if applicable).
    *   `google-generativeai`: Google AI SDK for Gemini models.
    *   `tiktoken`: For tokenization (if applicable).
*   **API Keys:** Obtain API keys for any external services utilized by the agents (e.g., Google AI Studio, OpenAI). Store these keys securely, preferably using environment variables.

## Installation & Setup Instructions

1.  **Clone the Repository:**
    ```bash
    git clone https://github.com/SheemaMasood381/5-Day-AI-Agents-Intensive-Course-with-Google2025.git
    cd 5-Day-AI-Agents-Intensive-Course-with-Google2025
    ```

2.  **Install Dependencies:**
    ```bash
    pip install -r requirements.txt  #If a requirements.txt file is available
    # Otherwise, install dependencies as mentioned above
    # pip install openai google-generativeai tiktoken
    ```

3.  **Set Up API Keys:**
    *   Obtain the necessary API keys (Google AI Studio, OpenAI, etc.).
    *   Set environment variables to securely store your API keys. For example:

        ```bash
        export GOOGLE_API_KEY="YOUR_GOOGLE_API_KEY"
        export OPENAI_API_KEY="YOUR_OPENAI_API_KEY"
        ```

        You can also set these in your notebook or `.env` file.

4.  **Open Notebooks:**
    Launch Jupyter Notebook or JupyterLab:
    ```bash
    jupyter notebook
    # or
    jupyter lab
    ```
    Navigate to the cloned repository and open the desired notebook (`.ipynb`) file.

## Usage Examples & API Documentation

Refer to the individual notebooks for detailed usage examples and API documentation specific to each task:

*   `ai-agents-day-1a-from-prompt-to-action.ipynb`:  Introduction to AI agents and prompt engineering.
*   `ai-agents-day-1b-agent-architectures.ipynb`: Exploring different agent architectures.
*   `ai-agents-day-2a-agent-tools.ipynb`: Utilizing tools within AI agents.
*   `ai-agents-day-2b-agent-tools-best-practices.ipynb`: Best practices for agent tool usage.
*   `ai-agents-day-3a-agent-sessions.ipynb`: Managing agent sessions.
*   `ai-agents-day-3b-agent-memory.ipynb`: Implementing agent memory.
*   `ai-agents-day-4a-agent-observability.ipynb`: Monitoring and debugging agents.
*   `ai-agents-day-4b-agent-evaluation.ipynb`: Evaluating agent performance.
*   `ai-agents-day-5a-agent2agent-communication.ipynb`: Exploring communication between multiple agents.

Inside each notebook, you'll find code examples, explanations, and exercises to guide you through the material.

## Configuration Options

Most configurations are done directly within the notebooks themselves. However, the following aspects can be configured:

*   **API Keys:**  As mentioned previously, API keys should be set as environment variables.
*   **Model Selection:** Many notebooks allow you to choose between different models (e.g., Gemini, GPT-3.5, GPT-4).  Refer to the notebook's documentation for instructions on how to specify the desired model.
*   **Hyperparameters:** Experiment with different hyperparameters within the notebooks to optimize agent performance (e.g., temperature, top\_p).

## Contributing Guidelines

We welcome contributions to this repository! If you find any issues or have suggestions for improvements, please feel free to:

1.  **Fork the repository.**
2.  **Create a new branch for your feature or bug fix.**
3.  **Make your changes.**
4.  **Submit a pull request.**

Please ensure your code is well-documented and follows the existing coding style.

## License Information

License not specified. All rights reserved unless otherwise noted.
Contact [SheemaMasood381](mailto:your-email@example.com) for licensing inquiries.

## Acknowledgments

This repository is based on the 5-Day AI Agents Intensive Course with Google (Kaggle). We thank Google and Kaggle for providing the course materials and resources.
