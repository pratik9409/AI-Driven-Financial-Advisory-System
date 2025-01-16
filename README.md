# AI-Driven-Financial-Advisory-System


### Description
This project integrates advanced AI capabilities to provide financial analytics and investment insights using IBM Watson's foundation models and LangChain's planning and execution tools. The system processes user input, fetches live financial data, and generates comprehensive investment insights.

### Features
AI-Powered Analysis: Leverages IBM Watson’s LLama2-70B-chat for generating insights.
Dynamic News Extraction: Fetches recent financial news via Yahoo Finance and Google News.
Financial Data Export: Downloads balance sheets, income statements, and cash flow statements for any given stock ticker.
Flask Integration: Web interface for user interaction.
Extensible and Modular: Built with tools and templates for easy customization.
Installation and Setup
Prerequisites:

Python 3.8+
Pip (Python package manager)
API keys for IBM Watson and Serper (Google search API)
### Clone the Repository:

```bash
git clone https://github.com/yourusername/financial-advisory-ai.git
cd financial-advisory-ai
```

### Install Dependencies:
```bash
pip install -r requirements.txt
```


### Configure API Keys:
Replace your apikey in model.py with your IBM Watson API key.
Replace YOUR_SERPER_API_KEY in worker.py with your Serper API key.

### Run the Server:
```bash
python server.py
```

Access the Application:

Open your browser and go to http://localhost:8000.

### File Structure
model.py: Initializes IBM Watson's LLama2 model with custom parameters for token generation and temperature control.
worker.py: Implements tools to fetch financial data and generate insights using LangChain.
server.py: Hosts a Flask server to interact with the user and relay their input to the processing pipeline.

### How It Works
User submits a stock ticker (e.g., AAPL) via the web interface.
The system fetches financial data (news, stock prices, statements) and processes it using IBM Watson and LangChain agents.
A detailed investment report is generated and returned.
