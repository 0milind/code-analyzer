# Code Analysis AI Agent

## Overview
The **Code Analysis AI Agent** is a Streamlit-based application that allows users to analyze code snippets written in C, C++, Java, or Python. It utilizes Google's Gemini AI model to provide insights and explanations about the given code, supplemented by web research via DuckDuckGo.

## Features
- Accepts code snippets in C, C++, Java, and Python.
- Answers user queries related to the provided code.
- Uses Google's Gemini AI model for intelligent analysis.
- Fetches supplementary information using DuckDuckGo.
- User-friendly Streamlit interface.

## Setup Instructions

### 1. Clone the Repository
Ensure you have `git` installed and clone the repository:
```sh
 git clone <repository-url>
 cd <repository-folder>
```

### 2. Create a Virtual Environment
It's recommended to create a virtual environment for dependency management:
```sh
python -m venv venv
source venv/bin/activate  # On macOS/Linux
venv\Scripts\activate    # On Windows
```

### 3. Install Dependencies
Install the required dependencies using the following command:
```sh
pip install -r req.txt
```

### 4. Set Up API Keys
Create a `.env` file in the root directory and add the following keys:
```
OPENAI_API_KEY="your-openai-key"
GOOGLE_API_KEY="your-google-key"
GROQ_API_KEY="your-groq-key"
PHIDATA_API_KEY="your-phidata-key"
```
Replace `your-<provider>-key` with your actual API keys.

### 5. Run the Application
Start the Streamlit application by running:
```sh
streamlit run code_qa_agent.py
```

## Usage
1. Enter a code snippet in the provided text area.
2. Type a query related to the code.
3. Click on **Analyze Code** to receive AI-generated insights.
4. View the response in the output section.

## Dependencies
The application requires the following Python libraries:
- `phidata`
- `python-dotenv`
- `yfinance`
- `packaging`
- `duckduckgo-search`
- `fastapi`
- `uvicorn`
- `groq`
- `openai`
- `sqlalchemy`
- `pgvector`
- `psycopg[binary]`
- `pypdf`
- `streamlit`
- `google-generativeai`

## Author
**Milind Mohapatra**

## License
This project is licensed under the MIT License.

