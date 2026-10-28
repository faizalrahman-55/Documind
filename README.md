DocuMind — Private AI Document Assistant

Ask questions about your documents using AI, with a focus on privacy and local processing.

DocuMind is an AI-powered document question-answering application that helps users upload documents, retrieve relevant information, and get answers in natural language. It uses Retrieval-Augmented Generation (RAG) to ground answers in document content and supports local language models through Ollama.

Features

- 📄 Document Support — Upload PDF, TXT, and Markdown files.
- 🤖 AI-Powered Q&A — Ask natural-language questions about your documents.
- 🔍 Retrieval-Augmented Generation — Retrieve relevant passages before generating answers.
- 🔒 Privacy-Focused — Use a locally running language model with Ollama.
- 💬 Interactive Interface — Explore document content through a Streamlit web application.
- 🧪 Automated Tests — Run unit tests to verify core functionality.
- ⚙️ Continuous Integration — Use GitHub Actions to automate testing.

Tech Stack

Technology| Purpose
Python| Core application logic
Streamlit| Web interface
Ollama| Local language model runtime
RAG| Document-grounded question answering
Pytest| Automated testing
GitHub Actions| Continuous integration

Project Structure

documind/
├── app.py                 # Streamlit application
├── requirements.txt       # Python dependencies
├── README.md              # Project documentation
├── LICENSE                # MIT license
├── .gitignore             # Files excluded from Git
├── tests/                 # Automated tests
└── .github/
    └── workflows/
        └── tests.yml      # CI workflow

Prerequisites

Before getting started, install:

- Python 3.10 or a compatible version supported by the project dependencies
- Git
- "Ollama" (https://ollama.com/)

Installation

1. Clone the repository

git clone https://github.com/YOUR_USERNAME/documind.git
cd documind

Replace "YOUR_USERNAME" with your GitHub username.

2. Create a virtual environment

python -m venv .venv

Activate it on Windows:

.venv\Scripts\Activate.ps1

Activate it on macOS or Linux:

source .venv/bin/activate

3. Install dependencies

pip install -r requirements.txt

4. Download a local AI model

Make sure Ollama is installed and running, then execute:

ollama pull llama3.2

5. Launch the application

streamlit run app.py

Open the local URL displayed in your terminal, usually "http://localhost:8501".

How to Use

1. Launch DocuMind in your browser.
2. Upload a supported document.
3. Click the document indexing button.
4. Enter a question about the document.
5. Review the generated answer and, where supported, its relevant source passages.

Tip: Ask specific questions for more useful answers. For example, “What are the three main conclusions of this report?”

Run Tests

Run the automated test suite from the project root:

pytest

Privacy and Security

DocuMind is designed to support local document processing and local AI inference. Actual privacy depends on the implementation and configuration of the application and its dependencies.

- Never commit passwords, API keys, credentials, or sensitive ".env" files.
- Keep private documents out of public repositories.
- Verify model and dependency behavior before using confidential information.
- Review generated answers against the original documents.

Roadmap

- [ ] Add semantic search with vector embeddings.
- [ ] Display citations and page numbers for retrieved passages.
- [ ] Support multiple document collections.
- [ ] Add conversation history.
- [ ] Improve document parsing and error handling.
- [ ] Add Docker support.
- [ ] Deploy a public demo with suitable privacy safeguards.

Contributing

Contributions are welcome!

1. Fork the repository.
2. Create a feature branch.
3. Make your changes and add tests.
4. Run the test suite.
5. Submit a pull request describing your changes.

License

This project is distributed under the MIT License. See the "LICENSE" file for details.

Author

Your Name

- GitHub: @faizalrahman-55

---

If you find this project useful, consider giving the repository a ⭐ on GitHub.

Built to explore practical applications of local AI, document retrieval, and Python development.
