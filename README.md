# chat-rag
Open source project, to serve the purposes of exploiting large language models in answering user questions based on specific documents.


## Requirements

- Python 3.8 or later

### Install Python using MiniConda

1) Download and install MiniConda From [here](https://docs.anaconda.com/free/miniconda/#quick-command-line-install)
2) Create a new environment using the following command:
```bash
$ conda create -n chat-rag-app python=3.8
```

Another way to create a new environment is by using the following command:
```bash
$ conda create --name chat-rag-app python=3.8
```

3) Activate the environment:
```bash
$ conda activate chat-rag-app
```

### (Optional) Setup your command line for better readability
```bash
export PS1=export PS1="\[\033[01;32m\]\u@\h:\w\n\[\033[00m\]\$ "
```

## Installation

### Install the required packages

```bash
$ pip install -r requirements.txt
```

### Setup the environment variables

```bash
$ cp .env.example .env
```

Set your environment variables in the `.env` file. Like `OPENAI_API_KEY` value.

## Run the FastAPI server

```bash
$ uvicorn main:app --reload --host 0.0.0.0 --port 5000
```
