# Multi-Agent Debate DAG using LangGraph

This project is a Jupyter Notebook (`task2.ipynb`) that uses **OpenAI's GPT models** to automatically generate **pro and con arguments** for a given debate topic.

## Features
- Generate **4 concise pro arguments** supporting a topic.
- Generate **4 concise con arguments** opposing a topic.
- Easily extensible for different models or numbers of arguments.

## Requirements
Make sure you have Python 3.8+ installed.

Install the dependencies from `requirements.txt`:
```bash
pip install -r requirements.txt
```

## Setup
1. Clone or download this repository.
2. Open the notebook
3. Set your OpenAI API Key inside the notebook:
   ```python
   import os
   os.environ["OPENAI_API_KEY"] = "your_api_key_here"
   ```
    **Important:** Never commit your API key to public repositories.

## Usage
- Run the notebook cells step by step.
- Use the provided functions:
  ```python
  generate_pro_arguments("Should AI be used in education?")
  generate_con_arguments("Should AI be used in education?")
  ```

## Example Output
```text
Pro Arguments:
1. Increases personalized learning opportunities.
2. Provides quick access to information.
3. Reduces workload for teachers.
4. Encourages innovative teaching methods.

Con Arguments:
1. Risk of over-reliance on technology.
2. Potential data privacy concerns.
3. May reduce human interaction in classrooms.
4. High implementation costs.
```

## Notes
- The project uses **GPT-4o** by default, but you can change the model to any available OpenAI model.
- You can adjust the number of arguments by modifying the code.

