# ADR-Sys
# AI-Powered Automated Document Redaction System (ADR-Sys)

## Overview
ADR-Sys is an AI-driven system that automatically redacts sensitive information from documents using Natural Language Processing (NLP) and Optical Character Recognition (OCR). The system includes an MLOps pipeline for data processing, model training, deployment, and monitoring.

## Features
- **Text Redaction:** Detects and removes PII (e.g., names, emails, addresses).
- **Image Redaction:** OCR-based redaction for scanned documents.
- **MLOps Pipeline:** Automated model training and monitoring.
- **API Access:** FastAPI-based backend for document processing.

## Tech Stack
- **ML & NLP:** SpaCy, Hugging Face Transformers
- **OCR:**  EasyOCR
- **MLOps:** MLflow, DVC, Prometheus, Grafana
- **Infrastructure:** FastAPI, PostgreSQL, MinIO, Docker, Kubernetes

## Dataset
- [PII-NER Dataset](https://huggingface.co/datasets/Josephgflowers/PII-NER)

## Setup Instructions
1. **Clone the Repository**
   ```bash
   git clone https://github.com/your-repo/adr-sys.git
   cd adr-sys
   ```
2. **Set up Virtual Environment**
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```
3. **Install Dependencies**
   ```bash
   pip install -r requirements.txt
   ```
4. **Run the FastAPI Server**
   ```bash
   uvicorn app.main:app --reload
   ```
5. **Access API Documentation**
   - Open `http://127.0.0.1:8000/docs`

## License
This project is licensed under the MIT License.


