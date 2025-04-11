# Advanced-AIML

# News AI Agent

An AI agent that will search the web for the top links, attempt to read and extract the text content from each of those links, analyze the gathered information based on instructions and description gives response to the topic.


---

## 🔍 Project Overview

### ✅ What It Does
- Search the web for the top links.
- Uses AI (Gemini) to conduct online research.
- Employs tools to search the web (DuckDuckGoTools) and extract content from news articles (Newspaper4kTools).
- Analyze the gathered information based on instructions and description.
- Generate a worthy output.

### 💡 Why I Made It
In today's fast-paced information environment, efficient and thorough research is crucial for journalism. This agent aims to automate the initial stages of research, allowing writers to focus on analysis, storytelling, and delivering timely news. This is a forward-thinking approach to leveraging AI in news production!

### 🌟 Unique Features
- Specialized Persona: The agent is designed with a specific persona ("senior Times of India researcher"), which likely influences the tone and style 
  of its output.
- Integrated Research Workflow: It combines web searching and content extraction into a seamless workflow.
- Leverages Powerful LLM: Utilizing the Gemini model suggests access to cutting-edge natural language processing capabilities.
- Structured Instructions: The clear list of instructions guides the agent through a well-defined research and writing process.
- Markdown Output: The markdown=True setting facilitates well-formatted and readable output.
- Transparency: Showing tool calls (show_tool_calls=True) provides insight into the agent's reasoning process.
- Contextual Awareness: Adding the datetime to instructions (add_datetime_to_instructions=True) can help the agent consider the recency of 
  information.

---

## ⚙️ How It Works

### 🧠 Technology Used
- Python, agno (AI Agent Framework), Gemini (Large Language Model), DuckDuckGoTools (Web Search), Newspaper4kTools (News Article Extraction)

### 🔁 Workflow
1. Receives a Topic: The agent is initiated with a topic (e.g., "Graphic cards").
2. Web Search: The DuckDuckGoTools are used to find the top 5 relevant links for the given topic.
3. Content Extraction: The agent attempts to use Newspaper4kTools to extract the main text content from each of the identified URLs.
4. Information Analysis: The agent analyzes the extracted information from the various sources.
5. Article Generation: Based on the analysis, the Gemini model generates a news article suitable for the Times of India.
6. Output: The generated article is printed to the console in Markdown format, along with the tool calls made during the process.
---

## 🚀 Getting Started

### 🔧 Prerequisites
- Python environment
- Installation of the agno library and its dependencies (including the specific tool requirements).
```bash
pip install agno
```
- Installing the Google Generative AI Library:
```bash
pip install google-genai
```

### 🛠️ Setting Up and Running the AI Agent Project
Here's a step-by-step explanation of the commands you've provided to set up and run your AI agent project:

- Creating and Activating a Virtual Environment:
```bash
uv venv --python 3.12 .venv\Scripts\activate
```
- Setting the Google API Key:
```bash
set GOOGLE_API_KEY=**
```
- Installing Required Python Libraries:
```bash
pip install openai duckduckgo-search newspaper4k lxml_html_clean agno
```
- Running Your AI Agent Script:
```bash
python agent_gemini.py
```
