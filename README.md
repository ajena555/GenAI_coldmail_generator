## Cold Mail Generator

A Generative AI-powered platform that automates cold email outreach to companies based on job listings — saving time, effort, and cost in finding the right tech talent.

Project Overview

**Cold Mail Generator** is a proof-of-concept application that simulates how a service company could reach out to potential clients using smart, personalized cold emails. By extracting key job requirements from a job post URL, the app crafts a tailored outreach email offering relevant tech talent.

This project showcases the real-world application of **Generative AI**, **LLMs**, and **vector search** to solve modern recruiting and sales outreach challenges.

---

## Problem Statement

Hiring skilled tech talent for short-term or urgent roles is often slow and expensive. Companies must post job listings, screen resumes, and go through lengthy hiring processes.

## Solution

A fictional service brand uses this app to:
- Parse job listings from company career portals.
- Understand required skills using LLMs.
- Match internal talent portfolios.
- Automatically generate personalized cold emails for outreach.

---

## Tech Stack

| Tool | Purpose |
|------|---------|
| **Llama 3.1** | Large Language Model used for job parsing and email generation |
| **LangChain** | LLM orchestration and chaining of tasks |
| **ChromaDB** | Vector database to store and retrieve tech portfolio data |
| **Streamlit** | Web UI framework to interact with the app |


## Installation & Setup

1. **Clone the repository**
   git clone https://github.com/yourusername/cold-mail-generator.git
   cd cold-mail-generator

2. **Create a virtual environment**
  python -m venv venv
  source venv/bin/activate  # or venv\Scripts\activate on Windows.

3. **Install requirements**
pip install -r requirements.txt

4. **Run the app**
streamlit run main.py


📝 How It Works
Enter a URL of a job listing.
The app scrapes and cleans the job description.
It uses Llama 3.1 (via LangChain) to extract skills and role details.
Queries ChromaDB to retrieve matching internal talent profiles.
Generates a personalized cold email pitch.
