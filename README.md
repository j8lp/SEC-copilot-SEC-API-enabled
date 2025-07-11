# SEC-copilot 🤖

[Demo](https://www.loom.com/share/a3595d3042414380ba1bd193f4ca0b49?sid=4c441f24-8fea-48ee-b7d3-c4f14685f80b)

An AI copilot allowing users ask natural language questions and get answers about SEC fillings of their choice companies | using Langchain🦜 | OpenAI | Streamlit ⚡| SEC-API 

To use this app, you would need API keys from [OpenAI](https://help.openai.com/en/articles/4936850-where-do-i-find-my-secret-api-key) and [SEC-API](https://sec-api.io/signup)

## Architecture ⚙️

![image](https://github.com/Urias-T/SEC-copilot/assets/51706516/b9a68c09-d622-46d1-ae84-25cbd9aac2a3)



## Quick Start 🚀

App URL: [SEC-copilot](https://sec-copilot.streamlit.app/)

## Running Locally 💻

Follow these steps to set up and run the service locally :

### Prerequisites
- Python 3.8 or higher
- LangChain
- Streamlit
- Git

### Quick Setup (Auto-Activation) 🚀
Clone the repository :

```
git clone https://github.com/Urias-T/SEC-copilot
```

Navigate to the project directory :

```
cd SEC-copilot
```

**Option 1: PowerShell Auto-Setup**
```
.\activate.ps1
```

**Option 2: Command Prompt Auto-Setup**
```
activate.bat
```

**Option 3: VS Code**
- Open the project in VS Code
- The virtual environment will automatically activate
- Use `Ctrl+Shift+P` and run "Tasks: Run Task" → "Run SEC-copilot"

### Manual Setup
Create a virtual environment :

```
python -m venv venv
venv\Scripts\activate
```

Install the required dependencies in the virtual environment :

```
pip install -r requirements.txt
```

Launch the copilot service locally :

```
streamlit run app.py
```

That's it! The service is now up and running on ```localhost:8501```. 🤗

### With Docker 🐋

To run this as a docker container:

Clone the repository:

```
git clone https://github.com/Urias-T/SEC-copilot
```

Navigate to the project directory :

```
cd SEC-copilot
```

Build the Docker image:

```
docker build --build-arg OPENAI_API_KEY=<your_openai_api_key> --build-arg SEC_API_KEY=<your_sec_api_key> -t sec-copilot .
```

*Remember to replace <your_openai_api_key> and <your_sec_api_key> with your actual API keys*

Run the Docker container:

```
docker run -p 8080:8501 -d sec-copilot
```

Congratulations, your service will be running on ```localhost:8080``` 🎉

## Contributing 🙌🏽
If you want to contribute to this project, please open an issue and submit a pull request.


## License ⚖️
This project is made available under the [MIT License](https://github.com/Urias-T/SEC-copilot/blob/main/LICENSE). 
