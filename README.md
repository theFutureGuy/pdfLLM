
# Pdf-LLM

This repository contains a Retrieval-Augmented Generation (RAG) pipeline built using LangChain, Ollama, and ChromaDB to interact with PDFs. The purpose of this pipeline is to efficiently retrieve information from PDF documents and generate relevant responses.

## Table of Contents
- [Installation](#installation)
- [Usage](#usage)
- [Project Structure](#project-structure)
- [License](#license)

## Installation

To set up the project, follow these steps:

1. Clone the repository:
    ```sh
    git clone https://github.com/theFutureGuy/pdfLLM.git
    cd pdfLLM
    ```

2. Create and activate a virtual environment (optional but recommended):
    ```sh
    python3 -m venv venv
    source venv/bin/activate
    ```

3. Install the required packages:
    ```sh
    pip install -r requirements.txt
    ```

## Usage

To use the RAG pipeline, follow these steps:

1. Ensure you have the necessary data in the `data` directory. This includes your PDF files.

2. Run the `write_db.py` script to initialize and populate the ChromaDB with your PDF data:
    ```sh
    python write_db.py
    ```

3. Use the `query_data.py` script to query the database and retrieve relevant information:
    ```sh
    python query_data.py "Your query here"
    ```

4. To generate embeddings, use the `get_embedding_function.py` script:
    ```sh
    python get_embedding_function.py
    ```

## Project Structure

- `data/`: Directory to store your PDF files.
- `.gitignore`: Specifies files and directories to be ignored by git.
- `LICENSE`: License information for the project.
- `README.md`: This file.
- `get_embedding_function.py`: Script to generate embeddings using Ollama.
- `query_data.py`: Script to query the database.
- `requirements.txt`: List of required Python packages.
- `test_rag.py`: Script to test the RAG pipeline.
- `write_db.py`: Script to initialize and populate ChromaDB.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more details.
