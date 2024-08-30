# LangChain Documentation Helper

## Overview
LangChain Documentation Helper is a web application built to facilitate learning LangChain by creating a generative AI application. The app answers questions about LangChain using data sourced from the official LangChain documentation and employs Pinecone as a vector store for optimized search.

## Tech Stack
- **Client**: Streamlit
- **Server Side**: LangChain 🦜🔗
- **Vectorstore**: Pinecone 🌲

## Environment Variables
To run this project, you will need to add the following environment variables to your `.env` file:
- `PINECONE_API_KEY`
- `OPENAI_API_KEY`

## Run Locally

1. **Clone the project**:
    ```bash
    git clone https://github.com/melikaknight/Documentation-Helper_LLM.git
    ```

2. **Go to the project directory**:
    ```bash
    cd Documentation-Helper_LLM
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
To run tests, use the following command:
```bash
pipenv run pytest .
