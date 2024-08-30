# LangChain Documentation Helper

## Overview
LangChain Documentation Helper is a web application designed to assist with learning LangChain by building a generative AI application. This tool answers questions about LangChain using sources from the official LangChain documentation, and integrates a Pinecone vector store for efficient querying.

## Tech Stack
- **Client**: Streamlit
- **Server Side**: LangChain 🦜🔗
- **Vectorstore**: Pinecone 🌲

## Environment Variables
To run this project, you need to add the following environment variables to your `.env` file:
- `PINECONE_API_KEY`
- `OPENAI_API_KEY`

## Run Locally

1. **Clone the project**:
    ```bash
    git clone https://github.com/emarco177/documentation-helper.git
    ```

2. **Go to the project directory**:
    ```bash
    cd documentation-helper
    ```

3. **Download LangChain Documentation**:
    ```bash
    mkdir langchain-docs
    wget -r -A.html -P langchain-docs https://api.python.langchain.com/en/latest
    ```

4. **Install dependencies**:
    ```bash
    pipenv install
    ```

5. **Start the Streamlit server**:
    ```bash
    streamlit run main.py
    ```

## Running Tests
To run tests, execute the following command:
```bash
pipenv run pytest .
