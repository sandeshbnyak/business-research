# ResearchMind – Multi-Agent AI Research System

ResearchMind is an intelligent multi-agent research platform built with LangChain and Streamlit. It orchestrates multiple specialized AI agents to autonomously research a topic, gather information from the web, analyze content, generate a structured report, and critique the final output.

## Overview

ResearchMind simulates a collaborative research workflow using four AI-powered agents:

1. **Search Agent** – Finds relevant information from the web.
2. **Reader Agent** – Scrapes and extracts detailed content from discovered sources.
3. **Writer Chain** – Synthesizes findings into a comprehensive research report.
4. **Critic Chain** – Reviews the report and provides quality feedback and scoring.

The system transforms a simple research query into a polished research document with minimal user intervention.

---

## Features

* Multi-agent architecture using LangChain
* Autonomous web research workflow
* Web scraping and content extraction
* AI-generated structured research reports
* Automated report evaluation and scoring
* Streamlit-based interactive interface
* Support for Groq or OpenAI LLMs
* Modular and extensible design

---

## System Architecture
<img width="1536" height="1024" alt="image" src="https://github.com/user-attachments/assets/3d486c65-3b32-4bfc-97c4-ce5e7ab380c4" />

```text
User Query
     │
     ▼
┌───────────────┐
│ Search Agent  │
└───────┬───────┘
        │
        ▼
┌───────────────┐
│ Reader Agent  │
└───────┬───────┘
        │
        ▼
┌───────────────┐
│ Writer Chain  │
└───────┬───────┘
        │
        ▼
┌───────────────┐
│ Critic Chain  │
└───────┬───────┘
        │
        ▼
 Final Research Report
```

---

## Project Structure

```text
ResearchMind/
│
├── app.py                  # Streamlit application
├── agents.py               # Agent definitions and chains
├── tools.py                # Search and scraping tools
├── requirements.txt        # Dependencies
├── .env                    # API keys (not committed)
├── README.md
│
├── data/
│   └── research_outputs/
│
└── assets/
    └── screenshots/
```

---

## Installation

### Clone Repository

```bash
git clone https://github.com/sandeshbnyak/business-research.git
cd business-research
```

### Create Virtual Environment

```bash
python -m venv venv
```

### Activate Environment

Windows:

```bash
venv\Scripts\activate
```

Linux/Mac:

```bash
source venv/bin/activate
```

### Install Dependencies

```bash
pip install -r requirements.txt
```

---

## Environment Variables

Create a `.env` file:

### Using Groq

```env
GROQ_API_KEY=your_groq_api_key
```

### Using OpenAI

```env
OPENAI_API_KEY=your_openai_api_key
```

---

## Running the Application

Start Streamlit:

```bash
streamlit run app.py
```

The application will be available at:

```text
http://localhost:8501
```

---

## Example Research Topics

* LLM Agents 2025
* CRISPR Gene Editing
* Fusion Energy Progress
* Quantum Computing
* AI in Healthcare
* Autonomous Vehicles
* Climate Technology Innovations

---

## Sample Workflow

### Input

```text
LLM Agents 2025
```

### Output

* Search Results
* Scraped Content
* Final Research Report
* Critic Feedback
* Quality Score

---

## Technologies Used

* Python
* LangChain
* Streamlit
* Groq API / OpenAI API
* BeautifulSoup
* Requests
* Tavily Search
* Pydantic
* Pandas

---

## Future Improvements

* PDF report export
* Citation generation
* Research report history
* Multi-source ranking
* RAG integration
* Agent memory
* Deep research mode
* Report comparison system

---

## Author

**Sandesh B Nayak**

AI/ML Engineer | Generative AI Enthusiast

GitHub: https://github.com/sandeshbnyak

---

## License

This project is licensed under the MIT License.

Feel free to fork, modify, and contribute.
