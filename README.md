# AI Resume Critiquer

## Overview

The **AI Resume Critiquer** is a web application built using Streamlit that allows users to upload their resumes in PDF or TXT format and receive AI-powered feedback tailored to their job application needs. The application leverages OpenAI's language model to analyze the content of the resume and provide constructive suggestions for improvement.

## Features

- Upload resumes in PDF or TXT format.
- Input the targeted job role for personalized feedback.
- Receive structured analysis focusing on content clarity, skills presentation, experience descriptions, and specific improvements.
- User-friendly interface with real-time feedback.

## Requirements

To run this application, you need the following:
- Python 3.7 or higher
- Streamlit
- PyPDF2
- OpenAI Python client
- python-dotenv

You can install the required packages using pip:

```bash
pip install streamlit PyPDF2 openai python-dotenv
```

## Setup
1. Clone the respository (if applicable):
```bash
git clone https://github.com/SamraAzizi/resumeCritiquer.git
cd resumeCritiquer
```

2. Create a .env file in the root directory of the project and add your OpenAI API key:

```bash
OPENAI_API_KEY=your_openai_api_key_here
```

3. Run the application:
```bash
streamlit run main.py
```

