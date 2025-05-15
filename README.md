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

## Usage
1. Open the application in your web browser (the terminal will provide a local URL).
2. Upload your resume in PDF or TXT format using the file uploader.
3. Optionally, enter the job role you are targeting.
4. Click the "Analyze Resume" button to receive feedback.
5. Review the analysis results displayed on the page.

## Code Explanation
- File Upload: The application allows users to upload their resumes and extracts text from both PDF and TXT files.
- Text Extraction: The extract_text_from_pdf function handles PDF files, while the extract_text_from_file function manages TXT files.
- AI Analysis: Upon clicking the "Analyze Resume" button, the application constructs a prompt for the OpenAI API, requesting feedback on the resume.
- Error Handling: The application includes error handling to manage issues such as empty files or API errors.