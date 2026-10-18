# Word Embedding Based Search Engine

A Python-based semantic search application for e-commerce product discovery, built using Flask, sentence embeddings, and FAISS. The project uses a Flipkart product dataset to support semantic product search, API access, and evaluation workflows.

## Overview

This project explores intelligent product search by:

- Loading and preprocessing product data
- Generating embeddings for product titles and descriptions
- Indexing products using FAISS
- Providing a REST API and web interface
- Supporting evaluation and comparison of search models

## Tech Stack

- Python
- Flask
- FAISS
- Sentence Transformers
- NumPy and pandas
- PyTorch
- OpenAI-compatible LLM integration
- Docker and Docker Compose

## Features

- Semantic product search using embeddings
- Saved vector indexes and model artifacts
- Data preprocessing and enrichment
- Flask API endpoints for product search
- Web interface for browsing and comparing products
- Evaluation scripts and reports
- Docker support

## Project Structure

```text
.
├── app.py
├── config/
├── models/
├── results/
├── scripts/
├── src/
│   ├── api/
│   ├── core/
│   ├── data/
│   ├── evaluation/
│   ├── models/
│   └── utils/
├── templates/
├── tests/
├── requirements.txt
├── Dockerfile
├── docker-compose.yml
├── Makefile
└── .env.example
```

## Prerequisites

- Python 3.10 or later
- pip
- Docker (optional)

## Setup

Clone this repository:

```bash
git clone https://github.com/Hariraavi-code/word-embedding-search-engine.git
cd word-embedding-search-engine
```

Create and activate a virtual environment:

```bash
python -m venv .venv
```

On Windows:

```cmd
.venv\Scripts\activate
```

On Linux or macOS:

```bash
source .venv/bin/activate
```

Install dependencies:

```bash
pip install -r requirements.txt
```

Create your local environment file:

```bash
copy .env.example .env
```

On Linux or macOS, use `cp .env.example .env` instead. Configure any required values in `.env`, and never commit real API keys or secrets.

## Run the Application

```bash
python app.py
```

If the application starts successfully, open:

http://localhost:5000

Alternatively, use Docker:

```bash
docker compose up --build
```

## Models and Data

The repository includes saved model artifacts and a Flipkart product dataset. Depending on the configuration, some features may require additional model downloads or an API key.

## Evaluation

Evaluation scripts and reports are available in the `scripts/` and `results/` directories.

## Acknowledgment

This repository is based on a data science group project. Credit the original contributors and obtain their permission before publicly redistributing their work.

## License

No license has been declared. Check with the original contributors before reusing or redistributing the project.
